<template>
  <div>
    <Minimo v-if="true" />
    <CardDivider v-if="true" class="mx-auto" />
    <below-divider v-if="true" />
    <Footer v-if="true" />
    
  </div>
</template>

<script>
import Minimo from "./components/Minimo";
import CardDivider from "./components/CardDivider";
import BelowDivider from "./components/BelowDivider.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    Minimo,
    CardDivider,
    BelowDivider,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>
<style>

</style>
