<template>
  <div>
    <Navbar/>
    <div class="header">
      <div class="header-left">
        <h1>Invest in what you believe in </h1>
        <button>Start Investing</button>
      </div>
      <div class="header-right">
        <div class="header-img">
          <img src="/Hero.png" alt="hero-image">
        </div>
        <div class="header-text">
          <div class="header-text-one">
            <div class="header-text-img">
              <img src="/btc.svg" alt="">
            </div>
            <div class="header-text-first">
              <h5>Bitcoin</h5>
              <p>21,356.96</p>
            </div>
            <div class="header-text-second">
              <h5>+2.87%</h5>
              <p>595.84</p>
            </div>
          </div>
          <div class="header-text-one">
            <div class="header-text-img">
              <img src="/tsla.svg" alt="">
            </div>
            <div class="header-text-first">
              <h5>Tesla</h5>
              <p>223.20</p>
            </div>
            <div class="header-text-second">
              <h5>+1.98%</h5>
              <p>4.33</p>
            </div>
          </div>
          <div class="header-text-one">
            <div class="header-text-img">
              <img src="/xau.svg" alt="">
            </div>
            <div class="header-text-first">
              <h5>Gold</h5>
              <p>54.18</p>
            </div>
            <div class="header-text-second">
              <h5>+1.34%</h5>
              <p>0.72</p>
            </div>
          </div>
          <div class="header-summary">
            <p>Past performance is no indication of future performance.</p>
          </div>
          
        </div>
      </div>
    </div>
    <div class="reg">
      <div class="reg1">
        <img src="/Regulated.svg" alt="">
        <div class="reg-text">
          <h2>Regulated</h2>
        <p><span class="focused">MiFID II</span>  investment firm.
        </p>
        <p> <span class="focused">PSD2</span> payment institution.</p>

        <a href="">View licences</a>
        </div>
        
      </div>
      <div class="reg1">
        <img src="/Secure.svg" alt="">
        <div class="reg-text">
          <h2>Secure</h2>
          <p><span class="focused">Fully compliant with</span> AML5.
          </p>
          <p>Funds secured in offline wallets.</p>

          <a href="">Read more</a>
        </div>
        
      </div>
      <div class="reg2">
        <img src="/Trusted.svg" alt="">
        <div class="reg-text">
          <h2>Trusted</h2>
          <p><span class="focused"> 3.5+ million</span> happy users.
          </p>
          <p>Excellent Trustpilot rating.</p>

          <a href="">Read reviews.</a>
        </div>
        
      </div>
      
    </div>
    <hr class="invest-hr">
    <div class="invest">
      
      <div class="invest-header">
        <h4>INVEST</h4>
        <h2>All your investments.</h2>
        <h2>All on Bitpanda.</h2>
      </div>
      <div class="invest-grid">
        <div class="invest-options">
          <h4>Cryptocurrencies</h4>
          <p>Buy, sell and swap the cryptocurrencies you want anytime, anywhere</p>
          <img class="crypto-img" src="crypto.png" alt="">
        </div>
        <div class="invest-options">
          <h4>Stocks*</h4>
          <p>Invest in fractions of your favorite companies without committing to a whole share</p>
          <img src="stocks.png" alt="">
        </div>
        <div class="invest-options">
          <h4>ETFs*</h4>
          <p>Invest in fractions of your favorite ETFs* without committing to a whole share</p>
          <img class="crypto-img" src="ETFs.png" alt="">
        </div>
        <div class="invest-options invest-bottom">
          <h4>Commodities*</h4>
          <p>Fortify your portfolio with commodities* and shield it against inflation.</p>
        </div>
        <div class="invest-options invest-bottom">
          <h4>Crypto Indices</h4>
          <p>Auto-invest in the whole crypto market with a single click.</p>
        </div>
        <div class="invest-options invest-bottom">
          <h4>Precious Metals</h4>
          <p>Diversify your portfolio by invrsting in physically-backed precious metals.</p>
        </div>
      </div>
    </div>

    <!-- carousels -->
    <div class="features">
      
    </div>
  </div>
  
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style scoped>
  .header{
    margin-left: 5rem;
    margin-right: 5rem;
    margin-top: 5rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
}
  .header-left h1{
    font-size: 58px;
    font-weight: 600;
    padding-right: 10rem;
    margin-top: 12rem;
  }
  .header-left button{
    background-color: #27d17f;
    border: 1px solid #27d17f;
    color: #fff;
    border-radius: 9px;
    padding: 14px 40px;
    margin-top: 1rem;
  }
  .header-img{
    text-align: right;
  } 
  .header-right img{
    width: 80%;
    border-radius: 9px;
  }
  .header-text{
    margin-top: -30rem;
  }
  .header-text-one{
    width: 40%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 1rem;
    background: #f5f5f58a 0 0 no-repeat padding-box;
    border: 1px solid #ebebeb;
    border-radius: 10px;
    box-shadow: 0 0 7px #0000000c;
    padding: 14px 20px;
    margin-bottom: 1rem;
    z-index: 5;
    position: relative;
  }
  .header-text-img img{
    height: 40px;
    width: 40px;
  }
  .header-text-first h5{
    color: #282828;
    font-size: 17px;
    font-weight: 600;
  }
  .header-text-first p{
    color: #282828;
    font-size: 12px;
    font-weight: 600;
  }
  .header-text-second h5{
    color: #00804f;
    font-size: 17px;
    font-weight: 600;
  }
  .header-text-second p{
    color: #00804f;
    font-size: 12px;
    font-weight: 600;
  }
  .header-summary{
    margin-top: 11rem;
    text-align: right;
    color: #000000B3;
  }
  .header-summary p{
    font-size: 19px;
  }
  .reg{
    margin-left: 5rem;
    margin-right: 5rem;
    margin-top: 5rem;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 2rem;
  }
  .reg1{
    border-right: 1px solid rgb(225, 227, 230);
  }
  /* .reg1 img,.reg2 img{
    height: 60px;
    width: 60px;
  } */
  .reg1 h2,.reg2 h2{
    font-size: 27px;
    font-weight: 600;
    margin-top: 15px;
    margin-bottom: 15px;
  }
  .focused{
    font-weight: 600;
  }
  .reg1 a, .reg2 a{
    color: rgba(0,0,0,.7);
    font-weight: 600;
    border-bottom:  2px solid #27d17f;
  }
  .reg1 a:hover, .reg2 a:hover{
    color: #27d17f;
  }
  .invest-hr{
    margin-top: 7rem;
    margin-bottom: 7rem;
  }
  .invest{
    margin-left: 5rem;
    margin-right: 5rem;
  }
  .invest-header{
    text-align: center;
  }
  .invest-header h4{
    color: #8b8b8b;
    font-size: 18px;
    margin-bottom: 1.5rem;
    font-weight: 600;
  }
  .invest-header h2{
    font-size: 45px;
    font-weight: 600;
  }
  .invest-grid{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 1rem;
    row-gap: 1rem;
  }
  .invest-options{
    background-color: #f5f5f5;
    padding: 30px 30px 0px 30px;
    border-radius: 9px;
  }
  .invest-options h4{
    font-size: 35px;
    font-weight: 600;
  }
  .invest-options p{
    font-weight: 500;
  }
  .invest-options img{
    width: 100%;
    height: fit-content;
  }
  .crypto-img{
    margin-top: 1.5rem;
  }
  .invest-bottom{
    padding-bottom: 20px;
  }



  @media (max-width:576px) {
    .header{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 2rem;
}
.header-left h1{
    font-size: 40px;
    font-weight: 600;
    padding-right: 0rem;
    margin-top: 1rem;
  }
  .header-text{
    margin-top: -21.5rem;
  }
  .header-right img{
    width: 100%;
    border-radius: 9px;
  }
  .header-text-one{
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 1rem;
    background: #f5f5f58a 0 0 no-repeat padding-box;
    border: 1px solid #ebebeb;
    border-radius: 10px;
    box-shadow: 0 0 7px #0000000c;
    padding: 14px 20px;
    margin-bottom: 1rem;
    z-index: 5;
    position: relative;
  }
  .header-summary{
    margin-top: 4rem;
    text-align: center;
    color: #000000B3;
  }
  .header-summary p{
    font-size: 19px;
  }
  .reg{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 2rem;
  }
  .reg1, .reg2{
    display: grid;
    grid-template-columns: 1fr 3fr;
  }
  .reg1{
    border-right: none;
    padding-bottom: 2rem;
    border-bottom: 1px solid rgb(225, 227, 230);
  }
  .reg-text{
    margin-top: -1.2rem;
  }
  .invest{
    margin-left: 10px;
    margin-right: 10px;
  }
  .invest-grid{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    column-gap: 0rem;
    row-gap: 1rem;
  }
  }



  @media (min-width:577px) and (max-width:768px){
    .header{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 2rem;
}
.header-left h1{
    font-size: 40px;
    font-weight: 600;
    padding-right: 0rem;
    margin-top: 1rem;
  }
.header-left{
  text-align: center;
}
.header-text{
    margin-top: -33rem;
  }
  .header-summary{
    margin-top: 14.5rem;
    text-align: center;
    color: #000000B3;
  }
  .header-summary p{
    font-size: 19px;
  }
  .reg{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 4rem;
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 2rem;
  }
  .reg1, .reg2{
    display: grid;
    grid-template-columns: 1fr 6fr;
  }
  .reg1{
    border-right: none;
    padding-bottom: 2rem;
    border-bottom: 1px solid rgb(225, 227, 230);
  }
  .reg-text{
    margin-top: -1.2rem;
  }
  .invest{
    margin-left: 10px;
    margin-right: 10px;
  }
  .invest-grid{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    column-gap: 0rem;
    row-gap: 1rem;
  }
  }

  @media(min-width:769px) and (max-width:1200px){
    .header{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    row-gap: 2rem;
}
.header-left h1{
    font-size: 58px;
    font-weight: 600;
    padding-right: 5rem;
    margin-top: 7.5rem;
  }
  .header-text{
    margin-top: -26rem;
  }
  .header-summary {
    margin-top: 7rem;
    text-align: right;
    color: rgba(0,0,0,0.70196);
}
  .reg{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 4rem;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    column-gap: 2rem;
  }
  .invest{
    margin-left: 10px;
    margin-right: 10px;
  }
  }
</style>
