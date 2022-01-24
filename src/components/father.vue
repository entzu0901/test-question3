<template>
  <div>
    <h2>父親組件</h2>
    <son :count="count" @sayLove="getLove"></son>
    <brother></brother>
  </div>
</template>

<script>
import son from './son.vue'
import brother from './brother.vue'
export default {
    name:"father",
    data() {
        return {
            count:1,
        }
    },
    components:{son,brother},
    methods:{
        getLove(e){
           console.log(e)
        }
    }
};
</script>

<style>

</style>