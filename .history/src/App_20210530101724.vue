<template>
<div>
  <h1>{{title}}</h1>
  <Modal/>
</div>
</template>

<script>
import Modal from './components/Modal'

export default {
  name: 'App',
  components: {Modal},
  data() {
    return {
      title: 'My first template'
    }
  },
  
 }
</script>

<style>
.modal {
    width: 400px;
    padding: 20px;
    margin: 200px auto;
    background: white;
    border-radius: 10px;
  }
  .backdrop {
    top: 0;
    position: fixed;
    background: rgba(0,0,0,0.5);
    width: 100%;
    height: 100%;
  }
  .modal h1 {
    color: #03cfb4;
    border: none;
    padding: 0;
  }
  .modal p {
    font-style: normal;
  }
</style>
