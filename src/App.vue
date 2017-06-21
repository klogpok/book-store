<template>
  <div id="app">
    <img src="./assets/logo.png">
    <book-list></book-list>
  </div>
</template>

<script>
import BookList from './components/BookList.vue'
import Cart from './components/Cart.vue'
import BookDetails from './components/BookDetails.vue'
import BookFilter from './components/BookFilter.vue'
import BookPreview from './components/BookPreview.vue'
import BookEdit from './components/BookEdit.vue'

export default {
  name: 'app',
  components: { BookList, Cart, BookDetails, BookFilter, BookPreview , BookEdit}
}
</script>

<style>
  body {
    background: lightcoral;
  }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
