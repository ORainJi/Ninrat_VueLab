<template>
  <div class="container">
    <Manufacturer v-slot="data">
      <Devices :manufacturerId="data.factId"></Devices>
    </Manufacturer>
  </div>
</template>

<script>
import Manufacturer from "@/components/Manufacturer.vue";
import Devices from "@/components/Devices.vue";
export default {
  components: {
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>

<style scoped>
</style>