<template>
  <div class="scroll-wrapper" ref='wrapper'>
   <div class="scroll-conetent">
     <slot></slot>
   </div>
  </div>
</template>

<script>
import BScroll from 'better-scroll';

export default {
  name: 'Scroll',
  components: {
    data(){
      return{
        Scroll:null
      }
    }
  },
  mounted(){
    this.Scroll = new BScroll(this.$refs.wrapper)
  }
}
</script>

<style>

</style>