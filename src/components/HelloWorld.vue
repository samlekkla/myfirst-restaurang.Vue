<template>
  <div class="home">
    <h1>{{ restaurantName }}</h1>
    <p>
      Welcome to My-First Restaurant, where we serve delicious dishes with love and care. Explore our menu below or contact us to make a reservation.
    </p>
    <h3>Menu</h3>
    <ul>
      <li>Check out our menu</li>
    </ul>
    <h3>Contact</h3>
    <ul>
      <li>Contact us</li>
      <li>Call us: +123 456 789</li>
    </ul>
    <h3>Follow Us</h3>
    <ul>
      <li>Instagram</li>
      <li>Facebook</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  data() {
    return {
      restaurantName: 'My-First Restaurant',
    };
  },
};
</script>

<!-- Scoped styles specific to this component -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
  color: #73d3f0;
}
</style>
