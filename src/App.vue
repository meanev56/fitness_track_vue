<script setup>
  import Welcome from './components/pages/Welcome.vue';
  import Layout from './components/layouts/Layout.vue';

  import { ref } from 'vue';



  const selectedDisplay = ref(1);


  function handleChangeDisplay(idx) {
    selectedDisplay.value = idx
  }

</script>

<template>
  <Layout>

    <!-- page 1 -->
    <Welcome :handleChangeDisplay="handleChangeDisplay" v-if="selectedDisplay == 1"  />

  </Layout>
  
</template>

<style scoped>

</style>
