<template>
<div>
  <h1>{{title}}</h1>
  <Modal :header="header" :text="text" theme="sales" />
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
