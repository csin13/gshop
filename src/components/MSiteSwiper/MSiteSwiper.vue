<template>
  <swiper class="mSiteSwiper" :options="swiperOptions">
    <swiper-slide>
      <div>
        <ul class="nav">
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>甜品饮品</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>超市便利</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>新店特惠</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>准时达</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>预定早餐</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>宵夜特惠</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>土豪推荐</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>外卖</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>外卖</p>
          </li>
          <li>
            <a href=""><img src="./imgs/jd.png" alt="" /></a>
            <p>外卖</p>
          </li>
        </ul>
      </div>
    </swiper-slide>
    <swiper-slide>Slide 1</swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
export default {
  data() {
    return {
      //swiper配置
      swiperOptions: {
        // autoplay: true,
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
  height: 1rem;
}
.mSiteSwiper {
  height: 3.5rem;
  width: 100%;
  .nav {
    display: flex;
    height: 128px;
    margin: 0;
    padding: 0;
    flex-wrap: wrap;
    justify-content: center;
  }
  li {
    width: 20%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    list-style: none;
  }
  p {
    font-size: 12px;
  }
}
</style>