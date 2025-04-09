<template>
    <div class="slider">
         
         <div class="owl-carousel ">
             <div class="slider-img">
                 <div class="item">
                     <div class="slider-img"><img src="assets/img/image.png" alt="" style="width: 40%; height: auto; object-fit: cover;"></div>
                     <div class="container">
                         <div class="row">
                             <div class="col-lg-offset-2 col-lg-8 col-md-offset-2 col-md-8 col-sm-12 col-xs-12">
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
     
   
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
   
         <div class="container">
           <h1>Dokumen</h1>
           <p>Kumpulan Dokumen SPMI</p>
           <div class="list">
             <button>KEBIJAKAN MUTU </button>
             <button>MANUAL MUTU </button>
             <button>STANDAR MUTU </button>  
             <button>SOP </button>
             <button>INDIKATOR KINERJA (IK)  </button>
             <button>FORMULIR YANG DI GUNAKAN </button>
           </div>
           <div class="help-box">
             <p>Anda Butuh Bantuan?</p>
             <button>Hubungi Kami</button>
           </div>
         </div>
       </div>
     <footer class="bg-gray-200 text-gray-700 py-6">
         <div class="container mx-auto px-4 flex justify-between">
           <div>
             <h4 class="font-bold">Sistem Informasi Penjaminan Mutu Internal</h4>
             <p class="text-sm">Universitas Mayasari Bakti</p>
             <p class="mt-2 text-sm">Jl. Tamansari No.48, Sukahurip, Kec. Tamansari, Kab. Tasikmalaya, Jawa Barat 46196</p>
             <p class="mt-2 text-sm">📞 +62 811 7460 411</p>
             <p class="text-sm">✉ info@umb.ac.id</p>
           </div>
           <div>
             <h4 class="font-bold">LINK</h4>
             <ul class="text-sm mt-2">
               <li><a href="#" class="hover:underline">Website</a></li>
               <li><a href="#" class="hover:underline">Tentang Kami</a></li>
               <li><a href="#" class="hover:underline">Visi Misi</a></li>
             </ul>
           </div>
           <div>
             <h4 class="font-bold">BANTUAN</h4>
             <ul class="text-sm mt-2">
               <li><a href="#" class="hover:underline">Pusat Layanan</a></li>
               <li><a href="#" class="hover:underline">Cara Penggunaan</a></li>
               <li><a href="#" class="hover:underline">Kebijakan</a></li>
             </ul>
           </div>
         </div>
         <div class="text-center mt-4 text-sm text-gray-500">&copy; 2025 Universitas Mayasari Bakti - Semua Hak Dilindungi</div>
       </footer>
   </template>
   
   <style scoped>
   
   /* Style untuk slider */
   .slider {
       position: relative;
       width: 100%;
       overflow: hidden;
   }
   
   /* Style untuk setiap item slider */
   .slider .item {
       position: relative;
       text-align: center;
       width: 100%;
       animation: fadeIn 1.5s ease-in-out;
   }
   .slider-img img {
       max-width: 40%; /* Sesuaikan sesuai kebutuhan */
       height: auto;
       object-fit: cover;
   }
   
   /* Animasi untuk gambar slider */
   @keyframes fadeIn {
       from {
           opacity: 0;
           transform: translateY(20px);
       }
       to {
           opacity: 1;
           transform: translateY(0);
       }
   }
   
   /* Gaya untuk gambar dalam slider */
   .slider-img img {
       width: 50%; /* Ukuran gambar diperkecil */
       height: auto;
       object-fit: cover;
       transition: transform 0.5s ease-in-out;
   }
   
   .slider-img img:hover {
       transform: scale(1.05);
   }
   
   /* Gaya untuk teks dan tombol di slider */
   .slider-captions {
       position: absolute;
       top: 50%;
       left: 50%;
       transform: translate(-50%, -50%);
       text-align: center;
       color: #fff;
       background: rgba(0, 0, 0, 0.5);
       padding: 20px;
       border-radius: 10px;
       animation: fadeIn 1.5s ease-in-out;
   }
   
   .slider-title {
       font-size: 32px;
       font-weight: bold;
       margin-bottom: 10px;
       animation: fadeIn 2s ease-in-out;
   }
   
   .slider-text {
       font-size: 18px;
       margin-bottom: 15px;
       animation: fadeIn 2.5s ease-in-out;
   }
   
   .btn-success {
       background-color: #28a745;
       color: white;
       padding: 10px 20px;
       text-decoration: none;
       border-radius: 5px;
       transition: background-color 0.3s, transform 0.3s;
   }
   
   .btn-success:hover {
       background-color: #218838;
       transform: scale(1.1);
   }
   
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
   /* Footer Styling */
   footer {
     background-color: #f3f4f6;
     color: #4b5563;
     padding: 2rem 0;
   }
   
   footer .container {
     display: flex;
     justify-content: space-between;
     flex-wrap: wrap;
   }
   
   footer h4 {
     font-weight: bold;
     margin-bottom: 0.75rem;
   }
   
   footer ul {
     list-style: none;
     padding: 0;
   }
   
   footer ul li {
     margin-bottom: 0.5rem;
   }
   
   footer ul li a {
     text-decoration: none;
     color: #4b5563;
     transition: color 0.3s ease-in-out;
   }
   
   footer ul li a:hover {
     text-decoration: underline;
     color: #dc2626;
   }
   
   footer p {
     font-size: 0.875rem;
     margin-bottom: 0.5rem;
   }
   
   footer .text-center {
     margin-top: 1rem;
     font-size: 0.75rem;
     color: #6b7280;
   }
   
   /* Documents Section */
   .list {
     display: flex;
     flex-direction: column;
     align-items: center;
     gap: 10px;
   }
   
   .list button {
     width: 100%;
     max-width: 400px;
     padding: 10px;
     background-color: #f3f4f6;
     border: 1px solid #d1d5db;
     border-radius: 5px;
     cursor: pointer;
     font-weight: bold;
     transition: background-color 0.3s ease-in-out;
   }
   
   .list button:hover {
     background-color: #e5e7eb;
   }
   
   .help-box {
     margin-top: 20px;
     background-color: #3b82f6;
     color: white;
     padding: 20px;
     border-radius: 10px;
     text-align: center;
   }
   
   .help-box button {
     margin-top: 10px;
     padding: 10px 20px;
     background-color: #f59e0b;
     border: none;
     border-radius: 5px;
     cursor: pointer;
     font-weight: bold;
     transition: background-color 0.3s ease-in-out;
   }
   
   .help-box button:hover {
     background-color: #d97706;
   }
   </style>  
   
