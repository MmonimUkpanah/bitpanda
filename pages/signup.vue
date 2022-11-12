<template>
    <div>
      <Navbar3/>
      <div class="login">
        <h3>Create your Pay Bay Invest account</h3>
        <form method="post" @submit.prevent="signUp">
            <div class="name">
                <input type="text" required placeholder="First Name" v-model="signupinfo.first_name"> <input type="text" required placeholder="Last Name" v-model="signupinfo.surname">
            </div>
          
          <input type="email" placeholder="Email" required v-model="signupinfo.email">
          <select class="form-select" aria-label="Default select example" v-model="signupinfo.stage">
          <option selected >Stage</option>
          <option value="Promo">Promo</option>
          <option value="Gold">Gold</option>
          <option value="Silver">Silver</option>
          <option value="Platinum">Platinum</option>
        </select>
          <input type="password" name="" id="" required placeholder="password"  v-model="signupinfo.password">
          <input type="password" name="" id="" required placeholder="confirm password"  v-model="signupinfo.password2">
          <button type="submit" class="login-button">Create Account</button>
          <span class="account-button">Already have an account?</span>
          <div class="confirm">
            <p class="resend">Looking to open a business account? Sign up here</p>
          </div>
          
        </form>
      </div>
    </div>
  </template>
  
  <script>
  import ElementUI from "element-ui";
  import "element-ui/lib/theme-chalk/index.css";
  export default {
    components: {
      ElementUI,
    },
    data() {
      return {
        baseUrl: "https://paybay-invest.herokuapp.com/api/",
        signupinfo:{
            email:'',
            first_name:'',
            surname:'',
            password:'',
            password2:'',
            profile_value: 120000,
            stage:""
        }
      };
    },
    methods: {
      async signUp() {
        try {
          const response = await this.$axios.post(
            this.baseUrl + "register/",
            this.signupinfo
          )
          this.$router.push("/login")
          this.$message({
            message: "Account created successfully!",
            type: "success",
            });
          console.log(response);
        } catch (error) {
          console.log(error);
          this.$message({
            message: error.response.data,
            type: "warning",
            });
        } finally {
          this.signupinfo = {};
        }
      },
      
    },
  
    mounted() {
      
    },
  };
  </script>
  
  <style scoped>
    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    select{
      width: 100%;
      display: block;
      background-color: transparent;
      color: rgba(0, 0, 0, 0.87);
      padding: 10px 10px 10px;
      border-radius: 3px;
      border: 0.5px solid initial;
      margin-bottom: 1rem;
    }
    .login{
      width: 40%;
      margin-left: auto;
      margin-right: auto;
      margin-top: 5rem;
      margin-bottom: 10rem;
    }
    .login h3{
      font-size: 23px;
      font-weight: 500;
      margin-bottom: 30px;
    }
    .login input{
      display: block;
      width: 100%;
      background-color: transparent;
      color: rgba(0, 0, 0, 0.87);
      padding: 10px 10px 10px;
      border-radius: 3px;
      border: 0.5px solid initial;
      margin-bottom: 1rem;
    }
    .login label{
      color: rgb(66, 66, 66);
      display: inline-block;
      font-size: 13px;
      font-weight: 600;
      line-height: 1.15384em;
      margin-bottom: 6px;
    }
    .login button{
      display: block;
      width: 100%;
    }
    .login-button{
      background-color: rgb(39, 209, 127);
      border: none;
      border-radius: 3px;
      color: rgb(28, 28, 30);
      font-weight: 600;
      padding: 5px 0px;
      margin-top: 1rem;
      margin-bottom: 1rem;
    }
    .account-button{
      color: rgb(28, 28, 30);
      background-color: rgb(255, 255, 255) !important;
      border-width: 2px;
      border-style: solid;
      padding: 5px 0;
      border-color: rgb(39, 209, 127);
      display: block;
      text-align: center;
    }
    .confirm{
      text-align: center;
      margin-top: 1rem;
    }
    .confirm p{
      color: #333333;
      font-size: 15px;
    }
    .resend{
      color: rgb(0, 128, 79) !important;
    }
    .name{
        display: grid;
        grid-template-columns: 1fr 1fr;
        column-gap: 1rem;
    }
  
  
  
    @media(max-width:576px){
      .login{
      width: 100%;
      padding-right: 10px !important;
      padding-left: 10px;
      /* margin-left: 10px;
      margin-right: 10px; */
      margin-top: 5rem;
      margin-bottom: 10rem;
    }
    }
  
  
  
  
    @media(min-width:577px) and (max-width:1200px){
      .login{
      width: 50%;
      padding-right: 10px !important;
      padding-left: 10px;
      /* margin-left: 10px;
      margin-right: 10px; */
      margin-top: 5rem;
      margin-bottom: 10rem;
    }
    }
  </style>