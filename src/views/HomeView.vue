<script setup>
import TheWelcome from './TheWelcome.vue'
import AboutView from './AboutView.vue';
import SponsorView from './SponsorView.vue';
import CounterView from './CounterView.vue';
import Navbar from '../components/Navbar.vue';
import GalleryView from './GalleryView.vue';
import Footer from "../components/Footer.vue";
</script>

<template>
  <main>
  <Navbar />
<TheWelcome />
<CounterView />
<AboutView />
<SponsorView />
<GalleryView /> 

<Footer />


  </main>
</template>



