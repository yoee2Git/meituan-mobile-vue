<template>
  <Scroll>
    <current-city></current-city>
    <city-list></city-list>
  </Scroll>
</template>

<script>
// import BetterScroll from 'better-scroll';
import Scroll from "../common/BScroll"

import CurrentCity from "./CityList/CurrentCity";
import CityList from "./CityList";

export default {
  name: "CityScrollWrapper",
  components: {
    CurrentCity,
    CityList,
    Scroll
  },
  // mounted() {
  //   this.scroll = new BetterScroll(this.$refs.wrapper);
  // }
};
</script>

<style>
</style>