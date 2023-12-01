<template>
    <div class="navbar">
      <div>
          <div class="home.svg"><img src="../assets/Logowelinq.svg"/></div>
          <div class="navigation"> 
            <ul>
              <li>
                <div class="path">
                  <div class="icon"><img src="../assets/home.svg" /></div>
                  <div class="label">Home</div>
                </div>
              </li>
              <li>
                  <div class="path">
                      <div class="icon"><img src="../assets/mysession.png"/></div>
                      <div class="label">My Session</div>
                  </div>
              </li>
                <li>
                    <div class="path active">
                        <div class="icon"><img src="../assets/therapist.png"/></div>
                        <div class="label active">Therapist</div>
                    </div>
                </li>
                <li>
                    <div class="path">
                        <div class="icon"><img src="../assets/quizzes.svg"/></div>
                        <div class="label">Quizzes</div>
                    </div>
                </li>
                <li>
                    <div class="path">
                        <div class="icon"><img src="../assets/webinar.svg"/></div>
                        <div class="label">Webinars</div>
                    </div>
                </li>
                <li>
                    <div class="path">
                        <div class="icon"><img src="../assets/profile.svg"/></div>
                        <div class="label">profile</div>
                    </div>
                </li>
            </ul>
          </div>
          <div class="bottom-img"><img src="../assets/sidebardown.svg"/></div>
      </div>
      <!-- <h1>{{ msg }}</h1> -->
      </div>
  </template>
  
  <script>
  export default {
    name: 'NavBar',
    props: {
      msg: String
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  .navbar{
    background-color: white;
    padding: 20px;
    margin-bottom: 15px;
    margin-right: 20px;
    height: 70%;
    width: 40%;
  }
  .navigation ul{
    display: flex;
    flex-direction: column;
    list-style-type: none;

  }
  .navigation ul li{
    padding: 10px;
  }
  .navigation ul li .path{
    display: flex;
    justify-content: space-between;
  }
  .label{
    padding: 10px;
    flex:2;
    color: #848484;
    font-size: 22px;
    text-align: left;
  }
  .label .active{
    color: white;
  }
  .navigation .active{
    color: white;
    border-radius: 20px;
    background-color: #868CD1;
  }
  .icon{
    width: 44px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  </style>
  