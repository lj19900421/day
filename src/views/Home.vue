<template>
  <div class="home">
    <Swiper/>
    <div class="dl">
      <dl v-for="(item ,index) in list" :key="index">
        <dt><img :src="item.img" alt=""></dt>
        <dd>{{item.content}}</dd>
      </dl>
    </div>
    <p>金牌商家</p>
  </div>
</template>

<script>
import Swiper from '@/components/Swiper.vue'

export default {
  name: 'home',
  data() {
    return {
      list: [{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      },{
        'img': 'https://dummyimage.com/(30x30)',
        'content': '成单奖励'
      }]
    }
  },
  components: {
    Swiper
  }
}
</script>
<style lang="scss">
  .dl{
    width: 100%;
    height: 120px;
    display: flex;
    flex-wrap: wrap;
    dl{
      width: 25%;
      height: 50%;
      text-align: center;
    }
  }
</style>
