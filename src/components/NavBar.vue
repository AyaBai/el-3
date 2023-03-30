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
    <div type="flex" class="header">
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
          class="w-5 m-2 navbar_input"
          size="small"
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
        <div>
          <el-space direction="horizontal">
            <el-text class="mx-1" size='small'>Итого:</el-text><el-text class="mx-1">3 580 800</el-text>
            <el-text class="mx-1" size='small'>Успешных:</el-text><el-text class="mx-1" type="success"> 3 580 800</el-text>
            <el-text class="mx-1" size='small'>Не успешных:</el-text><el-text class="mx-1" type="danger"> 3 580 800</el-text>
          </el-space>
        </div>
      </div>
    </div>
  </el-container>
</template>

<style scoped lang="sass">
  html, body
    padding:0
    margin:0
    
  .header
    display: flex
    justify-content: space-between
    flex-direction: column
    width: 1374px
    padding: 16px 8px 8px 16px
    // outline: 2px solid turquoise

  .navbar_up
    display: flex
    justify-content: space-between
    flex-direction: row
    // outline: 2px solid black
    margin: 16px 8px 8px 16px

  .navbar_btn
    padding: 5px 16px 5px 16px

  .navbar_bottom
    display: flex
    justify-content: space-between
    flex-direction: row
    // outline: 2px solid yellow

</style>
