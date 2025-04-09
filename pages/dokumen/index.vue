<template>
  <div class="container">
    <h1 class="title">Buat dan Unduh PDF</h1>
    <textarea v-model="content" class="text-area" placeholder="Tulis sesuatu..."></textarea>
    <button @click="downloadPDF" class="download-button">Download PDF</button>
    <button @click="kirimriwayat" class="download-button secondary">Kirim ke Riwayat</button>

    <h2 class="subtitle">Riwayat PDF</h2>
    <ul class="history-list">
      <li v-for="(item, index) in history" :key="index" class="history-item">
        <div @click="viewPDF(item.url)">
          PDF {{ index + 1 }} - {{ item.timestamp }}
          <span v-if="!item.url" class="no-pdf" @click="hapusRiwayat(index)">(Hapus PDF)</span>
        </div>
        <button class="delete-button" @click="hapusRiwayat(index)">Hapus</button>
      </li>
    </ul>

    <iframe v-if="pdfUrl" :src="pdfUrl" class="pdf-viewer"></iframe>
  </div>
</template>

<script>

export default {
  data() {
    return {
      content: "",
      pdfUrl: "",
      history: []
    };
  },
  methods: {
    downloadPDF() {
      const doc = new jsPDF();
      const textLines = doc.splitTextToSize(this.content, 180);
      doc.text(textLines, 10, 10);
      const pdfBlob = doc.output("blob");
      const pdfUrl = URL.createObjectURL(pdfBlob);

      this.history.unshift({
        url: pdfUrl,
        timestamp: new Date().toLocaleString(),
        content: this.content
      });

      this.pdfUrl = pdfUrl;

      doc.save("document.pdf");
    },
    kirimriwayat() {
      this.history.unshift({
        url: "",
        timestamp: new Date().toLocaleString(),
        content: this.content
      });
    },
    viewPDF(url, index) {
  if (url) {
    this.pdfUrl = url;
  } else {
    if (confirm("Riwayat ini tidak memiliki file PDF. Hapus dari riwayat?")) {
      this.history.splice(index, 1);
    }
  }
}

    },
    reuseContent(text) {
      this.content = text;
    }
  }

</script>

<style scoped>
.container {
  max-width: 600px;
  margin: 20px auto;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.1);
  text-align: center;
}
.title {
  font-size: 24px;
  margin-bottom: 10px;
}
.subtitle {
  font-size: 18px;
  margin-top: 20px;
}
.text-area {
  width: 100%;
  height: 150px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}
.download-button {
  margin-top: 10px;
  margin-right: 10px;
  padding: 10px 20px;
  background-color: #3498db;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
.download-button.secondary {
  background-color: #f39c12;
}
.pdf-viewer {
  width: 100%;
  height: 500px;
  margin-top: 20px;
  border: 1px solid #ccc;
}
.history-list {
  list-style: none;
  padding: 0;
  text-align: left;
  margin-top: 10px;
}
.history-item {
  padding: 8px;
  border-bottom: 1px solid #eee;
  transition: background-color 0.2s;
}
.history-item:hover {
  background-color: #f9f9f9;
}
.reuse-button {
  margin-top: 5px;
  padding: 5px 10px;
  font-size: 12px;
  background-color: #2ecc71;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
.no-pdf {
  color: #e74c3c;
  font-size: 12px;
  margin-left: 8px;
  font-style: italic;
  cursor: pointer;
  text-decoration: underline;
}

</style>
