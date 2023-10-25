<script setup>
import navbar from '../components/Header.vue';
import copyright from '../components/Footer.vue';
</script>

<template>
  <navbar />
  <!-- Hero section with background image, heading, subheading and button -->
  <div
    class="relative overflow-hidden bg-cover bg-no-repeat"
    style="
      background-position: 50%;
      background-image: url('https://img.freepik.com/premium-photo/dark-new-retro-cyberpunk-background-with-mountains_1053-9231.jpg');
      height: 600px;
    "
  >
    <div
      class="absolute bottom-0 left-0 right-0 top-0 h-full w-full overflow-hidden bg-fixed"
      style="background-color: rgba(58, 58, 58, 0.75)"
    >
      <div class="flex h-full items-center justify-center">
        <div class="px-6 text-center text-white md:px-12">
          <h1 class="mb-6 text-5xl font-bold">Ini Halaman Home</h1>
          <!-- <h2 class="mb-6 text-5xl font-bold">Heading</h2>
          <h3 class="mb-8 text-3xl font-bold">Subeading</h3> -->
        </div>
      </div>
    </div>
  </div>

  <!-- <br />
  <br />
  <br />
  <br />
  <br /> -->
  <!-- <br />
  <br /><br />
  <br /> -->
  <!-- <br /> -->
  <!-- <br />
  <br />
  <br />
  <br /><br />
  <br />
  <br />
  <br />
  <br />
  <br /> -->
  <copyright />
</template>