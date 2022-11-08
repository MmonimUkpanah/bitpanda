<template>
    <div>
      <Navbar3/>
      <div class="login">
        <h3>Create your Bitpanda account</h3>
        <form action="">
            <div class="name">
                <input type="text" placeholder="First Name"> <input type="text" placeholder="Last Name">
            </div>
          
          <input type="email" placeholder="Email">
          <input type="password" name="" id="" >
          <input type="text" placeholder="Country of Residence">
          <button class="login-button">Create Account</button>
          <button class="account-button">Already have an account?</button>
          <div class="confirm">
            <p class="resend">Looking to open a business account? Sign up here</p>
          </div>
          
        </form>
      </div>
    </div>
  </template>
  
  <script>
  export default {
  
  }
  </script>
  
  <style scoped>
    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
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
      border-color: 0.5px solid initial;
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