<template>
  <div id="app">
    <Header msg="HOGEHOGE" />
    <p>{{ msg }}</p>
    <input type="text" v-model="msg">
    <button @click="clear()">clear</button>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  components: {
    Header
  },
  data() {
    return {
      msg: "Hello World!"
    }
  },  
  methods: {
    clear () {
      this.msg = ''
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 800px;
  margin: 60px auto;

}
</style>
