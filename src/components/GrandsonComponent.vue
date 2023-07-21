<template lang="">
    <div>
        小壮：{{cjb}} <br>
        {{sj}}
    </div>
</template>
<script>
export default {
    props:["cjb"],
    inject:["sj"]
}
</script>
<style lang="">
    
</style>