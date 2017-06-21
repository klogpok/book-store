<template>
  <section class="popup book-details">
    <button @click="closeMe">x</button>
    <h1>Details of: {{book.title}}</h1>
    <img src="http://via.placeholder.com/250x150">
    <h3>&#36;{{book.price}}</h3>
    <p>{{book.description}}</p>
    <button @click="requestNextBook">Next > </button>
  </section>
</template>

<script>
  export default {
    name: 'book-details',
    props: ['book'],
    data () {
    },
    methods: {
      closeMe() {
        console.log('close me!');
        this.$emit('close');
      },
      requestNextBook() {
        console.log('Requesting Next');
        this.$emit('next');
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
