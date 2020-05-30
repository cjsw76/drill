<template>
  <div class="">
    <p>{{ mes }}</p>
    <button @click="clickEvent">点击更新数据</button>
  </div>
</template>

<script>
import bus from 'assets/eventBus.js'
export default {
  name: 'FirstChild',
  data(){
    return{
      mes: '我是firstChild组件'
    }
  },
  methods:{
    clickEvent(){
      bus.$emit('userDefineEvent',this.mes)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
