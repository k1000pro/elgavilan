<template>
  <q-page class="bg-primary">
    <CaruselImagene> </CaruselImagene>
  </q-page>
</template>

<script>
import CaruselImagene from "src/components/CaruselImagene.vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
  components: { CaruselImagene },
});
</script>
