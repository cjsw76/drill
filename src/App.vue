<template>
  <div id="app">
    <FirstChild></FirstChild>
    <SecondChild></SecondChild>
  </div>
</template>

<script>
import SecondChild from './views/SecondChild.vue'
import FirstChild from './views/FirstChild.vue'

export default {
  name: 'App',
  components: {
   FirstChild,
   SecondChild
  }
}
</script>

<style>
@import "./assets/css/base.css";

</style>
