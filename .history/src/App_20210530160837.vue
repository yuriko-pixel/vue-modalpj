<template>
<div>
  <h1>{{title}}</h1>
  <div v-if="showModal">
    <Modal :heading="heading" :text="text" theme="sale" @close="toggleModal" />
  </div>  
  <button @click="toggleModal">open modal</button>
</div>
</template>

<script>
import Modal from './components/Modal'

export default {
  name: 'App',
  components: {Modal},
  data() {
    return {
      title: 'My first template',
      header: 'Sign up for the Giveaway!',
      text: 'Grab your ninja swag for half price!',
      showModa: false
    }
  },
   methods: {
    toggleModal() {
      this.showModal = !this.showModal
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
h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom: 10px;
}
</style>
