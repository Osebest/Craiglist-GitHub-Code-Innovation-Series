<script setup>
import hero from "../assets/Union.png";

</script>

<template>
  <v-parallax
    :src="hero"
    class="cov"
    height="600"
  >
    <div class="flex flex-column fill-height justify-center align-center text-white">
      <h1 class="text-5xl font-semibold mb-8 text-center">
        The One <span class="text-[#3E96ED]">Top List</span> for all your <span class="text-[#3E96ED]">needs</span>
      </h1>
      <h4 class="subheading">
       Market with us today!
      </h4>
    </div>
  </v-parallax>
</template>


<style scoped>
.cov{
  background: rgba(0, 0, 0, 0.8);
}
</style>