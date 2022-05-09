<template>
  <swiper class="mSiteSwiper" :options="swiperOptions">
    <swiper-slide
      ><img src="../../../static/imgs/test.jpg" alt=""
    /></swiper-slide>
    <swiper-slide>Slide 1</swiper-slide>
    <swiper-slide>Slide 2</swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
export default {
  data() {
    return {
      //swiper配置
      swiperOptions: {
        autoplay: true,
        pagination: {
          el: ".swiper-pagination",
        },
      },
    };
  },

  components: {},

  computed: {},

  methods: {},
};
</script>
<style lang='less' scoped>
img {
  width: 2rem;
  height: 2rem;
}
.mSiteSwiper {
  height: 3rem;
  width: 100%;
}
</style>