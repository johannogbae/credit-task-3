<template>
    <header>
      <h1>Welcome to Italiano Delights</h1>
      <p>Explore the flavors of Italy</p>
    </header>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/menu">Menu</router-link></li>
        <li><router-link to="/reservation">Reservation</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
      </ul>
    </nav>
  </template>
  
  <script>
  export default {
    name: 'Header',
  }
  </script>
  
  <style scoped>
  /* Header styles */
  header {
    background-color: #d81e05;
    color: #fff;
    text-align: center;
    padding: 20px;
  }
  
  nav ul {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 10px;
  }
  
  nav ul li {
    display: inline;
    margin: 0 20px;
  }
  
  </style>
  