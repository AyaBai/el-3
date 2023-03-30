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
    // justify-content: space-between
    flex-direction: column
    outline: 2px solid blue
    height: 100%

  .burger_btn,
  .funnel_btn,
  .check_btn,
  .id_btn
    display: inline-block
    background-repeat: no-repeat
    background-size: contain

  .burger_btn
    background-image: url(/menu_FILL.svg)
    padding: 24px 8px
    width: 40px
    height: 40px  

  .funnel_btn
    background-image: url(/Funnel.svg)
    padding: 10px

  .check_btn
    background-image: url(/Check.svg)
    padding: 10px

  .id_btn
    background-image: url(IdCard.svg)
    padding: 10px
    width: 40px
    height: 24px

  

</style>
