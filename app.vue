<script setup>

import { useBaseUrl } from '~/composables/useBaseUrl';
const baseUrl = useBaseUrl();

useHead({
  title: 'Praca dla kierowcy Wrocław w InfinitiUp',
  meta: [
    { name: 'description', content: 'Zostań kierowcą taxi we Wrocławiu i zarabiaj razem z nami w InfinitiUp' }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [ { innerHTML: '' } ]
})

</script>

<template>
  <div class="main-container">
    <ClientOnly>
      <!-- Adres mojego API z ENV: {{ baseUrl }} -->
      <div>
      </div>
    </ClientOnly>

     <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style lang="scss">
body{
  background-color: $background;
  font-family: 'FarAwayGalaxy', sans-serif;
  margin:0 auto;
  display:flex;
}
.logo-container {
  display: flex;
  justify-content: center; // Wyśrodkowanie w poziomie
  align-items: center; // Wyśrodkowanie w pionie
}
.main-container {
  display: flex;
  flex-direction: column; // Elementy ułożone pionowo
  justify-content: center; // Wyśrodkowanie w pionie
  align-items: center; // Wyśrodkowanie w poziomie
  height: 100%;
  width: 100vw;
}
</style>
