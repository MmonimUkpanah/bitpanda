<template>
    <div class="con">
        <nav class="navbar fixed-top con navbar-expand-lg ">
            <div class="container-fluid">
                <a class="navbar-brand" href="#"><img src="/logo-bitpanda.svg" alt="logo"></a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
                <img src="/menu.png" alt="toggler">
                </button>
                <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
                <ul class="navbar-nav mr-auto mb-2 mb-lg-0">
                    <li class="nav-item">
                    <a class="nav-link" href="dashboard">Home</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="portfolio">Portfolio</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#">Prices</a>
                    </li>
                </ul>
                <form class="d-flex button-group" role="search">
                    <button class="sign">Trade</button>
                    <button class="sign">Deposit</button>
                    <button class="log">Send</button>
                    <img src="grey.svg" alt="">
                </form>
                </div>
            </div>
        </nav>
    </div>
</template>


<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.navbar{
    background: white;
}
.con{
    margin-left: 10rem;
    margin-right: 10rem;
    padding: 20px 0;
    
}
.navbar-brand img{
    width: 136px;
}
.navbar-toggler img{
    width: 1.5rem;
    margin-top: -10px;
}
.nav-link{
    color: black;
    font-size: 15px;
    font-weight: 600;
    margin-right: 1rem;
}
.nav-link:hover{
    border-bottom: 2px solid #27d17f !important;
}
.navbar-nav{
    margin-left: 20%;
}
.login{
    background-color:#f3f3f2 ; 
    color: black;
    border-radius: 5px;
    font-size: 15px;
    padding: 5px 15px;
    border: none;
    margin-right: 0.5rem;
}
.sign{
    border-radius: 3px;
    font-size: 15px;
    padding: 5px 15px;
    color: white;
    background: #16a858;
    border: 1px solid #16a858;
}
.log{
    border-radius: 3px;
    font-size: 15px;
    padding: 5px 15px;
    color: #16a858;
    background: white;
    border: 1px solid #16a858;
    margin-left: 1rem;
    margin-right: 1rem;
}
.navbar-toggler{
    background: #16a858;
    padding: 7px 10px;
}
.search{
    display: none;
}
.button-group p{
    color: rgb(51, 51, 51);
    font-weight: 600;
    margin-right: 1rem;
    margin-top: 0.2rem;
}




@media(max-width:567px){
    .con{
    margin-left: 0;
    margin-right: 0;
    padding-left: 10px;
    padding-right: 10px;
}
.navbar-nav{
    margin-left: 0%;
    margin-top: 1.5rem;
}
.nav-link{
    color: black;
    font-size: 20px;
    font-weight: 600;
    margin-right: 1rem;
    margin-bottom: 1.5rem;
}
.search{
    display: block;
    width: 100%;
    border: none;
    border-radius: 5px;
    background-color: #f3f3f2;
    padding: 10px 15px;
    margin-top: 1.5rem;
    margin-bottom: 1rem;
}

.login{
    background-color:#f3f3f2 ; 
    color: black;
    border-radius: 5px;
    font-size: 15px;
    padding: 12px 15px;
    border: none;
    margin-right: 0.5rem;
    width: 50%;
}
.sign{
    background-color: #27d17f;
    color: white;
    border-radius: 5px;
    font-size: 15px;
    padding: 12px 15px;
    border: none;
    width: 50%;
}

}

@media(min-width: 577px) and (max-width:768px){
    .con{
    margin-left: 0;
    margin-right: 0;
    padding-left: 10px;
    padding-right: 10px;
}
.navbar-nav{
    margin-left: 0%;
    margin-top: 1.5rem;
}
.nav-link{
    color: black;
    font-size: 20px;
    font-weight: 600;
    margin-right: 1rem;
    margin-bottom: 1.5rem;
}
.search{
    display: block;
    width: 100%;
    border: none;
    border-radius: 5px;
    background-color: #f3f3f2;
    padding: 10px 15px;
    margin-top: 1.5rem;
    margin-bottom: 1rem;
}

.login{
    background-color:#f3f3f2 ; 
    color: black;
    border-radius: 5px;
    font-size: 15px;
    padding: 12px 15px;
    border: none;
    margin-right: 0.5rem;
    width: 50%;
}
.sign{
    background-color: #27d17f;
    color: white;
    border-radius: 5px;
    font-size: 15px;
    padding: 12px 15px;
    border: none;
    width: 50%;
}
}


@media(min-width: 769px) and (max-width:1200px){
    .con{
    margin-left: 0;
    margin-right: 0;
    padding-left: 10px;
    padding-right: 10px;
}
.navbar-nav{
    margin-left: 15%;
}
}

</style>