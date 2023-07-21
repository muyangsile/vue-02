<template lang="">
    <div class="menu-box">
        <div v-for="item in menuList">
            {{item.title}}
        </div>
    </div>
</template>
<script>
export default {
    props:['menuList']
}
</script>
<style scoped>
    .menu-box{
        width: 100%;
        height: 100px;
        background-color: purple;
        margin-top: 2%;
    }
</style>