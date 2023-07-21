<template lang="">
  <div>
    <Headcomponent posttitle="hello"></Headcomponent>
    <bannerComponent></bannerComponent>
    <ClassifyComponent :menuList="menuList"></ClassifyComponent>
    <LiveListComponent></LiveListComponent>
    <BarComponent></BarComponent>
  </div>
</template>
<script>
import Headcomponent from './components/Headcomponent.vue';
import bannerComponent from '@/components/BannerComponent.vue';
import ClassifyComponent from './components/ClassifyComponent.vue';
import LiveListComponent from './components/LiveListComponent.vue';
import BarComponent from './components/BarComponent.vue';

export default {
  //注册组件
  components:{
    Headcomponent,
    bannerComponent,
    ClassifyComponent,
    LiveListComponent,
    BarComponent
  },
  data(){
    return{
      hello:"张三",
      menuList:[]
    }
  },
  mounted(){
    this.initClassify();
  },
  methods:{
    initClassify(){
      this.menuList=[
        {menuIcon:"",title:"全部"},
        {menuIcon:"",title:"靓女"},
        {menuIcon:"",title:"帅哥"},
        {menuIcon:"",title:"游戏大神"}
      ]
    }
  }

}
</script>
<style>
  *{
    margin: 0;
    padding: 0;
    list-style: none;
    box-sizing: border-box;
  }
</style>