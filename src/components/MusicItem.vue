<template>
    <div class="container">
        <div class="s-title">
            {{name}}
        </div>
        <div class="s-singer">
            {{singer}}
        </div>
        <div class="icon">
            <mu-icon value="play_circle_outline" color="#888"></mu-icon>
        </div>
    </div>
</template>

<script>
  export default {
    name: "music-item",
    data:function(){
      return{
      }
    },
    props:['name','singer']
  }
</script>

<style scoped>
.s-title{
    font-size: 17px;
}
    .s-singer{
        font-size: 12px;
        color: #888;
    }
    .container{
        position: relative;
        border-bottom: 1px #ddd solid;
        padding: 5px 10px;
    }
    .icon{
        position: absolute;
        right:10px;
        top:13px;
    }
</style>