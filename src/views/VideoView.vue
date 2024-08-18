<template>
  <header
    class="page-kv"
    :style="{ backgroundImage: `url(${backgroundImage})` }"
  >
    <div class="kv-caption" data-aos="zoom-in" data-aos-duration="500">
      <h3 class="font-weight-bold text-white text-shadow mb-0">影音專區</h3>
      <h5 class="font-weight-bold text-white text-shadow mb-0">
        Audio And Video
      </h5>
    </div>
  </header>

  <!-- Content Section -->
  <section class="content">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <div class="row">
            <meta
              http-equiv="Content-Type"
              content="text/html; charset=utf-8"
            />

            <div class="col-md-4 col-12 mb-md-4 mb-3">
              <div class="card border-0 p-0">
                <div class="card-img">
                  <a
                    href="https://www.youtube.com"
                    target="_blank"
                    class="hover-img"
                  >
                    <img
                      class="card-img-top"
                      src="@/assets/img/1130312105942.jpg"
                      alt="video 01"
                    />
                  </a>
                </div>
                <div class="card-body px-0">
                  <a href="https://www.youtube.com" target="_blank">
                    <h5 class="text-dark">台灣最新研發成果，ADP破壁防護噴粉</h5>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <nav class="py-5" aria-label="Page navigation">
        <div
          class="col-lg-12 col-md-12 col-sm-12 text-center"
          style="margin-top: 50px"
        >
          <div style="height: 20px"></div>
        </div>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: "VideoView",
  data() {
    return {
      backgroundImage: require("@/assets/img/kv-v.jpg"),
    };
  },
};
</script>
