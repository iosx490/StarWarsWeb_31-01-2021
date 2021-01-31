<template>
<div id="av">
  <b-navbar type="light" variant="light">
    <b-nav>
      <b-nav-item to="/Home">Home</b-nav-item>
      <b-nav-item to="/PrimeraTriologia">Primera Triologia</b-nav-item>
      <b-nav-item to="/SegundaTriologia">Segunda Triologia</b-nav-item>
      <b-nav-item to="/TerceraTriologia">Tercera Triologia</b-nav-item>

    </b-nav>
  </b-navbar>
</div>
</template>

<style>

.bg-light
{
background-color: white!important;
border-radius: 50px;
justify-content: center;
}
.navbar-nav li{

margin-left: 1%;
margin-right: 1%;

}

.nav-link {

color: black!important;
font-weight: bold;

}

#av{

  padding-bottom: 2%;
}

@media (max-width: 575px ) {
  #av{
    display: none;
    }

    .nav-link {

      color: rgb(255, 255, 255)!important;
      
    }
}


</style>