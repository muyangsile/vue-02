<template lang="">
  <div>
    父组件:来自于子组件的数据：{{message}}
    <SonCompnent :cjb="cjb" v-on:suibian="receiveMessage"></SonCompnent>
  </div>
</template>
<script>
import SonCompnent from './components/SonCompnent.vue';
export default {
  provide:{
    sj:"朱自清的《背影》"
  },
  data(){
    return{
      message:"",
      cjb:"亮晶晶的传家宝"
    }
  },
  components:{
    SonCompnent
  },
  methods:{
    receiveMessage(data){
      console.log(data)
      this.message=data
    }
  }
}
</script>
<style lang="">
  
</style>