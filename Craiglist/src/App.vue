<script setup>
import { RouterView } from 'vue-router'
import NavBarVue from './components/NavBar.vue'
import { ref } from 'vue'
import Footer from './components/Footer.vue';



const theme = ref('light')

function onClick() {
  theme.value = theme.value === 'light' ? 'dark' : 'light'
}

</script>


<template>
  <v-app :theme="theme">
    <NavBarVue :onClick="onClick" />

    <v-main>

      <RouterView />

    </v-main>
    <Footer />

  </v-app>
</template>


<style scoped>

</style>
