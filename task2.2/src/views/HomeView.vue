<template>
  <div class="home">
    <!-- Restaurant Information -->
    <section class="restaurant-info">
      <h3 class="restaurant-description">
        Welcome to Italiano Delights. We offer a delightful culinary experience
        that brings the flavors of Italy to your plate. Our dishes are prepared
        with love and the finest ingredients to satisfy your taste buds.
      </h3>
    </section>

    <!-- Button to View Menu -->
    <router-link to="/menu">
      <button class="cta-button">View Menu</button>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
}
</script>

<style scoped>
/* Home Page styles */
.home {
  background-image: url('@/assets/images/bg.jpg');
  background-size: cover;
  background-position: center;
  text-align: center;
  padding: 100px 0;
  color: #fff; /* Set text color to white for visibility */
}

/* Restaurant Description styles */
.restaurant-description {
  font-size: 1.2rem;
  margin-top: 20px;
  background-color: rgba(0, 0, 0, 0.5); /* Add background color with transparency */
  padding: 150px;
  border-radius: 5px;
}

/* Button styles */
button.cta-button {
  background-color: #d81e05;
  color: #fff;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  font-size: 1.2rem;
  transition: background-color 0.3s;
  margin-top: 20px;
}

button.cta-button:hover {
  background-color: #ff4c32;
}
</style>
