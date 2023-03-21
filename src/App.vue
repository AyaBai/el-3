<script setup>
  import { Search } from '@element-plus/icons-vue'
  import NavBar from './components/NavBar.vue'
  import HelloWorld from './components/HelloWorld.vue'
  import RightNavBar from './components/RightNavBar.vue'
  
</script>

<template>
  <div class="container">
  
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
  .container
    display: flex
    flex-direction: row
    width: 1440px
    height: 934px
    color: #606266
    outline: 4px solid blueviolet


</style>
