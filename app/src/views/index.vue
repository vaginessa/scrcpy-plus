<template>
  <div class="home">
    <welcome />
    <device />
    <scrcpy />
  </div>
</template>

<style>
section {
  text-align: center;
  margin-top: 2em;
}
.center {
  display: flex;
  justify-content: center;
}
</style>

<script>
import welcome from '@/components/welcome.vue';
import device from '@/components/device.vue';
import scrcpy from '@/components/scrcpy.vue';

export default {
  name: 'HomeView',
  components: { welcome, device, scrcpy }
}
</script>