<template>
  <v-app class="main">
    <v-main class="d-flex justify-center align-center">
      <HomePage />
    </v-main>
  </v-app>
</template>

<script setup>
import HomePage from "./components/HomePage.vue";
</script>
<style scoped>
.main {
  background-color: hsl(185, 75%, 39%); /* Base background color */
  background-image: url("/src/assets/bg-pattern-top.svg"),
    /* First background image */ url("/src/assets/bg-pattern-bottom.svg"); /* Second background image */
  background-repeat: no-repeat, no-repeat; /* Ensure both images don't repeat */
  background-position: -75% 155%, 150% -110%; /* First image at top-left (0%, 0%), second at bottom-right (100%, 100%) */
  background-size: 70%, 70%; /* First image scales to 100% of container, second scales to 50% */
}


@media screen and (min-width: 600px) and (max-width: 960px) {
  .main {
    background-position: -100% 500%, 150% -550%; /* Adjusted positions */
    background-size: 70%, 70%; /* Adjust size as per the requirement */
  }
}

/* Media query for screen width less than 600px */
@media screen and (max-width: 599px) {
  .main {
    background-position: -110% -10%, 200% 140%; /* Adjusted positions */
    background-size: 80%, 80%; /* Adjust size as per the requirement */
  }
}
</style>