<script>
export default {
  props: ["cArr"],
  methods: {
    //点击按钮后把自己的分类传递出去
    change(x) {
      // console.log(x);
      // 自定义事件
      this.$emit("MyEvent", x);
    },
  },
};
</script>
<template>
  <div v-for="x in cArr">
    <button @click="change(x)">{{ x }}</button>
  </div>
</template>
<style scoped>
button {
  width: 150px;
  height: 50px;
  background-color: pink;
  margin-top: 5px;
}
</style>