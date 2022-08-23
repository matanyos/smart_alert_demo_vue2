@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap");
<template>
<v-app>
  <div class='headerFooter'> 
    <img src="./assets/MinuendoLogo.png" height="120" style="margin-top:80px">
    <h2 style="color:white;font-weight: lighter;letter-spacing: 3px;font-family:">Smart Alert</h2>
  </div>
  <div class='mainBody' style="text-align:center">
    <p style="margin-right: 244px;" class="white--text">E-mail:</p>
          <v-text-field class="centered-input text--darken-3 mt-3" style="width:300px"  label="E-mail:" solo dense></v-text-field>
    <v-btn depressed dark large class="rounded-pill" color="red" style="width:300px">Log In</v-btn>
  </div>
  <div class='headerFooter'>

  </div>
</v-app>
</template>

<script>


</script>


<style>
#app {
    font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 0px;
}

body {
  margin: 0;
}
.headerFooter {
  min-height: 25vh; 
  background-color:#1a2225
}

.mainBody {
  min-height: 50vh;
  background-color:#1a2225;
}
.centered-input input {
  text-align: center
}
</style>