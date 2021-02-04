<template>
  <h2>Expériences</h2>
  <div v-for="experience in experiences" :key="experience.id">
    <GenericBlock :title="experience.title" :detail="experience.detail" :date="experience.date"/>
  </div>

  <h2>Formations</h2>
  <div v-for="training in trainings" :key="training.id">
    <GenericBlock :title="training.title" :detail="training.detail" :date="training.date"/>
  </div>
</template>

<script>
import data from "../../db.json";
import GenericBlock from './GenericBlock.vue';

export default {
  name: 'RightColumn',
  components: { GenericBlock },
  data() {
    return {
      experiences: data.experiences, 
      trainings: data.trainings
    }
  }
}
</script>

<style scoped>
h2 {
  margin-top: 0;
  border-bottom: 1px solid #2c3e50;
}
</style>
