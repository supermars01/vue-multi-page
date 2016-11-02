<template>
  <ul class="one">
    <!-- <li v-for="(item, index) of items">
      {{ item.msg }}
      <hr />
    </li> -->
    <li v-for="(index, item) of items" track-by="$index">
         {{ item.msg }} － {{ index }}
    </li>
  </ul>
</template>
<script>
export default {
  name:'one',
  data: function() {
    return {
      items:[
        {msg: 'james'},
        {msg: 'wede'},
        {msg: 'kobe'},
        {msg: 'antony'},
        {msg: 'hadden'}
      ]
    }
  }
}
</script>

<style lang='sass'>
  $color : #cacaca;
  body{ background-color: $color;color:#999;}
</style>
