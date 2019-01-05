<template>
  <li @click="handleClick">{{content}}</li>
</template>

<script>
export default {
    props: ['content','index'],
    methods: {
        handleClick:function(){
            this.$emit('delete',this.index)
        }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--全局样式与局部样式-->
<style scoped>

</style>
