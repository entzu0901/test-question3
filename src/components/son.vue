<template>
  <div class="son">
      <h2>兒子組件</h2>
      <span>父組件傳過來的值{{count}}</span>
      <button @click="sayLove">表達</button>
  </div>
</template>

<script>
export default {
    name:"son",
    props:['count'],
    methods:{
        sayLove(){
            this.$emit('sayLove','I LOVE YOU FATHER')
            this.$bus.$emit('sayLoveBrother','I LOVE YOU Brother')
        }
    }
}
</script>
