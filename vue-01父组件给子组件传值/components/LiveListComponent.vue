<template lang="">
    <div class="liveBox">
        <LiveItem v-for="num in 10"></LiveItem>
    </div>
</template>
<script>
import LiveItem from './view/LiveItem.vue';
export default {
    components:{
        LiveItem
    }
}
</script>
<style scoped>
    .liveBox{
        width: 100%;
        padding-left: 5%;
        padding-right: 5%;
        min-height: 300px;
        margin-top: 2%;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>