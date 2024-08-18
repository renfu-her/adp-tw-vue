<template>
  <header
    class="page-kv"
    :style="{ backgroundImage: `url(${backgroundImage})` }"
  >
    <div class="kv-caption" data-aos="zoom-in" data-aos-duration="500">
      <h3 class="font-weight-bold text-white text-shadow mb-0">聯絡我們</h3>
      <h5 id="contactus" class="font-weight-bold text-white text-shadow mb-0">
        Contact Us
      </h5>
    </div>
  </header>

  <!-- Content Section -->
  <section class="content">
    <div class="container">
      <div class="row justify-content-between pb-md-5">
        <div class="col-lg-6 col-12 pb-md-4 pb-5">
          <div class="row">
            <div class="col-12 px-md-3 px-0" id="form-anchor">
              <h2 class="page-title text-center" id="contactus">聯絡我們</h2>
              <h5 class="text-lightdark text-center mb-4">
                請完成下方諮詢表單並送出，我們將會安排專人與您聯繫。
              </h5>

              <form
                action="send_contact.php"
                method="post"
                class="contactform needs-validation"
              >
                <div class="form-group">
                  <label for="contact_name" required="">姓名</label>
                  <input
                    type="text"
                    class="form-control form-control-lg"
                    id="contact_name"
                    name="contact_name"
                    required
                  />
                </div>
                <div class="form-group">
                  <label for="contact_tel" required="">聯絡電話</label>
                  <input
                    type="phone"
                    class="form-control form-control-lg"
                    id="contact_tel"
                    name="contact_tel"
                    required
                  />
                </div>
                <div class="form-group">
                  <label for="contact_email" required="">電子郵件</label>
                  <input
                    type="email"
                    class="form-control form-control-lg"
                    id="contact_email"
                    name="contact_email"
                    required
                  />
                </div>
                <div class="form-group">
                  <label for="contact_objects">諮詢商品</label>
                  <input
                    type="text"
                    class="form-control form-control-lg"
                    id="contact_objects"
                    name="contact_objects"
                    value=""
                  />
                </div>
                <div class="form-group">
                  <label for="contact_message">諮詢內容</label>
                  <textarea
                    class="form-control form-control-lg"
                    id="contact_message"
                    name="contact_message"
                    rows="4"
                  ></textarea>
                </div>
                <div class="w-100 text-center mb-3">
                  <div ref="recaptcha"></div>
                </div>

                <input
                  type="submit"
                  class="btn btn-main bg-main-gradient w-100 py-0"
                  value="送出"
                />
              </form>
            </div>
          </div>
        </div>
        <div class="col-lg-5 col-12 pb-md-4 pb-5">
          <div class="row align-items-center">
            <div class="col-12 mb-md-4 px-0">
              <ul class="link-group mt-md-5">
                <li class="w-100">
                  <a href="#"
                    ><img
                      src="@/assets/img/ic-home.svg"
                      class="footer-listicon"
                    />昶安奈米應用生技有限公司</a
                  >
                </li>
                <li class="w-100">
                  <a href="tel:+886-6-2791367"
                    ><img
                      src="@/assets/img/ic-cellphone.svg"
                      class="footer-listicon"
                    />(06)279-1367</a
                  >
                </li>
                <li class="w-100">
                  <a
                    href="https://maps.app.goo.gl/RoF5fMJEQRY5JgFm6"
                    target="_blank"
                    ><img
                      src="@/assets/img/ic-marker1.svg"
                      class="footer-listicon"
                    />臺南市仁德區一甲里19鄰太乙三街21號</a
                  >
                </li>
              </ul>
            </div>
            <div class="col-12 px-0">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d918.2924174456425!2d120.2523489!3d22.980787499999998!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x346e714d5bf93155%3A0xaf7280ff8de3fc7b!2zNzE35Y-w5Y2X5biC5LuB5b635Y2A5aSq5LmZ5LiJ6KGXMjHomZ8!5e0!3m2!1szh-TW!2stw!4v1708797895365!5m2!1szh-TW!2stw"
                width="100%"
                height="600"
                style="border: 0"
                allowfullscreen=""
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactView",
  data() {
    return {
      backgroundImage: require("@/assets/img/kv-c.jpg"),
      recaptchaLoaded: false,
    };
  },
  mounted() {
    this.loadRecaptcha();
  },
  methods: {
    loadRecaptcha() {
      if (this.recaptchaLoaded) return;

      const script = document.createElement('script');
      script.src = 'https://www.google.com/recaptcha/api.js?render=explicit';
      script.async = true;
      script.defer = true;
      
      script.onload = () => {
        this.recaptchaLoaded = true;
        window.grecaptcha.ready(() => {
          window.grecaptcha.render(this.$refs.recaptcha, {
            sitekey: '6LcYOpcpAAAAAMC1A8zOPk87AlW7b5YWDGfbLUkj',
          });
        });
      };

      document.head.appendChild(script);
    },
    async submitForm() {
      // Get the reCAPTCHA response
      const recaptchaResponse = await new Promise(resolve => {
        window.grecaptcha.ready(() => {
          resolve(window.grecaptcha.getResponse());
        });
      });

      // Here you would typically send the form data along with the recaptchaResponse to your server
      console.log('Form submitted with reCAPTCHA response:', recaptchaResponse);

      // Your form submission logic here
      // You might want to use axios or fetch to send a POST request to your server
    },
  },
};
</script>
