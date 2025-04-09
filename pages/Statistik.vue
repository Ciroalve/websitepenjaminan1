<template>
    <div class="data-grafik">
      <div class="header">
        <h2>Data Grafik</h2>
        <p>Statistik Penjaminan Mutu</p>
      </div>
      <div class="cards-container">
        <div class="card">
          <h3>Persentase Standar Mutu</h3>
          <p>
            Standar Mutu adalah kesepakatan yang telah disepakati bersama oleh
            sekelompok orang atau organisasi dan telah didokumentasikan yang
            terdiri dari spesifikasi teknis dan kriteria akurat yang digunakan
            sebagai peraturan, petunjuk atau definisi tertentu untuk menjamin
            kualitas suatu barang, produk, proses atau jasa sesuai dengan yang
            telah dinyatakan dan disepakati.
          </p>
        </div>
        <div class="card">
          <h3>Persentase Evaluasi</h3>
          <p>Evaluasi adalah proses penilaian untuk menentukan kualitas, efektivitas, atau pencapaian suatu kegiatan.</p>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .data-grafik {
    font-family: Arial, sans-serif;
    background-color: #f4f7fa;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  }
  
  .header {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .header h2 {
    font-size: 2rem;
    color: #2a5298;
    margin-bottom: 10px;
  }
  
  .header p {
    font-size: 1rem;
    color: #555;
  }
  
  .cards-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
  }
  
  .card {
    background-color: #ffffff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  
  .card h3 {
    font-size: 1.25rem;
    color: #3a7ca5;
    margin-bottom: 10px;
  }
  
  .card p {
    font-size: 1rem;
    color: #666;
  }
  
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
  }
  </style>
  