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
    <div class="container">
    <Banner/>
    </div>
    <div class="container mt-4">
      <div class="row">
        <div v-for="gateau in gateaux" :key="gateau" class="col-md-6 mb-4">
          <card :cardTitle="gateau"
                card-text="lorem ispum"
          />
        </div>
      </div>
    </div>
  </main>
  <footer>
  <div class="container text-center mt-4 mb-4 border-top border-dark p-2" style="background-color: #f8f9fa;">
    horaires : 7h-20h du lundi au samedi
  </div>
  </footer>
</template>

<style scoped>

</style>
