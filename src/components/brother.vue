<template>
  <div>
      <h3>兄弟組件</h3>
  </div>
</template>

<script>
export default {
    name:'brother',
    created(){
        this.$bus.$on('sayLoveBrother',this.getLove)
    },
    methods:{
        getLove(e){
            console.log('兄弟組件',e)
        }
    }
}
</script>

<style>

</style>