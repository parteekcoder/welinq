<template>
    <div class="TopBar">
        <!-- <div v-if="loading" class="loading">Loading...</div> -->
        <div class="heading">Therapists</div>
        <div class="utility">
            <div class="settings"><img src="../assets/settings.svg"/></div>
            <div class="search-bar"><input type="text" placeholder="Search for Session"/></div>
            <div class="notification"><img src="../assets/notify.svg"/></div>
            <div class="profile"><img src="../assets/home.svg"/></div>
        </div>
    </div>
</template>
  
<script>

// import TherapistCard from './TherapistCard.vue'
export default {
    components:{
        // TherapistCard
    },
    props:{
        
    },
    name: 'TopBar',
}


</script>

<style scoped>
.TopBar{
    display: flex;
    justify-content: space-between;
    padding: 20px;
    align-items: center;
}
.heading{
    font-size: 50px;
    font-weight: 700;
}
.TopBar .utility{
    padding: 20px;
    display: flex;
    justify-content: end;
    align-items: center;
    gap: 0 70px;
    width: 70%;
}
.TopBar .utility img{
    width: 40px;
}

.search-bar input{
    padding: 20px;
    border: none;
    width: 400px;
    border-radius: 20px;
}

.settings{
    padding: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    border-radius: 50%;
    overflow: hidden;
}

.settings img{
    width: 30px;
    height: 30px;
}

.notification{
    background-color: #868CD1;
    border-radius: 50%;
    padding: 15px;
}

.notification img{
    width: 30px;
    height: 30px;
}

.profile{
    border-radius: 50%;
    padding: 10px;
}
</style>
  
