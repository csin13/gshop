<template>
  <footer class="footer_guide">
    <a
      href="javascript:;"
      class="guide_item"
      :class="{ on: '/msite' === $route.path }"
      @click="goTo('/msite')"
    >
      <span><i class="iconfont icon-waimai"></i><span> </span>外卖</span>
    </a>
    <a
      href="javascript:;"
      class="guide_item"
      :class="{ on: '/search' === $route.path }"
      @click="goTo('/search')"
    >
      <span> <i class="iconfont icon-sousuo"></i><span></span>搜索</span></a
    ><a
      href="javascript:;"
      class="guide_item"
      :class="{ on: '/order' === $route.path }"
      @click="goTo('/order')"
      ><span><i class="iconfont icon-dingdan"></i><span></span>订单</span></a
    ><a
      href="javascript:;"
      class="guide_item"
      :class="{ on: '/profile' === $route.path }"
      @click="goTo('/profile')"
      ><span><i class="iconfont icon-wode"></i><span></span>我的</span></a
    >
  </footer>
</template>

<script>
export default {
  data() {
    return {};
  },

  components: {},

  computed: {},

  methods: {
    goTo(path) {
      this.$router.replace(path);
    },
  },
};
</script>
<style lang='less' scoped>
.footer_guide {
  position: fixed;
  display: flex;
  align-items: center;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 50px;
  background-color: #f5f5f5;
  .guide_item {
    flex: 1;
    display: flex;
    justify-content: center;
    text-decoration: none;
    text-align: center;
    color: #999999;
    span {
      display: block;
      .iconfont {
        font-size: 22px;
      }
    }
  }
  .on {
    color: #6fa6ee;
  }
}
</style>