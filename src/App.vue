<template>
  <div>
    <h2>vue組件通信</h2>
    <father></father>
  </div>
</template>

<script>
import father from './components/father.vue'
export default {
  name:'app',
  components:{
    father
  },
  data() {
      return {
      
        }
    },
  methods:{
    
  }  
}
</script>

<style>
 
</style>