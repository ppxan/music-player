<template>
    <div class="container">
        <div class="tab">

            <mu-tabs :value.sync="active" inverse color="#d43c33" text-color="#d43c33" indicator-color="#d43c33" full-width  center>
                <mu-tab>推荐音乐</mu-tab>
                <mu-tab>热门歌曲</mu-tab>
                <mu-tab>搜索</mu-tab>
            </mu-tabs>
    </div>
            <div class="demo-text" v-if="active === 0">
                <RecommendMusicTab></RecommendMusicTab>
            </div>
            <div class="demo-text" v-if="active === 1">
                <HotMusicTab></HotMusicTab>
            </div>
            <div class="demo-text" v-if="active === 2">
                <SearchTab></SearchTab>
            </div>
    </div>
</template>

<script>
    import RecommendMusicTab from './RecommendMusicTab'
    import SearchTab from './SearchTab'
    import HotMusicTab from './HotMusicTab'
  export default {
    components:{
      RecommendMusicTab,
      SearchTab,
      HotMusicTab
    },
    name: "content-tab",
    data: function(){
      return {
        active: 1
      }
    }
  }
</script>

<style scoped>
.container{
    padding: 0;
    color: black;
}
    .active-tab{
        color: #d43c33;
    }
    .tab{
        position: fixed;
        margin-top: 50px;
        width: 100%;
        z-index: 1000;
    }
</style>