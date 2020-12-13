<template>
  <div>
    <header>
      <div class="left-section">
        <img alt="Logo" src="../assets/resize-logo.jpg">
        <h1>YumYumConvo</h1>
      </div>
      <div id="text">
          <router-link to="/" class="btn">Homepage</router-link>
          <router-link to="/profile" class="btn main">Your profile</router-link>
          <router-link to="/blog" class="btn">Explore restaurants</router-link>
        <router-link to="/login" class="blue-btn">Login</router-link>
      </div>
    </header>
    <body>
      <div class="main-rec">
        <div class="left-profile">
          <img class="img2" src="../assets/user profile.svg" alt="User avatar">
          <p class="name"><strong>Jane Doe</strong></p>
          <div class="basic-info">
            <p><strong>Joined on:</strong> 01/01/2020</p>
            <p><strong>Location</strong> San Francisco, CA</p>
            <p><strong>Food preferences:</strong> Vegetarian, Mediterranean</p>
            <p><strong>Email:</strong> janedoe@gmail.com</p>
          </div>
        </div>
      </div>
      <Footer/>
    </body>
  </div>
</template>

<script>
import Footer  from './Footer.vue';

export default {
  name: 'Profile',
  props: {
    msg: String
  },
  components: {
    Footer
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  display: flex;
  flex-direction: row;
  align-items: center;
}

.left-section {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  padding-left: 50px;
  padding-right: 220px;
}

h1 {
  font-family: EB Garamond;
  font-style: normal;
  font-weight: 800;
  font-size: 42px;
  line-height: 55px;

  color: #000000;
  padding-left: 20px;
}

#text {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;

  font-family: EB Garamond;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 26px;

  color: #000000;
}

.btn {
  padding-right: 40px;
}

.blue-btn {
  background-color: #001C55;
  color: white;
  border-radius: 8px;
  padding: 9px 15px 9px 15px;
}

.main {
  font-weight: bold;
}

/*

*/

.img2 {
  width: 170px;
}

.left-profile {
  display: flex;
  flex-direction: column;
  padding: 40px 40px 40px 100px;
}

.name {
  font-family: EB Garamond;
  font-style: normal;
  font-size: 23px;
  line-height: 30px;

  color: #000000;
  padding: 20px 0px 20px 0px;
}

.basic-info {
  width: 300px;
  font-family: EB Garamond;
  font-style: normal;
  font-size: 20px;
  line-height: 30px;

  color: #000000;
}

.main-rec {
  display: flex;
  flex-direction: row;
}

.img3 {
  width: 80vw;
  padding-left: 40px;
}

.img4 {
  width: 80vw;
  padding-top: -5px;
  /* margin-top: -5px; */
}

.img5 {
  width: 70wh;
}

.row {
  display: flex;
  flex-direction: row;
  width: 60vw;
  justify-content: space-between;
  align-items: flex-end;
  font-family: EB Garamond;
  font-style: normal;
  font-weight: bold;
  font-size: 23px;
  line-height: 30px;
  /* color: #FFFFFF; */
  color: #000000;
}
</style>
