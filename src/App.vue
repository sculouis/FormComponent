<template>
  <div id="app">
    <TextBox v-model="data1.val"></TextBox>
  </div>
</template>

<script>
import TextBox from "./components/TextBox";

var model = {
  data1: {
    val: "測試",
    value: "主檔",
    select: "1",
    date: "2019-05-15",
    picker: true
  },
  datas: [
    {
      no: 1,
      title: "標題1",
      val: 1234567890123.123,
      value: "測試TextBox",
      select: "1",
      date: "2019-05-15",
      picker: true,
      checked: true,
      isdelete: 0
    },
    {
      no: 2,
      title: "標題2",
      val: 1234567890123.123,
      value: "測試TextBox",
      select: "2",
      date: "2019-05-16",
      picker: false,
      checked: false,
      isdelete: 0
    }
  ]
};

export default {
  name: "App",
  data: function() {
    return model;
  },
  components: {
    TextBox
  },
  mounted: {}
};
</script>

<style>
#app {
}
</style>
