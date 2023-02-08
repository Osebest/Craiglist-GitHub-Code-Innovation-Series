<script setup>
import { RouterView } from 'vue-router'
import NavBarVue from './components/NavBar.vue'
import { ref } from 'vue'



const theme = ref('light')

function onClick() {
  theme.value = theme.value === 'light' ? 'dark' : 'light'
}

</script>


<template>
  <v-app :theme="theme">
    <NavBarVue :onClick="onClick"/>

    <v-main>
      <v-container>
        <RouterView />
      </v-container>
    </v-main>
  </v-app>
</template>


<style scoped>

</style>
