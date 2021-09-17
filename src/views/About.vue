<template>
  <div id="login" class="login">
      <h3>{{ compantName }}</h3><br>
      <h4 class="desc">{{desc}}</h4>
      <p class="pass">{{pass}}</p><br>
      <div class="form">
        <b-form>
            <div>
                <label for="text-email">Email</label>
                <b-form-input type="email" id="text-email" aria-describedby="email-help-block"></b-form-input>
            </div><br>
            <div>
                <label for="text-password">Password</label>
                <b-form-input type="password" id="text-password" aria-describedby="password-help-block"></b-form-input>
            </div><br><br>

            <b-button variant="outline-primary" class="loginme">Sign up</b-button>
            <p class="or">or</p>
            <b-button variant="outline-danger" class="loginme"><b-icon icon="google" aria-hidden="true"></b-icon> Sign up with google</b-button>
            <p class="signup">Already have an account? <router-link to="/" class="signupT">Log in</router-link></p>
        </b-form>
      </div>
  </div>
</template>

<script>
export default {
    name:"login",
    data(){
        return{
            compantName:"Diamond Plus",
            desc: "Sign up",
            pass: "Enter your email and password"
        }
    }
}
</script>

<style scoped>
.desc{
    font-size: 30px;
    text-align: left;
    color: black;
}

.pass{
    text-align: left;
    color: gray;
}

.form{
    text-align: left;
}

.me{
    margin-left: 10px;
}

.loginme{
    width: 100%
}

.or{
    text-align: center;
    margin-top: 10px;
    font-size: 17px;
    color: gray;
}

.signup{
    margin-top: 10px;
}

.signupT{
    font-weight: normal;
    color: #1b85f0;
    text-decoration: none;
}
</style>