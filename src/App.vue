<script setup>
import CarComponent from './components/CarComponent.vue'
</script>

<template>
  <main class="main-box">
    <CarComponent class="orangeBack">
      <img src="/src/components/icons/icon-sedans.svg">
      <h1>Sedans</h1>
      <p>Choose a sedan for its affordability and excellent fuel economy.
        Ideal for cruising in the city or on your next road trip.</p>
      <button>Learn More</button>
    </CarComponent>
    <CarComponent class="darkcyanBack">
      <img src="/src/components/icons/icon-suvs.svg">
      <h1>SUVs</h1>
      <p>Take an SUV for its spacious interior, power, and versatility.
        Perfect for your next family vacation and off-road adventures.</p>
      <button>Learn More</button>
    </CarComponent>
    <CarComponent class="verydarkcyanBack">
      <img src="/src/components/icons/icon-luxury.svg">
      <h1>Luxury</h1>
      <p>Cruise in the best car brands without the bloated prices.
        Enjoy the enhanced comfort of a luxury rental and arrive in style.</p>
      <button>Learn More</button>
    </CarComponent>

  </main>
</template>

<style scoped>
.main-box {
  display: flex;
  max-width: 49.5rem;
}

.main-box h1 {
  font-family: 'Big Shoulders';
  text-transform: uppercase;
  color: hsl(0, 0%, 95%);
  margin-top: 25px;
}

.main-box p {
  font-family: 'Lexend Deca';
  font-size: 13px;
  line-height: 1.5rem;
  color: hsla(0, 0%, 100%, 0.75);
  margin-top: 25px;
}

.main-box button {
  width: 120px;
  height: 42px;
  border: none;
  border-radius: 50px;
  font-family: 'Lexend Deca';
  cursor: pointer;
  margin-top: 60px;
}

.main-box button:hover {
  background: transparent;
  color: hsl(0, 0%, 95%);
  border: 2px solid hsl(0, 0%, 95%);
}

.orangeBack button {
  color: hsl(31, 77%, 52%);
}

.darkcyanBack button {
  color: hsl(184, 100%, 22%);
}

.verydarkcyanBack button {
  color: hsl(179, 100%, 13%);
}

@media (max-width: 800px) {
  .main-box {
    flex-direction: column;
    max-width: 40rem;
  }
}
</style>
