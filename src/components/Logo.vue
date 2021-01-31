<template>
  <div class="logo">
    <img alt="StarWars logo" src="../assets/Logo.png">



      <b-navbar-toggle id='MovilButton' class="navbar-dark" v-b-toggle.sidebar-1></b-navbar-toggle>

      <b-sidebar id="sidebar-1" shadow>


          <b-nav vertical>
            
      <b-nav-item to="/Home">Home</b-nav-item>
      <p class="linea"></p>
      <b-nav-item to="/PrimeraTriologia">Primera Triologia</b-nav-item>
      <p class="linea"></p>
      <b-nav-item to="/SegundaTriologia">Segunda Triologia</b-nav-item>
      <p class="linea"></p>
      <b-nav-item to="/TerceraTriologia">Tercera Triologia</b-nav-item>
      <p class="linea"></p>
               

         </b-nav>


    </b-sidebar>
    </div>
</template>

<style>


#MovilButton{
  
display: none;
  float:right ;
  font-size: 5vw;
}
.logo img{

  width: 20%;
}

.linea{

    border-style: inset;
    border-width: 1px;
    margin-left:5% ;
    margin-right:5% ;
}

#sidebar-1{

padding-top:2% ;
  background-color: black!important;
  border-radius: 0px;
}

.b-icon.bi{

  color: #ffffff;

}

#sidebar-1{

  display: none;
} 
@media (max-width: 575px ) {

  .logo {

    text-align: left;
    margin: 2% 2%;

  }


#sidebar-1{

  display: block;
} 

  .nav-item a{
text-decoration: white;
  color: white;
}


#MovilButton{

display: block;

}

}

</style>