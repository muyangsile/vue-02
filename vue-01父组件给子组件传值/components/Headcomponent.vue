<template lang="">
    <div class="h_box">
        <span>首页</span>
        <input type="text"/>
        <div>搜索</div>{{posttitle}}
    </div>
</template>
<script>
export default {
    props:['posttitle'],
    data(){
        return{
            
        }
    }
}
</script>
<style scoped>
    .h_box{
        display: flex;
        margin-top: 2%;
    }
    .h_box>input{
        width: 60%;
        margin-left: 5%;
        margin-right: 5%;
    }
</style>