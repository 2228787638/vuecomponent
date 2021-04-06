<template>
  <span>
    <a href="" class="btn" :style="{'--color':color}">{{ text }}</a>
  </span>
</template>

<script>
export default {
  props: ['text', 'color', 'type'],
  name: "gd-button",
  created() {
    if (this.type === 'default') this.color = '#34495e'
    else if (this.type === 'main') this.color = '#3498db'
    else if (this.type === 'success') this.color = '#2ecc71'
    else if (this.type === 'information') this.color = '#d35400'
    else if (this.type === 'warning') this.color = '#8e44ad'
    else if (this.type === 'danger') this.color = '#c0392b'
  }
}
</script>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

span {
  width: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  float: left;
  margin: 2px;
}

span a {
  background: var(--color);
  color: #ecf0f1;
  font-size: 1em;
  text-decoration: none;
  border: solid 2px #ecf0f1 !important;
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 40px;
  position: relative;
  overflow: hidden;
  border-radius:25px;
  transition: 1s;
  z-index: 0;
}

.btn::after {
  content: '';
  width: 0;
  height: 100%;
  position: absolute;
  background: #ecf0f1 !important;
  z-index: -1;
  transition: 1s;
}

.btn:hover{
  color: var(--color);
}

.btn:hover::after{
  width: 200%;
}
</style>
