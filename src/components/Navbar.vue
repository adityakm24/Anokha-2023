<script type="text/javascript" scoped>
$(window).scroll(function () {
  $('nav').toggleClass('scrolled', $(this).scrollTop() > 75);
});


$(document).ready(function () {
  $('i').click(function () {
    $(this).toggleClass('fa-solid-plus-square fa-minus-square');
  });
});

</script>

<template>

  <nav class="navbar navbar-expand-lg sticky-top bg-clr">
    <a class="navbar-brand mr-auto" href="#">Logo Here</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span>
        <i class="fa-solid fa-bars" style="color:#fff; font-size:28px;"></i>
      </span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <div class="navbar-nav  ml-auto">
        <a href="/#home" class="nav-item nav-link">Home</a>
        <a href="/#about" class="nav-link">About</a>
        <a href="/#gallery" class="nav-link">Gallery</a>
        <a href="/Contact" class="nav-link">Contact</a>
        <button class="rgstr">Register</button>
      </div>
    </div>
  </nav>
  <router-view />
</template>


<style scoped>

.rgstr {
  border-radius: 10px;
  font-size: 15px;
  padding-left: 10px;
  padding-right: 10px;
}

.bg-clr {
  background: rgb(0, 0, 0) !important;
  transition: 0.1s ease-in;
}

.bg-clr.scrolled {
  background: rgba(0, 0, 0, 0.686) !important;
  -webkit-backdrop-filter: blur(10px);
  backdrop-filter: blur(10px);
}

.navbar {
  margin: auto;
  padding: 20px;
  text-align: center;
}

.navbar a {
  font-weight: light;
  color: #ababab;
  text-align: center;
  transition: 0.2s ease-in;
  padding-right: 10px;
}


.navbar a:hover {
  color: rgb(255, 255, 255);
}

.navbar a.router-link-exact-active {
  color: rgb(47, 0, 255);
  border-radius: .5rem;
  text-decoration: underline;
}

.navbar-toggler-icon {
  color: #fff;
}
</style>
