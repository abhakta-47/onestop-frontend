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
import axios from 'axios';
import { DatePicker } from 'ant-design-vue';
Vue.use(DatePicker);

import 'ant-design-vue/dist/antd.css';
export default {
  methods: {
    onChange(date, dateString) {
          console.log(date, dateString);
        },
    submit() {
      var self = this;
      axios.post('https://dxepsmwpz6.execute-api.ap-south-1.amazonaws.com/production/profile', {
        "email":self.email,"name":self.name,"rollNo":self.rollNo,"contactNo":self.contactNo
      }).then(res => {})
    }
  }
}
</script>
