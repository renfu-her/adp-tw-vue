<template>
    <footer class="sec-footer py-5 bg-main-gradient">
      <div class="container">
        <div class="d-flex flex-md-row flex-column justify-content-md-between justify-content-start align-items-md-center w-100">
          <div class="d-flex flex-md-row flex-column align-items-md-center">
            <ul class="link-group">
              <li><a href="tel:+886-6-2791367" class="text-white"><i class="fas fa-phone footer-listicon"></i>(06)279-1367</a></li>
              <li><a href="https://maps.app.goo.gl/RoF5fMJEQRY5JgFm6" class="text-white" target="_blank"><i class="fas fa-map-marker-alt footer-listicon"></i>臺南市仁德區一甲里19鄰太乙三街21號</a></li>
            </ul>
          </div>
          <span class="m-0 text-md-right text-left text-nowrap text-white">Copyright &copy; {{ currentYear }} <br> 昶安奈米應用科技有限公司</span>
        </div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterComponent',
    computed: {
      currentYear() {
        return new Date().getFullYear()
      }
    }
  }
  </script>