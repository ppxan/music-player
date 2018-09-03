<template>
    <div class="gridlist">
        <mu-grid-list class="gridlist-demo" :cols="2" :columnHeight="110">
            <mu-grid-tile v-for="(tile,index) in list" v-bind:key="index">
                <img :src="tile.image">
                <span slot="title">{{tile.title}}</span>
                <span slot="subTitle">by <b>{{tile.author}}</b></span>
                <mu-button slot="action" icon>
                    <mu-icon value="star_border"></mu-icon>
                </mu-button>
            </mu-grid-tile>
        </mu-grid-list>
    </div>
</template>

<script>
  import breakfast from '../../1.jpg'

  export default {
    name: "picture-list",
    data: function () {
      return {
        list: [{
          image: breakfast,
          title: 'Breakfast',
          author: 'Myron'
        },{
          image: breakfast,
          title: 'Breakfast',
          author: 'Myron'
        },{
          image: breakfast,
          title: 'Breakfast',
          author: 'Myron'
        },{
          image: breakfast,
          title: 'Breakfast',
          author: 'Myron'
        }]
      }
    }
  }
</script>

<style scoped>
</style>