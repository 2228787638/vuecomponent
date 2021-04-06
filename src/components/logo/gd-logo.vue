<template>
  <div>
    <span><strong>A</strong> P <strong>M</strong> D</span>
  </div>
</template>

<script>
export default {
  name: "gd-logo"
}
</script>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

div {
  cursor: pointer;
  color: #2c3e50;
  font-size: 2em;
}

div strong {
  display: inline-block;
  transition: 1s;
  background: #2c3e50;
  border-radius: 50%;
  width: 45px;
  height: 45px;
  text-align: center;
  color: #ecf0f1;
}

div span strong:nth-of-type(1) {
  background: #27ae60;
}

div span strong:nth-of-type(2) {
  background: #f1c40f;
}

div span:hover strong:nth-of-type(1) {
  transform: rotate(360deg) scale(1.5);
  background: #27ae60;
}

div span:hover strong:nth-of-type(2) {
  transform: rotate(-360deg) scale(1.5);
  background: #f1c40f;
}
</style>
