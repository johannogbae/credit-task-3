<template>
    <div class="reservation">
      <!-- Reservation Form -->
      <section class="reservation-form">
        <h2>Make a Reservation</h2>
        <form @submit.prevent="submitReservation">
          <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" v-model="reservationData.name" required>
          </div>
          <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" v-model="reservationData.email" required>
          </div>
          <div class="form-group">
            <label for="date">Date:</label>
            <input type="date" id="date" v-model="reservationData.date" required>
          </div>
          <div class="form-group">
            <label for="time">Time:</label>
            <input type="time" id="time" v-model="reservationData.time" required>
          </div>
          <button type="submit">Submit</button>
        </form>
      </section>
  
      <!-- Confirmation Message (Optional) -->
      <section v-if="reservationSubmitted" class="confirmation">
        <p>Thank you, {{ reservationData.name }}! Your reservation for {{ reservationData.date }} at {{ reservationData.time }} has been confirmed.</p>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ReservationView',
    data() {
      return {
        reservationData: {
          name: '',
          email: '',
          date: '',
          time: ''
        },
        reservationSubmitted: false
      };
    },
    methods: {
      submitReservation() {
        // You can implement the reservation submission logic here
        // For demonstration purposes, we'll just show a confirmation message
        this.reservationSubmitted = true;
      }
    }
  };
  </script>
  
  <style scoped>
  /* Reservation Form styles (you can add more styling as needed) */
  .reservation-form {
    background-color: #fff;
    padding: 20px;
    border: 1px solid #ccc;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    max-width: 400px;
    margin: 0 auto;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    font-weight: bold;
  }
  
  input[type="text"],
  input[type="email"],
  input[type="date"],
  input[type="time"] {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
  }
  
  button[type="submit"] {
    background-color: #d81e05;
    color: #fff;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 1.2rem;
    transition: background-color 0.3s;
  }
  
  button[type="submit"]:hover {
    background-color: #ff4c32;
  }
  
  /* Confirmation Message styles (you can customize this as well) */
  .confirmation {
    background-color: #d81e05;
    color: #fff;
    padding: 20px;
    text-align: center;
    max-width: 400px;
    margin: 0 auto;
  }
  </style>
  