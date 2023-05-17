<script setup>
import TheWelcome from './components/TheWelcome.vue'
import LeftHome from './components/HomeLeft.vue'
import TheMap from './components/MapView.vue'
</script>

<template>
  <LeftHome />
 
  <main class="rightPanel">
    <TheMap />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}
.rightPanel{
  background-image: url("./assets/indiaMap.png");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  display: flex;
  place-items: center;
  background-color:rgba(0,0,0,0.5);
  flex: 1 1 auto;
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
