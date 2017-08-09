<template>
  <div id="app">
    <img src="./assets/logo.png" @click="showToast">
    <hello></hello>
  </div>
</template>

<script>
import Hello from './components/Hello'
import Toast from './components/toast';

export default {
  name: 'app',
  components: {
    Hello
  },
  methods: {
    showToast () {
      console.log(Toast)
      Toast('Upload Completed');
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
