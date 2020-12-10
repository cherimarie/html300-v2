<template>
  <div>
      <img :src="source" width=80%>
  </div>
</template>


<script>
export default {
  name: 'Image',
  props: ['source'],
}
</script>




<!-- <img :src="technique.imgThree" :alt="technique.title" width=80%> -->
