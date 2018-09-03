<template>
    <div class="container">
        {{text}}
    </div>
</template>

<script>
  export default {
    name: "title-bar",
    data:function(){
      return {}
    },
    props:['text']
  }
</script>
<style scoped>
    .container{
        position: relative;
        padding: 10px;
    }
.container:after {
    content: " ";
    position: absolute;
    left: 0;
    top: 50%;
    margin-top: -9px;
    width: 2px;
    height: 16px;
    background-color: #d33a31;
}
</style>