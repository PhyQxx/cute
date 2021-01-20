<template>
  <div class="background">
    <el-timeline>
      <el-timeline-item
        v-for="(activity, index) in activities"
        :key="index"
        :type="activity.type"
        :size="activity.size"
        :color="activity.color"
        :icon="activity.icon"
        :timestamp="activity.timestamp"
        :placement="activity.placement">
        <el-card>
          <h4>三毛流浪记</h4>
        </el-card>
      </el-timeline-item>
    </el-timeline>
  </div>
</template>

<script>
  export default {
    name: "index",
    data() {
      return{
        activities: [{
          type: 'success',
          size: 'middle',
          color: 'red',
          icon: 'el-icon-more',
          timestamp: '2021-01-19',
          placement: 'top'
        },{
          type: 'success',
          size: 'middle',
          color: 'red',
          icon: 'el-icon-more',
          timestamp: '2021-01-01',
          placement: 'top'
        }]
      }
    }
  }
</script>

<style scoped>
  .background {
    height: 54rem;
    width: 100%;
    background: url("~@/assets/yupiaoxue/bg.jpg") no-repeat fixed;
    background-size: 100% 100%;
    opacity: 0.2;
  }
</style>
