# simple_parent_child_communication_vue

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


### Reference
https://medium.com/covenant-university-developers-community/building-a-simple-data-filtering-app-with-vue-js-521420c73899

With data-binding


Vue.component('tag-list', {
   props: ['item'],
   template: '<li></li>'
 })

var app = new Vue({
   el: '#app',
   data: {
     tagList: [
       { tag: 'x-men' },
       { tag: 'avengers' },
       { tag: 'guardians of the galaxy' }
     ]
   } })

<div id="app">
   <ol>
     <tag-list v-for="list in tagList" v-bind:item="list"></tag-list>   
   </ol>
</div>
