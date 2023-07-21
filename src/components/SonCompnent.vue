<template lang="">
    <div>
        大壮： {{cjb}} <br>
        <!-- <button @click="sendMessage">传递数据</button> -->
        <input type="text" v-model="message"  @keydown="sendMessage">
       <GrandsonComponentVue :cjb="cjb"></GrandsonComponentVue>
    </div>
</template>
<script>
import GrandsonComponentVue from './GrandsonComponent.vue';

export default {
    props:["cjb"],
    data(){
        return{
            message:""
        }
    },
    methods:{
        sendMessage(){
            this.$emit('suibian',this.message);
        }
    },
    components:{
        GrandsonComponentVue
    }
}
</script>
<style lang="">
    
</style>