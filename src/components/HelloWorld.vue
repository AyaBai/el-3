<script>
  import {Tickets} from '@element-plus/icons-vue'

  export default {
    data() {
          return {
            items: [
              {
                number:'200',
                result:'100 000 000₸',
                name:'Название сделки', 
                icon:'',
                calendar:'15.03.2022',
                time:'23:00'

              }
            ],
            total: [
              {
                sum: '1 000 000₸',
                percent: '100%'
              }
            ]
          }
    }
  }

</script>

<template>
  <el-container class="main_list">
    <el-main>
      <el-row :gutter="20">
        <el-col :span="4">
          <div class="grid-content ep-bg-purple head_cell bg-[#409EFF]">Название этапа (0)</div>
            
          <div class="total_line" v-for="cell in total" :key="cell.sum">
            <div class="grid-content text-[#606266] bg-transparent inline-block text-base ">{{cell.sum}}</div>
            <div class="grid-content text-[#606266] bg-transparent text-xs">{{cell.percent}}</div>
          </div>

          <div  class="deal_cell">
            <div v-for="item in items" :key="item.number" class="cover_cell">
              <div class="cell_up">
                <span class="number_cell">
                  <img src="/Union.svg">
                  {{item.number}}
                </span><br>
                <span class="result_cell"> {{item.result}}</span><br>
              </div>
              <span class="name_cell"> {{item.name}}</span><br>
              <div class="cell_up">
                <span class="icon_cell">{{item.icon}}</span><br>
                <div class="cell_right">
                  <span class="calendar_cell">{{item.calendar}}</span><br>
                  <span class="time_cell">{{item.time}}</span>
                </div>
              </div>
            </div>
          </div>

        </el-col>
        <el-col :span="4">
          <div class="grid-content ep-bg-purple head_cell bg-[#7D40FF]">Название этапа (0)</div>
          
          <div class="total_line" v-for="cell in total" :key="cell.sum">
            <div class="grid-content text-[#606266] bg-transparent inline-block text-base ">{{cell.sum}}</div>
            <div class="grid-content text-[#606266] bg-transparent text-xs">{{cell.percent}}</div>
          </div>

          <div  class="deal_cell">
            <div v-for="item in items" :key="item.number" class="cover_cell">
              <div class="cell_up">
                <span class="number_cell">
                  <img src="/Union.svg">
                  {{item.number}}
                </span><br>
                <span class="result_cell"> {{item.result}}</span><br>
              </div>
              <span class="name_cell"> {{item.name}}</span><br>
              <div class="cell_up">
                <span class="icon_cell">{{item.icon}}</span><br>
                <div class="cell_right">
                  <span class="calendar_cell">{{item.calendar}}</span><br>
                  <span class="time_cell">{{item.time}}</span>
                </div>
              </div>
            </div>
          </div>
        </el-col>

        <el-col :span="4">
          <div class="grid-content ep-bg-purple head_cell bg-[#CD40FF]">Hазвание этапа (0)</div>
        </el-col>
        <el-col :span="4">
          <div class="grid-content ep-bg-purple head_cell bg-[#B25600]">Название этапа (0)</div>
        </el-col>
        <el-col :span="4">
          <div class="grid-content ep-bg-purple head_cell bg-[#00B512]">Название этапа (0)</div>
        </el-col>
        <el-col :span="4"><div class="grid-content ep-bg-purple head_cell bg-[#F56C6C]">Название этапа (0)</div></el-col>
      </el-row>
    </el-main>
  </el-container>
  
</template>

<style scoped lang="sass">
  html, body
    padding:0
    margin:0
    
  
  .main_list
    // outline: 2px solid red
    background-color: #F2F3F5

  .el-row 
    margin-bottom: 20px

  .el-row:last-child 
    margin-bottom: 0

  .el-col 
    border-radius: 4px


  .grid-content 
    border-radius: 4px
    min-height: 36px

  .total_line
    display: flex
    justify-content: space-between
    margin: 12px
    align-items: baseline

  .head_cell
    border-radius: 0px 16px 16px 0px
    padding: 4px 8px
    color: #fff

  .deal_cell
    margin-right: 20px
    display: inline-block
    // outline: 2px solid orangered
    background: #FFFFFF
    width: 203px
    // height: 107px
    border-radius: 0px 4px 4px 0px
    padding: 12px 8px
    


  .number_cell
    background: #F0F2F5
    border-radius: 100px
    padding: 2px 8px
    font-size: 12px
    font-weight: 400  
    display: flex
    // height: 16px


  .result_cell
    font-weight: 400
    font-size: 12px
    color: #606266

  .name_cell
    color: #409EFF
    font-weight: 500
    font-family: 'PingFang SC'
    text-align: left

  .icon_cell
    background-image: url(/Frame.svg)
    background-repeat: no-repeat
    background-size: cover
    width: 24px
    height: 24px


  .calendar_cell,
  .time_cell
    color: #909399
    font-size: 10px

  .cover_cell
    display: flex
    justify-content: space-between
    flex-direction: column

  .cell_up
    display: flex
    justify-content: space-between
    flex-direction: row
    align-items: baseline

  .cell_right
    flex-direction: column
    text-align: right



    
</style>
