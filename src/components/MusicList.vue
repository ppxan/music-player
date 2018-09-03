<template>
    <div class="musiclist">
        <MusicItem v-for="item in list" :name="item.name" :singer="item.singer"></MusicItem>
    </div>
</template>

<script>
  import MusicItem from './MusicItem'
  export default {
    name: "music-list",
    data:function(){
      return {
        list:[{
          name:'幻听',
          singer:'许嵩'
        },{
          name:'幻听',
          singer:'许嵩'
        },{
          name:'幻听',
          singer:'许嵩'
        },{
          name:'幻听',
          singer:'许嵩'
        },{
          name:'幻听',
          singer:'许嵩'
        },{
          name:'幻听',
          singer:'许嵩'
        }]
      }
    },
    components:{
      MusicItem
    }
  }
</script>

<style scoped>

</style>