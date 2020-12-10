<!-- HTML goes here -->
<template>
  <div class="home">
    <Intro msg="EGGS ALL DAY"/>
  </div>
</template>


<!-- Javascript goes here -->
<script>
// @ is an alias to /src
import Intro from '@/components/Intro.vue'

export default {
  name: 'Home',
  components: {
    Intro
  }
}
</script>


<!-- CSS goes here -->
