<template>
  <div id="knrm-1">
    <div id="title">KNRM</div>
    <el-tabs v-model="activeName" type="card">
      <el-tab-pane label="Description" name="first">
        <description></description>
      </el-tab-pane>
      <el-tab-pane label="Guideline" name="second">
        <guideline></guideline>
      </el-tab-pane>
      <el-tab-pane label="Demo" name="third">
        <demo></demo>
      </el-tab-pane>
    </el-tabs>
  </div>
</template>

<script>
  import Description from './Description'
  import Guideline from './Guideline'
  import Demo from './Demo'

  export default {
    name: 'KNRM',
    data () {
      return {
        activeName: 'first'
      }
    },
    components: {
      'description': Description,
      'guideline': Guideline,
      'demo': Demo
    }
  }
</script>

<style scoped>
  #title{
    font-size: 30px;
  }
  #knrm-2 {
    overflow: hidden;
  }
</style>
