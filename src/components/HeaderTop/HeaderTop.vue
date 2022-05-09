<template>
  <header class="header" :class="{ header_isSlot: isSlot }">
    <slot class="header_left" name="left"></slot>
    <div class="header_title">
      <h2>{{ title }}</h2>
    </div>
    <slot class="header_right" name="right"></slot>
  </header>
</template>

<script>
export default {
  props: {
    title: String,
    isSlot: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {};
  },

  components: {},

  computed: {},

  methods: {},
};
</script>
<style lang="less" scoped>
.header {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 1rem;
  background-color: rgb(74, 157, 235);
  color: #fff;
}
.header_isSlot {
  justify-content: space-between;
  align-items: center;
}
</style>
