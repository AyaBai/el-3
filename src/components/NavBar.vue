<script setup>
  import { ref } from 'vue'
  import { 
    Search,
    Bell
     } from '@element-plus/icons-vue'

  const value = ref('')
  const input2 = ref('')

  const options = [
    {
      value: 'Option',
      label: 'Название воронки1',
    },
    {
      value: 'Option2',
      label: 'Название воронки2',
    },
    {
      value: 'Option3',
      label: 'Название воронки3',
    },
    {
      value: 'Option4',
      label: 'Название воронки4',
    },
    {
      value: 'Option5',
      label: 'Название воронки5',
    },
    {
      value: 'Option6',
      label: 'Название воронки6',
    },
  ]

</script>

<template>
  <el-container>
    <el-header type="flex">
    <div class="navbar_up">
      <el-select v-model="value" class="m-2 list_name" placeholder="Название воронки">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        />
      </el-select>
      <el-input
        v-model="input2"
        class="w-50 m-2 navbar_input"
        placeholder="Поиск + фильтр"
        :prefix-icon="Search"
      />
      <el-button class="navbar_btn" type="primary">Добавить сделку</el-button>
      <el-button class="navbar_bell" :icon="Bell" circle></el-button>
    </div>
  
    <div class="navbar_bottom">
      <div>
        <el-button type="primary" round>Воронка</el-button>
        <el-button round>Список</el-button>
      </div>
    </div>
    </el-header>
  </el-container>
</template>

<style scoped lang="sass">
  .cover
    // display: flex
    flex-direction: row
    justify-content: flex-start

    outline: 2px solid green
    width: 1374px
    height: 100px

  .navbar_up
    width: 1350px
    height: 32px

  .navbar_bottom

  .list_name
    width: 177px
    height: 32px
    // margin: 18px 12px 10px 16px

  .navbar_input
    width: 925px
    height: 32px
    padding: 5px 32px
    // margin: 18px 12px 10px 0px

  .navbar_btn
    // margin: 18px 12px 10px 0px

  .navbar_bell
    // margin: 16px 23px 10px 0px

 


  
</style>
