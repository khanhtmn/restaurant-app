<template>
  <div>
    <header>
      <div class="left-section">
        <img alt="Logo" src="../assets/resize-logo.jpg">
        <h1>YumYumConvo</h1>
      </div>
      <div id="text">
          <router-link to="/" class="btn">Homepage</router-link>
          <router-link to="/profile" class="btn">Your profile</router-link>
          <router-link to="/blog" class="btn main">Explore restaurants</router-link>
        <router-link to="/login" class="blue-btn">Login</router-link>
      </div>
    </header>
    <body>
      <div class="photo">
        <div class="blog-photo">
          <img src="../assets/pexels-igor-starkov.svg" alt="image">
          <p style="margin: 20px 10px 0px 10px;">Tranquil Restaurant at Serene Street</p>
        </div>
        <div class="blog-photo">
          <img src="../assets/pexels-chan-walrus.svg" alt="image">
          <p style="margin: 20px 10px 0px 10px;">Home Meal Restaurant at 8th Street</p>
        </div>
        <div class="blog-photo">
          <img src="../assets/pexels-lisa-fotios.svg" alt="image">
          <p style="margin: 20px 10px 0px 10px;">Pasta Paradise at Italian Town</p>
        </div>
      </div>
      <div class="photo">
        <div class="blog-photo">
          <img src="../assets/pexels-elevate.png" alt="image">
          <p style="color: white">Mushroom Party at King Street</p>
        </div>
        <div class="blog-photo">
          <img src="../assets/pexels-quang-nguyen-vinh.png" alt="image">
          <p style="color: white">Brunch at co-working cafe</p>
        </div>
        <div class="blog-photo">
          <img src="../assets/pexels-christel-jensen.svg" alt="image">
          <p style="color: white">Japanese fusion at Turk Street</p>
        </div>
      </div>
      <Footer/>
    </body>
  </div>
</template>

<script>
import Footer  from './Footer.vue';

export default {
  name: 'Blog',
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

.photo {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.blog-photo {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: #FFFFFF;
  border: 1px solid #0138A7;
  box-sizing: border-box;
  border-radius: 0px 0px 10px 10px;
  /* margin-bottom: 50px; */
  padding-bottom: 20px;
  margin-top: 50px;
}

</style>
