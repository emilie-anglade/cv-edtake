<template>
  
  <GeneralInformations :title="general.title" :name="general.name" :city="general.city" :mail="general.mail" :tel="general.tel" :github="general.github"/>
  
  <div v-for="skill in skills" :key="skill.id">
    <GenericBlock :title="skill.title" :detail="skill.detail"/>
  </div>
  
</template>

<script>
import data from "../../db.json";
import GeneralInformations from './GeneralInformations.vue';
import GenericBlock from './GenericBlock.vue';

export default {
  name: 'LeftColumn',
  components: { GenericBlock, GeneralInformations },
  data() {
    return {
      general: data.general, 
      skills: data.skills
    }
  }
}
</script>
