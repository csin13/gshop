<template>
  <div>
    <HeaderTop :title="address" isSlot>
      <div class="header_search" slot="left">
        <span><i class="iconfont icon-sousuo"></i></span>
      </div>
      <div class="header_login" slot="right">
        <span><a href="">登陆</a></span>
      </div>
    </HeaderTop>
    <!-- 轮播图 -->
    <MSiteSwiper />
  </div>
</template>

<script>
import HeaderTop from "../../components/HeaderTop/HeaderTop.vue";
import MSiteSwiper from "./MSiteSwiper.vue";
export default {
  data() {
    return {
      address: "昌平区北七家洪福科技园",
    };
  },

  components: {
    HeaderTop,
    MSiteSwiper,
  },

  computed: {},

  methods: {},
};
</script>
<style lang='less' scoped>
.header_search {
  margin-left: 10px;
}
.header_login {
  margin-right: 10px;
  a {
    color: #fff;
  }
}
</style>