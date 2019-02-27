<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <DataDisplay v-for="item in tweets"  :item="item" />
  
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import DataDisplay from './components/DataDisplay.vue'

export default {
  name: 'app',
  data () {
      return {
        moments: [{
        title:'Huawei unveils its foldable phone to rival Samsung' ,
        img:'https://ci6.googleusercontent.com/proxy/KJTgh2VsF6GE6BZlsxihYACYUDvhYSX5irJoxZ04XnSWj8aIdS0JAFjdg-qUK0sLCUnvW2URqpPsG6TMy-i2M0pe7Sguz_9XqKjRWGnP3De-vBW6C-RC3tSYfTuq9hzCBX_TLZiNaIgGXy0=s0-d-e1-ft#https://pbs.twimg.com/ext_tw_video_thumb/1099672071087575040/pu/img/Ykf5-sX2DutT_Vca.jpg' ,
        date:'Technology . Last night',
        description:"The folding version of the Chinese firm's Mate X range folds outward, compared to Samsung's, which opens like a book."
      },{
        title:'Equador hit with 7.5 magnitude earthquake' ,
        img:'https://ci4.googleusercontent.com/proxy/pQMZ-9lx74A-AbWpmpkvThe8DiBFyfUOxbBbqqiXsmlf46VTsAfD39sohKTMRnewhKW25XNeBNrd4ruMTYmWb0wtPpNe_q2iSQXyGRn4=s0-d-e1-ft#https://pbs.twimg.com/media/D0AaWb0WkAMOw1x.jpg?name=mosaic' ,
        date:'World News . Yesterday',
        description:"People in the small town of Palora, Ecuador, left their homes after feeling a magnitude 7.5 earthquake, according .."
      }],
        tweets: [
  {
    id: 1,
    name: 'James',
    handle: '@jokerjames',
    img: 'https://semantic-ui.com/images/avatar2/large/matthew.png',
    tweet: "If you don't succeed, dust yourself off and try again.",
    likes: 10,
  },
  { 
    id: 2,
    name: 'Fatima',
    handle: '@fantasticfatima',
    img: 'https://semantic-ui.com/images/avatar2/large/molly.png',
    tweet: 'Better late than never but never late is better.',
    likes: 12,
  },
  {
    id: 3,
    name: 'Xin',
    handle: '@xeroxin',
    img: 'https://semantic-ui.com/images/avatar2/large/elyse.png',
    tweet: 'Beauty in the struggle, ugliness in the success.',
    likes: 18,
  }
]
      }
    },
  components: {
    HelloWorld,DataDisplay
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
