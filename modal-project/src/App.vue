<template>
  <div>
    <p>{{ title }}</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      title: 'My First Vue.js App'
    }
  },
  components: {
    
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
  margin-top: 60px;
}
</style>
