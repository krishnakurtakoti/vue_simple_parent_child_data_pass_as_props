<template>
<div>


 
  <div>
    {{ item.name }} | {{ item.handle }} | {{ item.tweet }}
  </div>

 
 



</div>
</template>
<script>
export default {
  name: 'DataDisplay',
  props: {
    item: Object
    
    
  }
}
</script>