<template>
    <div class="Therapy-list">

        <ul v-if="apiData">
        <TherapistCard v-for="item in apiData" :key="item.id" :data="item" />
        </ul>
        <p v-else>Loading...</p>
</div>
</template>
  
<script>

import TherapistCard from './TherapistCard.vue'
import axios from 'axios'
export default {
    data() {
    return {
      apiData: null,
    };
  },
    components:{
        TherapistCard
    },
    props:{
        
    },
    mounted() {
    const apiUrl = 'https://api-container-ph3rhhnyiq-uc.a.run.app/therapists';

    axios.get(apiUrl)
      .then((response) => {
        this.apiData = response.data;
      })
      .catch((error) => {
        console.log('Error fetching data:', error);
      });
  },
    name: 'TherapyListVue',
}


</script>

<style scoped>
.Therapy-list{
    display: flex;
    align-items: stretch;
    justify-content: stretch;
}
</style>
  
