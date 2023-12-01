<template>
    <div class="therapist-card">
        <div class="profile-pic"><img :src='data.photoUrl'/></div>
        <div class="prize">{{data.hourlyRate}} $/hr</div>
        <div style="font-weight: 900;font-size: 20px;">{{ data?.firstname? data?.firstname: data?.nickname}}  <img v-if="data.isApproved" src="../assets/approve.svg"/></div>
        <div style="font-size: 13px;color: blue;font-weight: 200;">Last active 10min ago</div>
        <div>{{data.expertExperience}}yrs of experience</div>
        <div><span v-for="item in data.expertFocusArea" :key="item.id" >{{ item }},</span></div>
        <div>Dialect behaviours</div>
        <div class="book-session-chat">
            <button class="book-session">Book Session</button>
            <button class="chat">chat</button>
        </div>
    </div>
  </template>
  
  <script>
  export default {
      name: 'TherapistCard',
      props: {
          data: Object
        }
    }
  </script>
<style scoped>
.therapist-card{
    border-radius: 10px;
    background-color: white;
    margin: 8px;
    display: inline-block;
    width: 30%;
    padding: 15px 50px;
    text-align: center;
    font-weight: 600;
}
.therapist-card div{
    margin: 5px 0;
}

.prize{
    color: #EB7856;
    font-weight: 600;
}

.profile-pic {
    overflow: hidden;
}
.profile-pic img{
    width: 40px;
    border-radius: 50px;
    height: 50px;
}
.book-session-chat{
    margin-left: 15px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.book-session{
    background-color: #E5E7FF;
    border-radius: 10px;
    padding: 13px 10px;

}

.chat{
    border-radius: 50%;
    background-color: #CCF4DA;
    padding: 10px;
}
</style>