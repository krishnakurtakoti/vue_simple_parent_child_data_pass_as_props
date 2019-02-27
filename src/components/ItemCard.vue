<template>
<div>

  <div class="items-center "
 <div class="max-w-sm border border-grey-dark items-center p-2">
 <h3 class="card-title">{{ item.name}} </h3>
 
       <div class="px-2">

    <span v-for="(group, index) in item.stack" :key="index"  v-bind:class="group.color"    class="bg-yellow border border-black px-2" > {{ group.type }} </span>
</div>

</div>
</div>

</div>
</template>
<script>
export default {
  name: 'ItemCard',
    data() {

    return {
    // list of tags to giving each stack a different color

      tags: {

        language: 'green',

        framework: 'blue',

        frontend: 'pink',

        backend: 'grey',

        mobile: 'black',

        web: 'yellow',

        hybrid: 'red',

        database: 'orange'

      }

    };

  },
  props: {
    item: Object,
     required: true
    
    
  }
}
</script>