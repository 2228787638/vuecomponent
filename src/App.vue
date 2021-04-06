<template>
  <div id="app">
    按钮组件：<br>
    <gd-button text="默认按钮" color="#34495e"/>
    <gd-button text="默认按钮" type="default"/>
    <gd-button text="主要按钮" color="#3498db"/>
    <gd-button text="主要按钮" type="main"/>
    <gd-button text="成功按钮" color="#2ecc71"/>
    <gd-button text="成功按钮" type="success"/>
    <gd-button text="信息按钮" color="#d35400"/>
    <gd-button text="信息按钮" type="information"/>
    <gd-button text="警告按钮" color="#8e44ad"/>
    <gd-button text="警告按钮" type="warning"/>
    <gd-button text="危险按钮" color="#c0392b"/>
    <gd-button text="危险按钮" type="danger"/>
  </div>
</template>

<script>
import GdButton from "./components/button/gd-button";
export default {
  name: 'app',
  components: {GdButton},
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {

}
</style>
