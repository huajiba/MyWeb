<script>
import Child from "./Child.vue";
export default {
  data() {
    return {
      arr: [
        "水果",
        "蔬菜",
        "肉禽蛋",
        "海鲜水产",
        "粮油调味",
        "熟食卤味",
        "茶水饮料",
      ],
      msg: "水果",
    };
  },
  components: {
    Child,
  },
  methods: {
    change(x){
        this.msg=x;
    }
  },
};
</script>
<template>
  <h1>子传父-分类切换案例</h1>
  <div id="left">
    <child :cArr="arr" @MyEvent="change"/>
  </div>
  <div id="right">
    <p>请求{{ msg }}数据</p>
  </div>
</template>
<style scoped>
#left {
  width: 160px;
  height: 500px;
  background-color: gainsboro;
  float: left;
}
#right {
  width: 400px;
  height: 500px;
  background-color: rgb(255, 102, 0);
  float: left;
}
</style>