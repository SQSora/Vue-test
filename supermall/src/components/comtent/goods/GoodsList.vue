<template>
  <div class="goods">
    <goods-list-item v-for="item in goods":goods-item="item" />
  </div>

</template>

<script>
import GoodsListItem from './GoodsListItem.vue';


export default {
  components: { GoodsListItem },
  name: 'Goodslist',

  props: {
    goods:{
    type: Array,
    default(){
      return[]
    }
    }
  },

};
</script>

<style >
  .goods{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 2px;
  }
  
</style>