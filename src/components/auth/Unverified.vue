<template>
  <div id="app">
    <b-navbar class="p-4" toggleable="lg" type="light" variant="info" sticky >
      <b-container>

        <b-navbar-brand to="/"><img src="../../assets/Subtract.png" width="30" height="30" class="d-inline-block" alt="LogoFroster">
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
            <b-nav-item to="/" class="pr-3">Home</b-nav-item>
            <b-nav-item href="/products" class="pr-3">Products</b-nav-item>
            <b-nav-item href="/" class="pr-3">About Us</b-nav-item>
            <b-button class="my-3 my-sm-0 px-3 font-weight-bold border-0" href="/login" style="background-color: #151D65;">Login</b-button>
          </b-navbar-nav>
        </b-collapse>

      </b-container>
    </b-navbar>

    <b-container>
      <div id="unverified">
        <b-card class="border-0 shadow-lg p-0 rounded" img-left img-src="../../assets/signupIllustration.png" img-width="50%" alt="illustration-signin">
          <div id="verification" style="padding-top: 40%;">
            <h1 class="px-5 text-danger"><b>Ooopss...</b></h1>
            <p class="pt-3 px-5">Your account is not verified yet. Please verify your email
              by click on a link in your email.</p>
            <p class="pt-1 px-5">Doesn't receive an email? <a href="" style="text-decoration: none">Resend</a> </p>
          </div>

        </b-card>
      </div>
    </b-container>

    <div id="footer" class="pt-5">
      <footer class="footer static p-4 text-white" style="background-color: #151d65;">
        <b-container>
          <img src="../../assets/logo-reversed.png" width="30" height="30" class="d-inline-block align-middle" alt="logo-froster">
          <span class="d-inline-block align-middle pl-3"><b>Froster.</b></span>
          <div id="socmed" class="d-inline-block float-right" >
            <a href="https://www.facebook.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../../assets/fb.png" height="16"></a>
            <a href="https://www.instagram.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../../assets/ig.png" height="16"></a>
            <a href="https://www.twitter.com/" class="align-middle pr-3" style="text-decoration: none; color: white;"><img src="../../assets/tw.png" height="16"></a>
          </div>
        </b-container>
      </footer>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Unverified"
  }
</script>

<style scoped>
  .bg-info {
    background-color: #f2f5f7 !important;
  }
  #unverified{
    padding-top: 7%;
    padding-bottom: 7%;
  }
  .rounded{
    border-radius: 1rem !important;
  }
  .card-img-left {
    border-top-right-radius: 0 !important;
    border-top-left-radius: 1rem !important;
    border-bottom-right-radius: 0 !important;
    border-bottom-left-radius: 1rem !important;
  }
</style>