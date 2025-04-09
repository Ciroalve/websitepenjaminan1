<template>
    <nav class="navbar">
      <div class="navbar-container">
        <div class="navbar-logo">
          <img src="/assets/img/gambar.jpg" alt="Logo" class="logo" />
          <span class="navbar-title">UNIVERSITAS MAYASARI BAKTI</span>
          <span class="navbar-subtitle"></span>
        </div>
        <ul class="navbar-menu">
          <li><a href="/statistik">STATISTIK</a></li>
          <li><a href="/dokumen">DOKUMEN</a></li>
          <li><a href="/tentang-kami">TENTANG KAMI</a></li>
          <li><a href="/Galeri">Galeri</a></li>
          <li><a href="/login" class="login-link">Login</a></li>
        </ul>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: "Navbar",
  };
  </script>
  
  <style scoped>
  .navbar {
    background-color: #f8f9fa;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .navbar-container {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
  }
  
  .navbar-logo {
    display: flex;
    align-items: center;
  }
  
  .logo {
    height: 40px;
    margin-right: 10px;
  }
  
  .navbar-title {
    font-size: 18px;
    font-weight: bold;
    color: #000;
  }
  
  .navbar-subtitle {
    font-size: 14px;
    color: #555;
    margin-left: 5px;
  }
  
  .navbar-menu {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
  }
  
  .navbar-menu li {
    margin: 0 10px;
  }
  
  .navbar-menu a {
    text-decoration: none;
    color: #007bff;
    font-weight: bold;
    font-size: 14px;
  }
  
  .navbar-menu .login-link {
    color: #333;
  }
  </style>