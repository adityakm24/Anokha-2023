<script setup>

</script>

<template>
  <div class="sponsor">
    <h1 data-aos="fade-right">Sponsors</h1>

    <div data-aos="zoom-in">

      <div class="responsive">
        <img src="https://1000logos.net/wp-content/uploads/2021/05/Coca-Cola-logo-768x432.png" alt="CocaCola"
          width="600" height="300">
      </div>



      <div class="responsive">
        <img
          src="https://cdn.cookielaw.org/logos/67f35096-f18a-45a1-84a2-a83e00bd9540/2daa8fb4-3fd2-41bc-94b8-fe6ad3972f18/2d433c6f-80fd-4564-95cc-4a5bc829c0c3/AIRBUS_Blue.png"
          alt="Airbus" width="600" height="400">
      </div>

      <div class="responsive">
        <img
          src="https://upload.wikimedia.org/wikipedia/en/thumb/5/58/State_Bank_of_India_logo.svg/2560px-State_Bank_of_India_logo.svg.png"
          alt="SBI" width="600" height="400">
      </div>

      <div class="responsive">
        <img src="https://www.pngkey.com/png/detail/676-6762434_cognizant-logo-png.png" alt="SBI" width="600"
          height="400">
      </div>

      <div class="clearfix"></div>


    </div>

  </div>
</template>

<style scoped>
.sponsor {
  padding-top: 5%;
  background: radial-gradient(circle at 24.1% 68.8%, rgb(32, 32, 32) 0%, rgb(0, 0, 0) 99.4%);
  text-align: center;

}

.sponsor h1 {
  -webkit-text-stroke: 2px white;
  color: rgba(0, 0, 0, 0);
  font-weight: 800;
  font-size: 5rem;

}

.sponsor img {
  width: 100%;
  height: auto;
  padding: 20px;
}


.responsive {
  padding: 0 6px;
  float: left;
  width: 24.99999%;
}

@media only screen and (max-width: 912px) {

  .sponsor h1 {
    -webkit-text-stroke: 2px white;
    color: rgba(0, 0, 0, 0);
    font-size: 70px;
  }

}

@media only screen and (max-width: 700px) {
  .responsive {
    width: 49.99999%;
    margin: 6px 0;
  }
}

@media only screen and (max-width: 500px) {
  .responsive {
    width: 100%;
  }
}

.clearfix:after {
  content: "";
  display: table;
  clear: both;
}
</style>
