<template>
  <header
    class="page-kv"
    style="background-image: url(${backgroundImage)"
  >
    <div class="kv-caption" data-aos="zoom-in" data-aos-duration="500">
      <h3 class="font-weight-bold text-white text-shadow mb-0">產品資訊</h3>
      <h5 class="font-weight-bold text-white text-shadow mb-0">
        Product Information
      </h5>
    </div>
  </header>

  <!-- Content Section -->
  <section class="content">
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />

    <div
      class="row-odd"
      data-aos="fade-down"
      data-aos-delay="500"
      data-aos-duration="800"
    >
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-5 col-12 order-md-2">
            <img src="@/assets/img/1130311122948.png" class="img-fluid" />
          </div>

          <div class="col-lg-7 col-12 order-md-1">
            <div class="product-block pb-4">
              <h2 class="sec-title">ADP地瓜葉植化素</h2>
              <h5 class="sec-infos">
                含有豐富的膳食纖維、維生素A、C、葉酸及礦物質鈣、鐵。
                可促使血糖進入肝臟合成運用，維持血液中血糖的恆定。
                維持良好的血循、防止白內障、視網膜病變等眼疾。
              </h5>
              <div class="row pt-md-4">
                <div class="col-lg-6 col-12 mb-4">
                  <a
                    href="contact.php?item=ADP地瓜葉植化素#contactus"
                    class="btn-main bg-main-gradient"
                    >立即諮詢</a
                  >
                </div>
                <div class="col-lg-6 col-12 mb-4"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div
      class="row-even"
      data-aos="fade-down"
      data-aos-delay="500"
      data-aos-duration="800"
    >
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-5 col-12 order-md-1">
            <img src="@/assets/img/1130311122906.png" class="img-fluid" />
          </div>

          <div class="col-lg-7 col-12 order-md-2">
            <div class="product-block pb-4">
              <h2 class="sec-title">ADP木瓜鳳梨酵素</h2>
              <h5 class="sec-infos">
                可促進食慾、腸道蠕動及新陳代謝。 幫助消化、維持消化道機能
                養顏美容。幫助入睡、營養補給。健康維持
              </h5>
              <div class="row pt-md-4">
                <div class="col-lg-6 col-12 mb-4">
                  <a
                    href="contact.php?item=ADP木瓜鳳梨酵素#contactus"
                    class="btn-main bg-main-gradient"
                    >立即諮詢</a
                  >
                </div>
                <div class="col-lg-6 col-12 mb-4"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div
      class="row-odd"
      data-aos="fade-down"
      data-aos-delay="500"
      data-aos-duration="800"
    >
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-5 col-12 order-md-2">
            <img src="@/assets/img/1130311092054.png" class="img-fluid" />
          </div>

          <div class="col-lg-7 col-12 order-md-1">
            <div class="product-block pb-4">
              <h2 class="sec-title">ADP丁香魚</h2>
              <h5 class="sec-infos">
                丁香魚含有豐富的鈣質、胺基酸。 EPA、DHA，能預防心血管疾病。
              </h5>
              <div class="row pt-md-4">
                <div class="col-lg-6 col-12 mb-4">
                  <a
                    href="contact.php?item= ADP丁香魚#contactus"
                    class="btn-main bg-main-gradient"
                    >立即諮詢</a
                  >
                </div>
                <div class="col-lg-6 col-12 mb-4"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div
      class="row-even"
      data-aos="fade-down"
      data-aos-delay="500"
      data-aos-duration="800"
    >
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-5 col-12 order-md-1">
            <img src="@/assets/img/1130311091717.png" class="img-fluid" />
          </div>

          <div class="col-lg-7 col-12 order-md-2">
            <div class="product-block pb-4">
              <h2 class="sec-title">ADP黑糖薑 超微粉末</h2>
              <h5 class="sec-infos"></h5>
              <div class="row pt-md-4">
                <div class="col-lg-6 col-12 mb-4">
                  <a
                    href="contact.php?item=ADP黑糖薑 超微粉末#contactus"
                    class="btn-main bg-main-gradient"
                    >立即諮詢</a
                  >
                </div>
                <div class="col-lg-6 col-12 mb-4"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  
</template>

<script>
export default {
  name: "ProductView",
  data() {
    return {
      backgroundImage: require('@/assets/img/kv-p.jpg')
    }
  }
};
</script>
