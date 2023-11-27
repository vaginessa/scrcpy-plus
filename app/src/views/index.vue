<template>
  <div class="home">
    <information />
    <device />
    <scrcpy />
  </div>
</template>

<style>
section {
  border: 1px solid white;
  text-align: center;
}
</style>

<script>
import information from '@/components/information.vue';
import device from '@/components/device.vue';
import scrcpy from '@/components/scrcpy.vue';

export default {
  name: 'HomeView',
  components: { information, device, scrcpy }
}
</script>