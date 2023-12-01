<template>
    <div class="view-profile-container">
      <div class="profile">
        <img src="../assets/home.svg"/>
        <div class="info">
            <div class="details">
                <div class="name">name</div>
                <div class="designation">designation</div>
            </div>
            <button class="view-profile">View Profile</button>
        </div>
    </div>
    <div class="calender">
      I will use any calender library to implement this
    </div>
    <div class="session">
      <div class="period">Sesison Period</div>
      <div class="time">60 min</div>
      <div class="note"><span>Note:</span>*Session period will be of 60min</div>
      
    </div>
    <div class="session">
      <div class="period">Select Time</div>
      <div class="time-format">
        <div class="am"><input name="select-time" type="radio"/>AM</div>
      <div class="pm"><input name="select-time" type="radio"/>PM</div>
    </div>
      <div class="time-options">

        <div>10:00 am</div>
        <div>10:30 am</div>
        <div>11:00 am</div>
        <div>12:00 am</div>
        <div>11:30 am</div>
        <div>12:30 am</div>
      </div>
    </div>
    <button class="book-session">Book Session</button>
  </div>
</template>
  
  <script>


  export default {
    name: 'ViewProfile',
    props: {
      msg: String
    },
  }
  </script>
  

  <style scoped>
  .view-profile-container{
    background-color: white;
    border-radius: 15px;
    margin: 7px;
    display: flex;
    gap: 20px;
    flex-direction: column;
    width: 80%;
    padding: 20px;
  }
.profile{
    display: flex;
    gap: 20px;
    align-items: center;

}
.info{
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.details{
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.profile img{
    border-radius: 50%;
    width: 80px;
}

.view-profile{
  background-color: #868CD1;
  border-radius: 20px;
  padding: 20px;
  border: none;
}

.calender{
  display: flex;
  padding: 20px;
  border: 1px solid #ECEDFF;
}

.session{
  border: 2px solid #C0C5FC;
  padding: 20px;
  border-radius: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 10px
}

.session .period{
  font-weight: 800;
}

.session .time{
  background-color: #ECEDFF;
  padding: 10px;

}
.session .note{
  font-weight: 300;
  color: gray;
}
.session .note span{
  font-weight: 700;
}

.time-format{
  display: flex;
  gap: 10px;
}

.time-options{
  display: flex;
  font-weight: 500;
  flex-wrap: wrap;
  gap: 20px;

  justify-content: center;
  align-items: center;
}
.time-options div{
  padding: 10px 30px;
}

.book-session{
  color: white;
  padding: 20px 30px;
  font-size: 20px;
  border-radius: 20px;
}
  </style>
  