<script setup>
import { ref } from 'vue'

const cities = ref(['Atlanta', 'Boston', 'Charlotte', 'Chicago', 'Cleveland', 'Dallas', 'Denver', 'Detroit', 'Golden State', 'Houston', 'Indianapolis', 'Houston', 'Los Angeles', 'Miami', 'Milwaukee', 'Minneapolis', 'New York', 'San Francisco', 'Seattle', 'Tampa', 'Washington', 'Wilmington'])

console.log(cities)

</script>

<template>
  <div class="cov">
    <v-container>
      <div class="flex px-2 mb-6">
        <h1 class="text-2xl font-semibold">Nearby Cities</h1>
        <v-spacer></v-spacer>
        <p class="text-[#3E96ED] underline decoration-[#3E96ED] cursor-pointer">see more</p>
      </div>
      <v-slide-group show-arrows>
        <v-slide-group-item v-for="city in cities" :key="city" v-slot="{ isSelected, toggle }">
          <button @click="toggle" :class="{ 'bg-blue-400 text-white': isSelected }"
            class="rounded-full mx-2 py-2 px-8 text-[#3E96ED] bg-[#d2e8fb] transition-colors hover:bg-[#6fb9fa] hover:text-white">
            {{ city }}
          </button>
        </v-slide-group-item>
      </v-slide-group>
    </v-container>
  </div>
</template>

<style scoped>
.cov {
  background-color: rgba(0, 0, 0, 0.1);
  padding-bottom: 20px;
}
</style>