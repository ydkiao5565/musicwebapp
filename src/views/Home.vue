<template>
  <TopNav></TopNav>
  <SwiperCom></SwiperCom>
</template>

<script>
// @ is an alias to /src
import TopNav from '@/components/TopNav.vue'
import SwiperCom from '@/components/SwiperCom.vue'


export default {
  name: 'Home',
  
  components: {
    TopNav,
    SwiperCom,
  }
}
</script>
