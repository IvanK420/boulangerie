<script setup>

import Navbar from "@/components/Navbar.vue";
import Banner from "@/components/Banner.vue";
import Card from "@/components/Card.vue";
let gateaux = [
    "Tropezienne", "Gateau patate", "Gateau tisson" , "foret noire", "gateau massepin"
]
</script>

<template>
  <header>
    <Navbar/>
  </header>
  <main>
    <div class="container h-10">
    <Banner/>
    </div>
    <div class="container mt-4">
      <div class="row">
        <div v-for="gateau in gateaux" :key="gateau" class="col-md-6 mb-4">
          <card :cardTitle="gateau"/>
        </div>
      </div>
    </div>
  </main>
  <footer>

  </footer>
</template>

<style scoped>

</style>
