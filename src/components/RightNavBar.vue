<script setup>
  import { 
    Edit
     } from '@element-plus/icons-vue';
 


</script>

<template>
  <el-container>
    <el-aside width="66px" class="block">
      <button class="burger_btn"></button>
      <button class="funnel_btn"></button>
      <button class="check_btn"></button>
      <button class="id_btn"></button>
    </el-aside>
  </el-container>
</template>

<style scoped lang="sass">
  .block
    display: flex
    justify-content: space-between
    flex-direction: column
    outline: 2px solid blue

  .burger_btn,
  .funnel_btn,
  .check_btn,
  .id_btn
    background-repeat: no-repeat
    background-size: contain

  .burger_btn
    background-image: url(/menu_FILL.svg)
    padding: 24px 8px    

  .funnel_btn
    background-image: url(/funnel.svg)
    padding: 10px

  .check_btn
    background-image: url(/check2.svg)
    padding: 10px

  .id_btn
    background-image: url(check1.svg)
    padding: 10px
    width: 20px
    height: 20px

  

</style>
