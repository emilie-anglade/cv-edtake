<template>
  <div class="cv-container">
    <div class="left-container">
      <LeftColumn />
    </div>
    <div class="right-container">
      <RightColumn />
    </div>
  </div>
</template>

<script>
import LeftColumn from './LeftColumn.vue';
import RightColumn from './RightColumn.vue';


export default {
  name: 'CV',
  components: { LeftColumn, RightColumn }
}
</script>


<style>
  .cv-container {
    background-color: rgb(236, 232, 232);
    display: flex;
    flex-wrap: wrap;
    margin: 0 auto;
    padding: 0;
    max-width: 870px;
  }
  .left-container {
    flex: 2;
    background-color: rgb(177, 106, 106);
    padding: 2rem;
  }
  .right-container {
    flex: 3;
    padding: 2rem;
  }
</style>