<template>
  <swiper :options='swiperOption' class="banner">
    <swiperSlide v-for="(item ,index) in list" :key="index">
      <img :src="item" alt="">
    </swiperSlide>
  </swiper>
</template>
<script>
import {swiper,swiperSlide} from 'vue-awesome-swiper'
export default {
  data() {
    return {
      swiperOption: {
        autoplay: true,
        loop: true
      },
      list:['https://dummyimage.com/(300x200)','https://dummyimage.com/(300x200)','https://dummyimage.com/(300x200)']
    }
  },
  components: {
    swiper,
    swiperSlide
  }
}
</script>
<style lang="scss">
  .banner{
    width: 100%;
    height: 200px;
    img{
      width: 100%;
      height: 100%;
    }
  }
</style>