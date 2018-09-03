<template>
    <div>
        <TitleBar text="推荐歌单"></TitleBar>
        <PictureList></PictureList>
        <TitleBar text="热门音乐"></TitleBar>
        <MusicList></MusicList>

    </div>
</template>

<script>
    import TitleBar from './TitleBar'
    import PictureList from './PictureList'
    import MusicList from './MusicList'
    import MusicItem from './MusicItem'
  export default {
      components:{
        TitleBar,
        PictureList,
        MusicList,
        MusicItem
      },
    name: "recommend-music-tab"
  }
</script>

<style scoped>

</style>