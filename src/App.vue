<script setup>
  import { Search } from '@element-plus/icons-vue'
  import NavBar from './components/NavBar.vue'
  import HelloWorld from './components/HelloWorld.vue'
  import RightNavBar from './components/RightNavBar.vue'
  
</script>

<template>
  <div class="common-layout">
  
    <div>
      <RightNavBar></RightNavBar>
    </div>
    <div>
      <NavBar></NavBar>
      <HelloWorld></HelloWorld>
    </div>
  </div>
  
</template>

<style lang="sass">
  html, body
    padding:0
    margin:0
    
  .common-layout
    display: flex
    flex-direction: row 
    outline: 4px solid blueviolet
    background-color: #fff
    width: 100%



</style>
