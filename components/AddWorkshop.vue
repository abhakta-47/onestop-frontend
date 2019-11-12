<template>
  <div class="card">
    <div class="card-body">
      <div class="form-group">
        <input type="text" class="form-control">
      </div>
      <div class="form-group">
        <textarea type="text" class="form-control" rows="3">
      </div>
      <a-date-picker @change="onChange" />
    </div>
  </div>
</template>

<script>
import Vue from 'vue';
import { DatePicker } from 'ant-design-vue';
Vue.use(DatePicker);

import 'ant-design-vue/dist/antd.css';
export default {
methods: {
  onChange(date, dateString) {
        console.log(date, dateString);
      }
}
}
</script>
