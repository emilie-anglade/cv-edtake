<template>
  <div class="general-container">
    <img :src="img" alt="profile pic"/>
    <div class="general-info-container">
      <h2>{{ title }}</h2>
      <h3>{{ name }}</h3>
      <h4>{{ city }}</h4>
      <h4>{{ mail }}</h4>
      <h4>{{ tel }}</h4>
      <h4>{{ github }}</h4>
    </div>
  </div>
</template>

<script>
import profile_pic from '../assets/profilepic.png';

export default {
  name: 'GeneralInformations',
  data() {
    return{
      img: profile_pic
    }
  },
  props: ['title', 'name', 'city', 'mail', 'tel', 'github']
}
</script>

<style scoped>
.general-container {
  display: flex;
  flex-direction: column;
}
.general-info-container {
  
  border-bottom: 1px solid whitesmoke;
}

.general-info-container h2, h3, h4 {
  margin: 0 0 1rem 0;
}

h2, h3 {
  font-style: italic;
}

h4 {
  font-weight: normal;
}

img {
  width: 50%;
  margin: 0 auto 1rem auto;
  border-radius: 20%;
  
}
</style>