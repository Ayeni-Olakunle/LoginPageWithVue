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
                <p class="right"><a href="#" class="rightT">Forget Password?</a></p>
            </div>

            <b-form-checkbox>
            <p class="me">Remember me</p>
            </b-form-checkbox>
            <b-button variant="outline-primary" class="loginme">Login now</b-button>
            <p class="or">or</p>
            <b-button variant="outline-danger" class="loginme"><b-icon icon="google" aria-hidden="true"></b-icon> Sign in with google</b-button>
            <p class="signup">Don't have an account?<router-link to="/signup" class="signupT">Sign up</router-link></p>
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
            desc: "Login to your account",
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

.right{
    text-align: right;
    color: #1b85f0;
    text-decoration: none;
}
.rightT{
    color: #1b85f0 !important;
    text-decoration: none !important;
    font-weight: normal !important;
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
    margin-top: 10px !important;
}

.signupT{
    font-weight: normal !important;
    color: #1b85f0 !important;
    text-decoration: none !important;
    margin-left: 5px !important;
}
</style>