<template>
    <div class="menu">
      <!-- Dishes -->
      <section class="dishes">
        <!-- Dish 1 -->
        <div class="dish">
          <img src="@/assets/pizza.jpg" alt="Pizza">
          <h2>Pizza Margherita</h2>
          <p>Tomato, mozzarella, basil</p>
          <p>$12.99</p>
          <button class="add-to-cart">Add to Cart</button>
        </div>
  
        <!-- Dish 2 -->
        <div class="dish">
          <img src="@/assets/spaghetti.jpg" alt="Spaghetti">
          <h2>Spaghetti Carbonara</h2>
          <p>Eggs, cheese, pancetta</p>
          <p>$14.99</p>
          <button class="add-to-cart">Add to Cart</button>
        </div>
  
        <!-- Add more dishes here -->
        <!-- Dish 3 -->
        <div class="dish">
          <img src="@/assets/dish3.jpg" alt="Dish 3">
          <h2>Dish 3 Name</h2>
          <p>Ingredients for Dish 3</p>
          <p>$15.99</p>
          <button class="add-to-cart">Add to Cart</button>
        </div>
  
        <!-- Dish 4 -->
        <div class="dish">
          <img src="@/assets/dish4.jpg" alt="Dish 4">
          <h2>Dish 4 Name</h2>
          <p>Ingredients for Dish 4</p>
          <p>$16.99</p>
          <button class="add-to-cart">Add to Cart</button>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AboutView',
  }
  </script>
  
  <style scoped>
  /* Menu styles */
  .menu {
    background-color: #f4f4f4;
    padding: 20px;
  }
  
  /* Dishes styles */
  .dishes {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
  }
  
  .dish {
    width: 30%;
    padding: 20px;
    margin: 20px;
    border: 1px solid #ccc;
    text-align: center;
    background-color: #fff;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
  }
  
  /* Button styles */
  button.add-to-cart {
    background-color: #d81e05;
    color: #fff;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  button.add-to-cart:hover {
    background-color: #ff4c32;
  }
  </style>
  