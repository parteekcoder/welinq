<template>

    <div class="Therapy-page">
        <TopBar/>
        <div class="outer-container-right">
            <TherapyListVue />
            <ViewProfile/>
        </div>
    </div>
  </template>
  
<script>

  import ViewProfile from '@/components/ViewProfile.vue';
import TherapyListVue from '../components/TherapyList.vue';
  import TopBar from '../components/TopBar.vue';
  export default {
    name: 'TherapyPage',
    components:{
    TherapyListVue,
    TopBar,
    ViewProfile
}
  }
  </script>
  <style scoped>
  .Therapy-page{
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
 .outer-container-right{
    display: flex;
    justify-content: space-between;
 }
  </style>
  