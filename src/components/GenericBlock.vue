<template>
  <h2>{{title}}</h2>
  <p class="date">{{date}}</p>
  <p>{{detail}}</p>
</template>

<script>

export default {
  name: 'GenericBlock',
  props: ['title', 'detail', 'date']
}

</script>

<style scoped>
 p {
   margin-top: 0;
   margin-bottom: 0.5rem;
 }

 h2 {
   font-size: 20px;
   margin: 1rem 0 0 0;
 }

 .date {
   font-style: italic;
 }
</style>