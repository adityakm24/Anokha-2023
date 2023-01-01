<script setup>

import { onMounted } from "vue";
import AOS from "aos";

onMounted(() => {
    AOS.init();
})

</script>

<template>
  <div class="imgcont">

    <div class="center" id="home">
      <p>Amrita Vishwa Vidyapeetam Presents</p>
      <h1><span style="color:red;">ANOKHA</span> <span class="year"> 2023</span></h1>
      <button class="btn-primary">Register</button>
    </div>
  </div>
</template>


<style type="text/css" scoped>
.btn-primary {
  background-color: red;
  padding: 10px;
  width: 25%;
  border: 0px;
  border-radius: 10px;
  transition: 0.2s;
  font-size: 18px;
}

.btn-primary:hover {
  background-color: rgb(255, 255, 255);
  color: black;
  padding: 10px;
  width: 25%;
  border: 0px;
  border-radius: 10px;
  transition: 0.2s;
  font-size: 18px;
}


.imgcont {
  background-image: url('../assets/images/header.png');
  height: 50%;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  padding: 20%;

}

.year {
  -webkit-text-stroke: 2px white;
  color: rgba(0, 0, 0, 0);
}

.center {
  position: absolute;
  top: 50%;
  left: 50%;
  color: black;
  transform: translate(-50%, -50%);
  text-align: center;
}

.center p {
  font-size: 30px;
  color: white;
}


.center h1 {
  font-weight: bolder;
  font-size: 150px;
}

@media only screen and (max-width: 912px) {
  .imgcont {
    height: 300px;
    background-image: url('../assets/images/header.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
    padding: 50%;

  }

  .imgcont img {
    width: 100%;
    height: 100%;
  }

  .center {
    position: absolute;
    left: 50%;
    color: black;
    transform: translate(-50%, -50%);
  }

  .center p {
    font-size: 20px;
  }


  .center h1 {
    font-weight: bolder;
    font-size: 70px;
  }
}

</style>

