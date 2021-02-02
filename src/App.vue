<template>
  <div>
    <Minimo  />
    <CardDivider  class="mx-auto" />
    <below-divider  />
    <Footer  />
    
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
