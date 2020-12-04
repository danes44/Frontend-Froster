<template>

  <div id="app">
    <b-navbar class="p-4" toggleable="lg" type="light" variant="info" sticky >
      <b-container>

        <b-navbar-brand href="#"><img src="../assets/Subtract.png" width="30" height="30" class="d-inline-block" alt="LogoFroster">
          <b class="pl-3">Froster.</b>
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse" class="border-0">
          <template #default="{ expanded }">
            <b-icon v-if="expanded" icon="x" style="color: #151D65; width:30px; height: 30px;"></b-icon>
            <b-icon v-else icon="list" style="color: #151D65; width:30px;  height: 30px;"></b-icon>
          </template>
        </b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto text-sm-center font-weight-bold">
            <b-nav-item to="/" class="pr-3" active>Home</b-nav-item>
            <b-nav-item href="/products" class="pr-3">Products</b-nav-item>
            <b-nav-item href="#aboutus" class="pr-3">About Us</b-nav-item>
            <b-button class="my-3 my-sm-0 px-3 font-weight-bold border-0" to="/login" style="background-color: #151D65;">Login</b-button>
          </b-navbar-nav>
        </b-collapse>

      </b-container>
    </b-navbar>

    <div id="title" >
      <b-container>
        <b-row align-v="center">
          <b-col lg="6" md="6">
            <h1 style="font-weight: 900; font-size: 3.3rem;" >Choose Better <br> Live Better.</h1>
            <h6>“One of the very nicest things about life is the way we must regularly stop whatever
              it is we are doing and devote our attention to eating.”</h6>
          </b-col>
          <b-col lg="6" md="6">
            <img class="title-img" src="../assets/Illustration.svg" alt="illustration-img" >
          </b-col>
        </b-row>
      </b-container>
    </div>

    <div id="aboutus">
      <b-container>
        <b-row class="justify-content-md-center" style="padding-top: 15%;">
          <h1 align="center" class="pb-5 font-weight-bolder"> Why You Have to Choose Us?</h1>
        </b-row>

        <b-row>
          <b-col lg="1">
            <img src="../assets/dollar icon.png" width="75">
          </b-col>
          <b-col class="pt-4">
            <h4><b>Money Back Guarantee</b></h4>
            <p> Money Back Guarantee applies to virtually everything on our site, and
              there's no extra fee for coverage. It’s automatic and covers your purchase price plus
              original shipping on eligible purchases.
            </p>
          </b-col>
          <b-col lg="1">
            <img src="../assets/packaging icon.png" width="75">
          </b-col>
          <b-col class="pt-4">
            <h4> <b>Good Packaging</b> </h4>
            <p> We package your frozen food with Thermal Pouch which is
              made from Reinforced Insulation Foil and a heavy duty
              air baffle. Packaging with 3 convenient and practical sizes in flat packed
              kit form.
            </p>
          </b-col>
        </b-row>

        <b-row>
          <b-col lg="1">
            <img src="../assets/delivery icon.png" width="75">
          </b-col>
          <b-col class="pt-4">
            <h4> <b>Fast Delivery</b> </h4>
            <p> "That's what we're here for!  Give us a call and let us do the hard work for you!"
              We have a fantastic range of fast delivery promotional items that can be printed and
              delivered within 7 days... some in just 24 hours!
            </p>
          </b-col>
          <b-col lg="1">
            <img src="../assets/discount icon.png" width="75">
          </b-col>
          <b-col class="pt-4">
            <h4> <b>Discount</b> </h4>
            <p> Skip the lines and the stress with our delicious frozen food.
              That way you have more time to enjoy the day!.
              Froster sends your frozen food straight to your door.
              Plus sometimes we're offering special discount for you!.
            </p>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <div id="packaging">
      <b-container>
        <h1 style="text-align: center; font-weight: bold; padding-top: 15%"> Our Packaging</h1>
        <p style="text-align: center; font-size: 1.2rem">We collaborate with
          <a href="https://upac.com.au/">upac.com.au</a>
          <br>
          to keep your frozen food still frozen until you receive it
        </p>
        <b-row class="pt-5 no-gutters">
          <b-col lg="5" class="px-0 px-sm-3 pb-3">
            <b-img-lazy  src="../assets/foil-feat-3.jpg" style="border-radius: 1rem!important; width: 90%"></b-img-lazy>
          </b-col>
          <b-col class="align-middle">
            <b-row class="pb-3 no-gutters">
              <b-col cols="3">
                <b-img-lazy  src="../assets/foil-feat-2.jpg" style="border-radius: 1rem!important; width: 70%"></b-img-lazy>
              </b-col>
              <b-col>
                <h3><b>Heavy Duty</b></h3>
                <p class="mb-0">We package your frozen food with Thermal Pouch which is
                  made from Reinforced Insulation Foil and a heavy duty
                  air baffle</p>
              </b-col>
            </b-row>

            <b-row class="pb-3 no-gutters">
              <b-col cols="3">
                <b-img-lazy  src="../assets/foil-feat-4.jpg" style="border-radius: 1rem!important; width: 70%"></b-img-lazy>
              </b-col>
              <b-col>
                <h3><b>Practical Sizes</b></h3>
                <p>Packaging with 3 convenient and practical sizes in flat packed
                  kit form.</p>
              </b-col>
            </b-row>

            <b-row class="pb-3 no-gutters">
              <b-col cols="3">
                <b-img-lazy  src="../assets/foil-feat-1.jpg" style="border-radius: 1rem!important; width: 70%"></b-img-lazy>
              </b-col>
              <b-col>
                <h3><b>Lightweight Pouches</b></h3>
                <p>We use lightweight pouches so that your frozen food doesn’t
                  damaged by the load when we are delivering your frozen food </p>
              </b-col>
            </b-row>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <div id="ourstore">
      <b-img id="background-img" src="../assets/background.png"
           style="width: 100%;
           opacity: 0.12;
           position: absolute;
           bottom:0;
           z-index: -1;"
      ></b-img>
      <b-container>
        <div>
          <h1 style="text-align: center; font-weight: bold; padding-top: 15%">Our Store</h1>
          <b-row class="pt-5">
            <b-col sm md class="pr-5">
              <b-row class="justify-content-end">
                <img src="../assets/Subtract.png" style="width: 14%;">
              </b-row>
              <b-row class="justify-content-end">
                <h5><b>Froster.</b></h5>
              </b-row>
              <b-row class="justify-content-end pt-3">
                <h5><b>Address</b></h5>
                <p class="text-right">Ruko Sagan Square, Jl. Prof. Herman Yohanes No.26,
                  Terban, Kec. Gondokusuman, Kota Yogyakarta,
                  Daerah Istimewa Yogyakarta 55223</p>
              </b-row>
              <b-row class="justify-content-end pt-3">
                <h5><b>Telephone Number</b></h5>
                <div class="w-100"></div>
                <p class="text-right">0274-546789</p>
              </b-row>
              <b-row class="justify-content-end pt-3">
                <h5><b>Email</b></h5>
                <div class="w-100"></div>
                <p class="text-right">admin@froster.tugasbesar.com</p>
              </b-row>
            </b-col>

            <b-col sm md class="pt-3 pt-lg-0 mx-3 mx-lg-0">
              <div style="width: 100%" class="embed-responsive embed-responsive-4by3" >
                <iframe class="rounded embed-responsive-item" width="100%" height="100%" frameborder="0"
                        scrolling="no" marginheight="0" marginwidth="0"
                        src="https://maps.google.com/maps?width=100%25&amp;height=600&amp;hl=en&amp;q=7%C2%B046'53.5%22S%20110%C2%B022'45.2%22E+(Froster%20Store)&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"></iframe>
              </div>
            </b-col>
          </b-row>
        </div>
      </b-container>
    </div>

    <div id="footer" class="pt-5">
      <footer class="footer static p-4 text-white" style="background-color: #151d65;">
        <b-container>
          <img src="../assets/logo-reversed.png" width="30" height="30" class="d-inline-block align-middle" alt="logo-froster">
          <span class="d-inline-block align-middle pl-3"><b>Froster.</b></span>
          <div id="socmed" class="d-inline-block float-right" >
            <a href="https://www.facebook.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../assets/fb.png" height="16"></a>
            <a href="https://www.instagram.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../assets/ig.png" height="16"></a>
            <a href="https://www.twitter.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../assets/tw.png" height="16"></a>
          </div>
        </b-container>
      </footer>
    </div>


  </div>


</template>

<script>
  export default {
    data() {
      return {
        fields: ['first_name', 'last_name', 'age'],
        busy:true,
        items: [
          { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { age: 89, first_name: 'Geneva', last_name: 'Wilson' }
        ]
      }
    }
  }
</script>

<style>
  .bg-info {
    background-color: #f2f5f7 !important;
  }
</style>