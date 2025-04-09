<template>
    <div class="tentang-kami">
      <div class="container">
        <h1>Tentang Universitas Mayasari Bakti</h1>
        <p>
          Universitas Mayasari Bakti (UMB) adalah lembaga pendidikan tinggi yang berkomitmen untuk mencetak generasi unggul
          dengan kompetensi global dan karakter yang kuat. Kami menawarkan pendidikan berkualitas di berbagai disiplin ilmu
          untuk membangun masa depan yang lebih baik.
        </p>
  
        <section class="sejarah">
          <h2>Sejarah</h2>
          <p>
            Universitas Mayasari Bakti didirikan pada tahun 1995 dengan visi untuk menjadi pusat pendidikan dan inovasi di
            Indonesia. Sejak awal berdirinya, UMB telah berkembang menjadi institusi yang dikenal karena kualitas pengajaran,
            penelitian, dan pengabdian masyarakat.
          </p>
        </section>
  
        <section class="visi-misi">
          <div class="visi">
            <h2>Visi</h2>
            <p>
              Menjadi universitas unggulan yang berkontribusi dalam pengembangan ilmu pengetahuan, teknologi, dan seni untuk
              kemajuan bangsa.
            </p>
          </div>
          <div class="misi">
            <h2>Misi</h2>
            <ul>
              <li>
                Menyediakan pendidikan yang bermutu tinggi dan relevan dengan kebutuhan global.
              </li>
              <li>
                Mengembangkan penelitian inovatif yang bermanfaat bagi masyarakat.
              </li>
              <li>
                Meningkatkan kerjasama dengan institusi nasional dan internasional.
              </li>
              <li>
                Membentuk lulusan yang memiliki kompetensi akademik dan karakter profesional.
              </li>
            </ul>
          </div>
        </section>
  
        <section class="kontak">
          <h2>Kontak Kami</h2>
          <p>
            Jika Anda membutuhkan informasi lebih lanjut tentang Universitas Mayasari Bakti, silakan hubungi kami melalui:
          </p>
          <ul>
            <li>Email: <a href="mailto:info@umb.ac.id">info@umb.ac.id</a></li>
            <li>Telepon: (021) 87654321</li>
            <li>Alamat: Jl. Pendidikan No. 10, Kota Tasikmalaya, Jawa Barat</li>
          </ul>
        </section>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TentangKamiUMB',
  };
  </script>
  
  <style scoped>
  /* Gaya untuk halaman Tentang Kami Universitas Mayasari Bakti */
  .container {
    width: 80%;
    margin: 0 auto;
    font-family: Arial, sans-serif;
    line-height: 1.6;
  }
  
  h1 {
    text-align: center;
    margin-bottom: 20px;
    font-size: 2.5rem;
    color: #2a5298;
  }
  
  p {
    margin-bottom: 15px;
    font-size: 1rem;
  }
  
  .sejarah,
  .visi,
  .misi,
  .kontak {
    margin-top: 20px;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  }
  
  h2 {
    font-size: 1.5rem;
    margin-bottom: 10px;
    color: #3a7ca5;
  }
  
  ul {
    list-style: disc;
    margin-left: 20px;
  }
  
  .kontak ul {
    list-style: none;
    padding: 0;
  }
  
  .kontak li {
    margin-bottom: 10px;
  }
  
  a {
    color: #2a5298;
    text-decoration: none;
    font-weight: bold;
  }
  
  a:hover {
    text-decoration: underline;
  }
  </style>
  