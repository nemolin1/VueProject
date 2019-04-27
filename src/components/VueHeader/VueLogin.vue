<template>
<div>
    <p>login component <span @click='cover'>{{isDrop ===true?'展开':'隐藏'}}</span></p>
</div>
</template>
<script>
export default {
    data (){
        return {
            isDrop:false
        }
    },
    methods:{
        cover (){
            this.isDrop = !this.isDrop
        }
    }
}
</script>
<style scoped>

</style>