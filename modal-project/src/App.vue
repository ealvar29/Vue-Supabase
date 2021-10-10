<template>
  <div>

  </div>
</template>

<script>


export default {
  name: 'App',
  components: {  },
  data() {
    return {
      title: 'My First Vue.js App',
      header: "sign up for giveaway",
      text: "Grab your inventory",
      theme: "",
      showModal: false
    }
  },
  methods: {
    toggleModal(){
      this.showModal = !this.showModal;
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
  margin-top: 60px;
}
</style>
