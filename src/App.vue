<script setup>
import Stat from "./components/Stat.vue";
import CitySelect from "./components/CitySelect.vue"
const data = {
  label: "Влфжность",
  stat: "90%",
}

function getCity(city) {
  console.log(city)
}
</script>

<template>
  <main class="main">
    <Stat v-bind="data">
    </Stat>
    <Stat label="Влажность" stat="90%">
    </Stat>
    <CitySelect @select-city="getCity"></CitySelect>
  </main>
</template>

<style scoped>
  .main {
    background: var(--color-bg-main);
    padding: 60px 50px;
    border-radius: 25px;
  }
</style>
