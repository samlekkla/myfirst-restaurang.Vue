<template>
  <div class="home">
     <img class="restaurant-logo" alt="Restaurant Logo" src="../assets/Res.jpg">
    <HelloWorld msg="Welcome to My-First Restaurant"/>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
.home {
  text-align: center;
}

.restaurant-logo {
  max-width: 30%; /* Justera efter dina behov */
  margin-bottom: 20px;
}

h3 {
  margin-top: 40px;
}
</style>
