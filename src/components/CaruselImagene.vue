<template class="bg-dark">
  <div class="" style="height: 200%">
    <q-carousel arrows animated v-model="slide">
      <q-carousel-slide
        name="first"
        img-src="https://dsm01pap001files.storage.live.com/y4mYGTRS-_FQtWfzuUrUhKyKPwu5RZlvQOELLriye6YNwvbch5AKm9P2ODAN9CDiovKWWVna9p-LqUF-tyD57UHUuy23_xFByqWsv6TsVS--5iBAcImyi_JtURTfh9uCJ3TQOg4ws4eOmNzfC5LhobXUYnClERFzcUui5mrwcKO5K5t8sC0LMIupS75g19UEAVYbXmIDWnFO5BpwsHHn9-Nng?encodeFailures=1&width=1507&height=848"
      >
        <div class="absolute-bottom custom-caption">
          <div class="text-h2">First stop</div>
          <div class="text-subtitle1">Mountains</div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        name="second"
        img-src="https://dsm01pap001files.storage.live.com/y4mp-NS1-aDtzp5SPZ4-3Ja5H7ByXW_HJFDt9r6Jyv413L991sQr2XfWF8fYZUCLIFVpB4Pm9iYEZQ0eESYbv-hB4yLuFwJROn6EcofF8u_TLGLduY5kYsKu_kmUM5npPUhSfNx5XlXECMzejnElduDsE5_Q4hjgV4h5_s0lCClpAva2ihCqi9t8CrIOWpR-G8c3lbcNcA-Ua8m7J8AOyTKsg?encodeFailures=1&width=1507&height=848"
      >
        <div class="absolute-bottom custom-caption">
          <div class="text-h2">Second stop</div>
          <div class="text-subtitle1">Famous City</div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        name="third"
        img-src="https://dsm01pap001files.storage.live.com/y4mG3nZn-HvI6MRTz4HBljz3BryK3PhARVAKhB2SHYSmb7DLk3Y1y14y0_Tfbkzc3G0d353IV9z0UbfdyprP6aC8vNEEp3Jhg1GR2l2evoO7PVSwWEgyadDW5juMEpasbZgsChjJTp04nKj1iwt77TWHMLSE6xFDPlmFRy5xMlnjpAPXSPXWqpYTnascldYawey0npjxdid8l13wbU6OE44lA?encodeFailures=1&width=1507&height=848"
      >
        <div class="absolute-bottom custom-caption">
          <div class="text-h2">Third stop</div>
          <div class="text-subtitle1">Famous Bridge</div>
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      slide: ref("first"),
    };
  },
};
</script>

<style lang="sass" scoped>
.custom-caption
  text-align: center
  padding: 12px
  color: white
  background-color: rgba(0, 0, 0, .3)
</style>
