<template>
  <div ref='wrapper'>
   <div class="content">
     <slot></slot>
   </div>
  </div>
</template>

<script>
import BScroll from 'better-scroll';

export default {
  name: scroll,
  components: {
    data(){
      return{
        bscroll:null
      }
    }
  },
  mounted(){
    this.bscroll = new BScroll(this.$refs.wrapper,{

    })
  }
}
</script>

<style>

</style>