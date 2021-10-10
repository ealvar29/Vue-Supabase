<template>
  <div>
    <p>{{ title }}</p>
    <div v-if="showModal"> 
    <Modal theme="Sale" @close="toggleModal">
      <h1>Ninja Giveaway</h1>
      <p>Testing slots</p>
      <template>
        <a href="#">Sign up now</a>
        <a href="#">More Info</a>
      </template>
    </Modal>
    </div>
    <button @click="toggleModal">Open Modal</button>
  </div>
</template>

<script>
import Modal from "./components/Modal.vue"

export default {
  name: 'App',
  components: { Modal },
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
