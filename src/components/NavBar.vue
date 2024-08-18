<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-white shadow ">
      <div class="container">
        <a class="navbar-brand" href="/">
          <img src="@/assets/img/logo-black.png" class="dark-logo img-fluid" alt="Logo">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end" id="navbarResponsive">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <router-link class="nav-link" to="/about">關於昶安</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/products">產品資訊</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/skills">專業技術</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/videos">影音專區</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/contact">聯絡我們</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'NavBar'
  }
  </script>
  