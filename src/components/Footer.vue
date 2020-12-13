<template>
  <div>
    <footer>
      <div class="main">
        <div class="logo-left">
          <img alt="Logo" src="../assets/resize-logo.jpg">
          <div class="section-left">
            <h3>YumYumConvo</h3>
            <p>Find a companion for your next dining experience</p>
            <p>©2020 YumYumConvo</p>
          </div>
        </div>
        <div class="section-right">
          <div class="contact">Contact & Support</div>
          <div class="info">
            <p>Email: hello@yumyumconvo.com</p>
            <p>Hotline: (555) 555-5555</p>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img {
  height: 50px;
  padding-top: 15px;
  padding-right: 10px;
}

.section-left {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin: 0px 20px 20px 0px;
}

.logo-left {
  display: flex;
  flex-direction: row;
  padding-left: 60px;
}

.section-right {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  padding: 20px 60px 0px 0px;
}

.contact {
  font-family: EB Garamond;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 23px;
  color: #000000;
  margin-bottom: 10px;
}

.info {
  font-family: EB Garamond;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 23px;
  color: #000000;
  margin: 0 20px 20px 0px;
  text-align: left;
}

p {
  margin: 0px 0px 0px 0px;
  padding-bottom: 10px;
}

h3 {
  font-size: 24px;
  margin-bottom: 15px;
}

.main {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
