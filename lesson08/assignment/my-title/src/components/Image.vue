<template>
  <div>
      <img :src="require(`../assets/${imageName}`)" width=80%>
  </div>
</template>


<script>
export default {
  name: 'image',
  props: ['imageName'],
}
</script>




<!-- <img :src="technique.imgThree" :alt="technique.title" width=80%> -->
