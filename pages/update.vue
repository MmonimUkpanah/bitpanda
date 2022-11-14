<template>
  <div>
    <div>
        <Navbar4/>
    </div>
    <div class="update">
        <div style="height:3rem">

        </div>
        <div class="update-form">
            <div class="update-form-title">
                <h3>Update Profile</h3>
            </div>
          <form  method="post" @submit.prevent="updateDetails()">
            <label for="">Date of birth</label>
            <input type="date" required name="" id="" v-model="updateInfo.dob">
            <label for="">Address</label>
            <input type="text" required v-model="updateInfo.address">
            <label for="">Postal code</label>
            <input type="number" required name="" id="" v-model="updateInfo.postal_code">
            <label for="">City</label>
            <input type="text" required v-model="updateInfo.city">
            <label for="">Country</label>
            <input type="text" required v-model="updateInfo.country">
            <label for="">Area code</label>
            <input type="text" required v-model="updateInfo.area_code">
            <label for="">Phone Number</label>
            <input type="text" required v-model="updateInfo.phone">
            <button type="submit">Update</button>
          </form>
        </div>
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
    data(){
        return{
            updateInfo:{
                dob:'',
                address:'',
                postal_code:null,
                city:'',
                country:'',
                area_code:'',
                phone:''
            },
            baseUrl: "https://paybay-invest.herokuapp.com/api/",
        }
    },
    methods: {
    async updateDetails() {
      try {
        const response = await this.$axios.post(this.baseUrl + "update-profile/",this.updateInfo);
        this.$message({
            message: "Profile Updated",
            type: "success",
            });
        console.log(response.data);
        this.updateInfo= {}
      } catch (error) {
        console.error(error);
      }
    },
  },
}
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
    .update{
        background: #f5f5f5;
        height: 100vh;
        margin-top: 2.4rem;
    }
    .update-form-title, h3{
        text-align: center;
        color: #16a858;
    }
    .update-form{
        width: 30%;
        margin: auto;
        height: auto;
        background: white;
        border-radius: 9px;
        padding: 1rem;
    }
    .update-form label{
        display: block;
    }
    .update-form input{
        display: block;
        width: 100%;
        margin-bottom: 0.5rem;
    }
    .update-form button{
        display: block;
        width: 100%;
        background: #16a858;
        color: white;
        border: none;
        border-radius: 5px;
        padding: 0.5rem;
        margin-top:1rem ;
    }



    @media(max-width: 576px){
        .update-form{
        width: 100%;
        margin: auto;
        height: auto;
        background: white;
        border-radius: 9px;
        padding: 1rem 10px;
    }
    }


    @media(min-width:577px) and (max-width:1200px){
        .update-form{
        width: 50%;
        margin: auto;
        height: auto;
        background: white;
        border-radius: 9px;
        padding: 1rem 10px;
    }
    }
</style>