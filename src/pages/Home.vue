<template>
<b-container fluid class="main">
  <navbar/>
  
</b-container>
</template>

<script>
import Navbar from '../components/Navbar.vue'

  export default {
  components: { Navbar },

  }
</script>

<style scoped>
.main{
  padding: 0;
}
.con{
  margin-right: 5rem;
  margin-left: 4.2rem;
  margin-top: 1.5rem ;
}
</style>