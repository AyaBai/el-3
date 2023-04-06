<link rel="stylesheet" href="http://www.elementscss.com/css/elementscss.min.css">
<script setup>
  import { 
    Edit, DocumentChecked
     } from '@element-plus/icons-vue';
 


</script>

<template>
  <el-container>
    <el-aside width="66px" class="block">
      <div class="sideBar">
        <div class="sideBar_item">
          <el-button class="btn_icon">
            <img src="/burger.svg" alt="menu">
          </el-button>
        </div>
        <div class="sideBar_item">
          <el-button type="primary" class="img_item">
            <img src="/funnel.svg"  alt="funnel">
          </el-button>
        </div>
        <div class="sideBar_item">
          <el-button class="btn_icon">
            <img src="/check.svg" alt="menu">
          </el-button>
        </div>
        <div class="sideBar_item">
          <el-button class="btn_icon">
            <img src="/idCard.svg" alt="idCard">
          </el-button>
        </div>
      </div>
      <div class="sideBar">
        <div class="sideBar_item">
          <el-button class="btn_icon">
            <img src="/Photo.svg" alt="idCard">
          </el-button>
        </div>
        <div class="sideBar_item">
          <el-button class="rbtn_exit">
            <img src="/Left Icon.svg" alt="idCard">
          </el-button>
        </div>
      </div>
      
    </el-aside>
  </el-container>
</template>

<style scoped lang="sass">

  .block
    display: flex
    justify-content: space-between
    text-align: center
    flex-direction: column
    // padding-left: 8px
    // outline: 2px solid blue
    height: 100vh

  .sideBar_item
    // background-color: green
    color: white
    margin: 8px

  .btn_icon
   padding: 24px 8px
   border: none

  .btn_exit
    border-radius: 9999px

  .img_item
    padding: 10px
    
  

</style>
