<template>
  <div id="app">
    <HeaderBar></HeaderBar>
    <ContentTab></ContentTab>
  </div>
</template>

<script>
  import HeaderBar from './components/HeaderBar'
  import ContentTab from './components/ContentTab'

export default {
  name: 'app',
  components:{
    HeaderBar,
    ContentTab
  },
  data: function(){
    return {
    }
  }
}
</script>

<style>
  #app{
    overflow-y: hidden;
  }
</style>
