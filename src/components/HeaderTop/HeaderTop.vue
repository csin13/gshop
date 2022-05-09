<template>
  <header class="header">
    <slot name="left"></slot>
    <div class="header_title">
      <h2>{{ address }}</h2>
    </div>
    <slot name="right"></slot>
  </header>
</template>

<script>
export default {
  props: {
    address: String,
  },
  data() {
    return {};
  },

  components: {},

  computed: {},

  methods: {},
};
</script>
<style lang="less" scoped></style>
