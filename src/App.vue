<template>
  <HelloWorld msg="뷰 공부 합시다 !"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style lang="scss">
@import "styles/components/header.scss";
@import "styles/reset.scss";
</style>
