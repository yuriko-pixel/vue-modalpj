<template>
<div>
  <h1>{{ title }}</h1>
  <p>Welcome...</p>
  <div v-if="showModal">
    <Modal :heading="heading" :text="text" theme="sale" @close="toggleModal">
      <h1>Sign up for the Givaway!</h1>
      <p>Grab your ninja swag for half price!</p>
    </Modal>
  </div>  
  <button @click="toggleModal">open modal (alt)</button>
</div>
</template>

<script>
import Modal from './components/Modal'
export default {
  name: 'App',
  components: { Modal },
  data() {
    return {
      title: 'My First Vue App!',
      heading: 'Sign up for the Givaway!',
      text: 'Grab your ninja swag for half price!',
      showModal: false,
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