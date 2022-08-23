
<template>
<v-app>
  <div class='headerFooter'> 
    <br>
    <br>
    <img src="./assets/MinuendoLogo.png" height="120" style="margin-top:0px">
    <h2 style="color:white;font-weight: lighter;letter-spacing: 1px;font-family:">Smart Alert</h2>
  </div>
  <div class='mainBody'>
    <p style="margin-right: 295px;margin-top: 80px ;margin-bottom: 0px">E-mail:</p>
    <center><v-text-field style="width:350px;font-size: 15px;" label="E-mail" solo></v-text-field></center>
    <p style="margin-right: 270px;margin-top: 0px ;margin-bottom: 0px">Password:</p>
    <center>
      <v-text-field
          color="red"
          style="width:350px ; font-size: 15px;"
          solo
          v-model="password"
          :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
          :type="showPassword ? 'text' : 'password'"
          name="passwordTextField"
          label="Password"
          @click:append="showPassword = !showPassword">
      </v-text-field>
    </center>
    <u class="forgotPassword">Forgot password?</u>
    <center><v-btn depressed dark large class="rounded-pill" color="red" style="width:350px;margin-top: 30px">Log In</v-btn></center>
  </div>
  <div class='headerFooter'>

  </div>
</v-app>
</template>

<script>
  export default {
    data () {
      return {
        showPassword: false,
      }
    },
  }
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
#app {
  font-family: 'Poppins';
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 0px;
  color:white
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
  text-align:center;
  background-color:#1a2225;
}
.forgotPassword {
  margin-left: 225px;
  margin-top: 0px;
  font-size: 14px;
  cursor: pointer !important;
}
</style>