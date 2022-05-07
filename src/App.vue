<template>
  <div>
    <router-view></router-view>
    <FooterGuide />
  </div>
</template>

<script>
import FooterGuide from "../src/components/FooterGuide/FooterGuide.vue";
export default {
  data() {
    return {};
  },

  components: {
    FooterGuide,
  },

  computed: {},

  methods: {},
};
</script>
<style lang='less' scoped>
</style>