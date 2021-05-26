<template>
  <header class="container">
    <div >
      <div><H1> Chitay-City</H1></div>
      <div><router-link  :to="{ name: 'Catalog'}">Каталог</router-link></div>
      <div><router-link :to="{ name: 'Admin'}">Админ панель</router-link></div>
    </div>
  </header>
</template>

<script>
import { BRow, BCol } from 'bootstrap-vue'
export default {
  name: 'VHeader',
  components: {
    BRow,
    BCol
  },
  directives: { 'v-header': this }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #50cceb;
}
</style>
