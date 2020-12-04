<template>
    <router-view>
    </router-view>
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
  :root {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    overflow-x: hidden;
  }
  body{
    font-family: 'Open Sans', sans-serif;
    font-weight: normal;
    color: #151D65 !important;
    background-color: #f2f5f7 !important;
  }
  .navbar-light .navbar-brand {
    color: #151D65 !important;
  }
  .navbar-light .navbar-nav .nav-link.active{
    color:#151D65 !important
  }
  .btn:hover {
    background-color: #007bff !important;
    text-decoration: none;
  }
  a {
    transition: color 0.3s ease-in-out;
  }
</style>
