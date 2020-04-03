<template>
  <div id="app">
    <keep-alive include="Index,Detail">
      <router-view />
    </keep-alive>
  </div>
</template>

<script>
import FastClick from "fastclick";

export default {
  name: "App",
  mounted() {
    //解决移动端300秒延迟问题
    if ("addEventListener" in document) {
      document.addEventListener(
        "DOMContentLoaded",
        function() {
          FastClick.attach(document.body);
        },
        false
      );
    }
  }
};
</script>

<style>
html,
body,
#app,
.container {
  height: 100%;
}
</style>