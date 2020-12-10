<!-- HTML goes here -->
<template>
  <div class="intro">
    <h1>{{ msg }}</h1>
    <p>Eggs are a great, inexpensive source of protein, and one of the few foods
      that naturally offer vitamin D. They're also incredibly versatile. So, why only eat them for breakfast?
      Check out some ideas for making eggs part of your meal any time of day.</p>
    <img src="../assets/egg-bkgrd.jpg" width=100% alt="Close-up of eggs scattered on a surface">
  </div>
</template>

<!-- Javascript goes here -->
<script>
export default {
  name: 'Intro',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only
<style scoped>
</style>
-->
