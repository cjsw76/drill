<template>
  <div class="">
    <p>{{ mes }}</p>
  </div>
</template>

<script>
import bus from 'assets/eventBus.js'
export default {
  name: 'SecondChild',
  data(){
    return{
      mes: 'secondChild中默认的值mes'
    }
  },
  methods:{
    
  },
  mounted(){
      let that = this;
      bus.$on('userDefineEvent',res=>{
        that.mes = res
      })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
