<template>
  <div class="home">
    <information />
    <device />
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
</template>

<style>
section {
  border: 1px solid white;
}
</style>

<script>
import information from '@/components/information.vue';
import device from '@/components/device.vue';

export default {
  name: 'HomeView',
  components: { information, device }
}
</script>