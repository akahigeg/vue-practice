<template>
  <header class="header">
    <h1>FIRST VUE</h1>
    <p>{{ msg }}</p>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<style>
.header {
  padding-bottom: 30px;
  border-bottom: 2px solid #999;
}
</style>