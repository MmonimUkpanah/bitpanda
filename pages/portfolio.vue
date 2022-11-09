<template>
    <div>
      <div>
         <Navbar4/> 
      </div>
      
      <div class="dash">
          <div style="height:2rem">
  
          </div>
          <!-- <div class="movers">
              <div class="movers-top">
                  <h4>Top movers</h4>
              </div>
             <div class="movers-view">
                  <h4>View all assets</h4>
             </div>
          </div>
          <div class="movers-card">
              <div class="movers-cards">
                  <img src="Screenshot1.png" alt="">
              </div>
              <div class="movers-cards">
                  <img src="Screenshot2.png" alt="">
              </div>
              <div class="movers-cards">
                  <img src="Screenshot3.png" alt="">
              </div>
              <div class="movers-cards">
                  <img src="Screenshot4.png" alt="">
              </div>
          </div> -->
          <!-- <hr class="mover-hr"> -->
          <div class="two-factor">
              <div class="two-factor-text">
                <p>Current portfolio value</p>
                  <h4>&#x20AC; 00.00</h4>
                  
              </div>
          </div>
          <!-- <div class="action">
              <div class="action-great">
                  <img src="verifynow.svg" alt="">
                  <h4>Hi Investor, great to see you here!</h4>
                  <p>Once you're ready, please verify your account.</p>
                  <button>Verify now</button>
              </div>
              <div class="action-eye">
                  <h6>Watchlist</h6>
                  <div class="action-eye-center">
                      <img src="list.svg" alt="">
                      <p>Keep an eye on assets by tapping a heart icon wherever you see it or start here.</p>
                      <button>Get Started</button>
                  </div>
              </div>
          </div> -->
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
      .dash{
          background: #f5f5f5;
          height: 120vh;
          margin-top: 2.5rem;
      }
      .movers{
          margin-left: 10rem;
          margin-right: 10rem;
         display: grid;
         grid-template-columns: 1fr 1fr;
      }
      .movers-top h4{
          font-size: 17px;
          font-weight: 600;
      }
      .movers-view h4{
          text-align: right;
          font-size: 17px;
          color: #16a858;
      }
      .movers-card{
          margin-top: 1rem;
          margin-left: 10rem;
          margin-right: 10rem;
          display: grid;
          grid-template-columns: 1fr 1fr 1fr 1fr;
          column-gap: 1rem;
      }
      .movers-cards img{
          width: 100%;
      }
      .mover-hr{
          margin-top: 1.5rem;
          margin-bottom: 1.5rem;
      }
      .two-factor{
          margin-left: 10rem;
          margin-right: 10rem;
          background: white;
          border-radius: 9px;
          padding: 1rem;
      }
      .two-factor-text h4{
          margin-top: 0.5rem;
          margin-bottom: 0.5rem;
          font-size: 50px;
      }
      .two-factor-button button{
          background: white;
          border: 2px solid #16a858;
          padding: 5px 20px;
          color: black;
          border-radius: 5px;
          margin-top: 1rem;
      }
      .action{
          margin-top: 2rem;
          margin-left: 10rem;
          margin-right: 10rem;
          display: grid;
          grid-template-columns: 1.3fr 1fr;
          column-gap: 2rem;
      }
      .action-great{
          background: white;
          padding: 1rem;
          text-align: center;
          border-radius: 9px;
      }
      .action-great h4{
          margin-top: 1rem;
          margin-bottom: 0.5rem;
      }
      .action-great p{
          margin-bottom: 1rem;
      }
      .action-great button{
      margin-bottom: 1rem;
      background: #16a858;
      color: black;
      padding: 0.5rem;
      width: 100%;
      border: none;
      border-radius: 5px;
      margin-top: 1rem;
      }
      .action-eye{
          background: white;
          padding: 1rem;
          border-radius: 9px;
      }
      .action-eye-center{
          text-align: center;
      }
      .action-eye-center p{
          margin-top: 1rem;
          margin-bottom: 1rem;
      }
      .action-eye-center button{
          margin-bottom: 1rem;
      background: white;
      color: black;
      padding: 0.5rem;
      width: 100%;
      border: 2px solid #16a858;
      border-radius: 5px;
      
      }
  
  
      @media(max-width:576px){
          .dash{
          background: #f5f5f5;
          height: auto;
          margin-top: 2.5rem;
      }
          .movers{
          margin-left: 10px;
          margin-right: 10px;
         display: grid;
         grid-template-columns: 1fr 1fr;
      }
      .movers-card{
          margin-top: 1rem;
          margin-left: 10px;
          margin-right: 10px;
          display: grid;
          grid-template-columns: 1fr;
          row-gap: 1rem;
      }
      .two-factor{
          margin-left: 10px;
          margin-right: 10px;
          background: white;
          border-radius: 9px;
          padding: 1rem;
          display: grid;
          text-align: center;
          grid-template-columns: 1fr;
          row-gap: 1rem;
      }
      .action{
          margin-top: 2rem;
          margin-left: 10px;
          margin-right: 10px;
          display: grid;
          grid-template-columns: 1fr;
          row-gap: 1rem;
      }
      }
  
  
  
      @media(min-width:577px) and (max-width:1200px){
          .dash{
          background: #f5f5f5;
          height: auto;
          margin-top: 2.5rem;
      }
          .movers{
          margin-left: 10px;
          margin-right: 10px;
         display: grid;
         grid-template-columns: 1fr 1fr;
      }
      .movers-card{
          margin-top: 1rem;
          margin-left: 10px;
          margin-right: 10px;
          display: grid;
          grid-template-columns: 1fr 1fr ;
          row-gap: 1rem;
      }
      .two-factor{
          margin-left: 10px;
          margin-right: 10px;
          background: white;
          border-radius: 9px;
          padding: 1rem;
          display: grid;
          grid-template-columns: 1fr 3fr 1fr;
      }
      .action{
          margin-top: 2rem;
          margin-left: 10px;
          margin-right: 10px;
          display: grid;
          grid-template-columns: 1fr 1fr;
          row-gap: 1rem;
      }
  
      }
  </style>