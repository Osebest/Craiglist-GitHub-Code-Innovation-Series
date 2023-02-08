<script setup>
import { ref } from 'vue'
import logo from '../assets/logos/logo.png'
import CountryList from './CountryList.vue'
import LanguageList from './LanguageList.vue'

const { onClick } = defineProps({
  onClick: {
    type: Function,
    required: true
  }
})

const drawer = ref(null)

</script>

<template>
  <v-navigation-drawer v-model="drawer" temporary class="pt-4">
    <v-list-item prepend-avatar="https://randomuser.me/api/portraits/men/78.jpg" title="John Leider"></v-list-item>

    <v-divider></v-divider>

    <v-list density="compact" nav class="pt-8 flex flex-col items-center gap-4">
      <CountryList />
      <LanguageList />
      <button class="rounded-full bg-[#3E96ED] mx-2 py-2 px-4 text-white hover:bg-[#77befb] transition-colors">
        Create a Posting
      </button>
      <button
        class="rounded-full border-2 border-[#3E96ED] mx-2 py-2 px-8 text-[#3E96ED] transition-colors hover:bg-[#77befb] hover:text-white hover:border-[#77befb]">
        Login
      </button>
      <v-btn :prepend-icon="theme === 'light' ? 'mdi-weather-sunny' : 'mdi-weather-night'" @click="onClick"></v-btn>
    </v-list>
  </v-navigation-drawer>
  <v-app-bar rounded elevation=4 class="px-4 py-3 px-md-10">
    <v-app-bar-title>
      <v-img :src="logo" contain class="logo"></v-img>
    </v-app-bar-title>
    <v-spacer></v-spacer>
    <template v-slot:append>
      <div class="hidden  lg:flex justify-between items-center">
        <CountryList />
        <LanguageList />
        <button class="rounded-full bg-[#3E96ED] mx-2 py-2 px-4 text-white hover:bg-[#77befb] transition-colors">
          Create a Posting
        </button>
        <button
          class="rounded-full border-2 border-[#3E96ED] mx-2 py-2 px-8 text-[#3E96ED] transition-colors hover:bg-[#77befb] hover:text-white hover:border-[#77befb]">
          Login
        </button>
        <v-btn :prepend-icon="theme === 'light' ? 'mdi-weather-sunny' : 'mdi-weather-night'" @click="onClick"></v-btn>
      </div>
      <button @click.stop="drawer = !drawer" class="lg:hidden">
        <v-icon icon="mdi-menu"></v-icon>
      </button>
    </template>
  </v-app-bar>
</template>

<style scoped>
button {
  border-style: solid;
}

.logo {
  max-width: 180px;
  max-height: 180px;
  min-width: 120px;
  min-height: 120px;
  margin-right: 5rem;
}
</style>