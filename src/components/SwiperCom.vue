<template>
  <div class="swiper-container">
    <div class="swiper-wrapper">
        <div class="swiper-slide" v-for="(img,i) in imgs" :key="i"><img :src="img"></div>
    </div>
    <!-- 如果需要分页器 -->
    <div class="swiper-pagination"></div>
  </div>
</template>

<script>
import Swiper from 'swiper';   
import 'swiper/css/swiper.css'
export default {
  data() {
    return {
      imgs:[
        require('../assets/img/swiper1.png'),
        require('../assets/img/swiper2.jpg'),
        require('../assets/img/swiper3.png')
      ]
    }
  },
  mounted() {
    var mySwiper = new Swiper('.swiper-container', {
    loop: true, // 循环模式选项
    
    // 如果需要分页器
    pagination: {
      el: '.swiper-pagination',
      clickable:true
    },
    
    // 如果需要前进后退按钮
    navigation: {
      nextEl: '.swiper-button-next',
      prevEl: '.swiper-button-prev',
    },
    
    // 如果需要滚动条
    scrollbar: {
      el: '.swiper-scrollbar',
    },
  })
  }
}
</script>

<style>
.swiper-container {
  width: 7.1rem;
  height: 3rem;
}

.swiper-slide img{
  width: 100%;
  height: 100%;
  border-radius: 0.2rem;
}
.swiper-pagination-bullet-active {
  background-color: orangered;
}
</style>