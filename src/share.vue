<script setup>
import { ref } from 'vue'
import Cookies from 'js-cookie'
function setrmad(){Cookies.set('rmads', '1', { expires: 7 })}

const aaurl = ref("/ads/share2.png")
</script>

<template>
  <img alt="二维码" :src="aaurl" style="max-width: 80%; max-height: 80%;"/>
  <h2><a :href="aaurl" v-on:click="setrmad" style="font-size: 3em;" download>保存分享</a></h2>
</template>



<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>