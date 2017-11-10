<template>
  <div :class="className"></div>
</template>

<style scoped>
  .vue-echarts {
    width: 100%;
    height: 100%;
  }
</style>

<script>
  let ECharts = require('echarts');
  import Debounce from 'lodash.debounce';
  // import Resize from 'element-resize-event';
  import Resize from 'element-resize-detector';
  import Wrapper from './wrapper.js';

  console.log('test')

  const IEcharts = Wrapper(ECharts, Resize, Debounce);
  export default IEcharts;
</script>
