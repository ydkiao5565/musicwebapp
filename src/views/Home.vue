<template>
  <div class="home">
    <div id="d1"></div>
    <svg class="icon" aria-hidden="true">
        <use xlink:href="#icon-31liebiao"></use>
    </svg>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style>
#d1{
  width: 3.75rem;
  height: 3.75rem;
  background-color: lightpink;
}
</style>
