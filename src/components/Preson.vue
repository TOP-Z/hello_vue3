<!--
 * @Description: 
 * @Author: 振顺
 * @Date: 2024-01-02 16:51:37
 * @LastEditTime: 2024-01-02 17:18:27
 * @LastEditors: 振顺
-->
<template>
  <div class="person">
    <h2>姓名：{{ name }}</h2>
    <h2>年龄：{{ age }}</h2>
    <button @click="changeName">修改名字</button>
    <button @click="changeAge">修改年龄</button>
    <button @click="showTel">查看联系方式</button>
  </div>
</template>

<script lang="ts">
export default {
  name: "Person", //组件名
  data() {
    return {
      name: "张三",
      age: 18,
      tel: "13888888888",
    };
  },
  methods: {
    showTel() {
      alert(this.tel);
    },
    changeName(){
      this.name = prompt("请输入新的名字");
    },
    changeAge(){
      this.age = prompt("请输入新的名字");
    },
  },
};
</script>
<style>
.person {
  background-color: skyblue;
  box-shadow: 0 0 10px;
  border-radius: 10px;
  padding: 20px;
}
button{
  margin: 0 5px;
}
</style>
