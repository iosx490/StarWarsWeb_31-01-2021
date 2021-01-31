<template>
  <div class="footer">
  <footer aria-label="Pie de la pagina" class="GeneralFooter">

        <nav aria-label="Mapa Web" class="Tabla">

        <div class="col">
            <h2><span class="sin_enlace"><a href="#PRIMERA">PRIMERA TRIOLOGIA</a></span></h2>
            <p>
            </p><hr>
            <p>
            </p><div class="apoyos">
            <ul>
            <li><a href="#PRIMERA">STAR WARS: EPISIODIO I</a></li>
            <li><a href="#PRIMERA">STAR WARS: EPISIODIO II</a></li>
            <li><a href="#PRIMERA">STAR WARS: EPISIODIO III</a></li>
            </ul>
            </div>
            </div>

        <div class="col">
                <h2><span class="sin_enlace"><a href="#SEGUNDA">SEGUNDA TRIOLOGIA</a></span></h2>
                <p>
                </p><hr>
                <p>
                </p>
                <div class="apoyos">
                <ul>
                <li><a href="#SEGUNDA">STAR WARS: EPISIODIO IV</a></li>
                <li><a href="#SEGUNDA">STAR WARS: EPISIODIO V</a></li>
                <li><a href="#SEGUNDA">STAR WARS: EPISIODIO VI</a></li>
                </ul>
                </div>
                </div>

        <div class="col">
                <h2><span class="sin_enlace"><a href="#TERCERA">TERCERA TRIOLOGIA</a></span></h2>
                <p>
                </p><hr>
                <p>
                </p><div class="apoyos">
                <ul>
                <li><a href="#TERCERA">STAR WARS: EPISIODIO IIV</a></li>
                <li><a href="#TERCERA">STAR WARS: EPISIODIO IIIV</a></li>
                <li><a href="#TERCERA">STAR WARS: EPISIODIO IX</a></li>
                </ul>
                </div>
                </div>
        </nav>
        <a href="https://www.starwars.com/"><img alt="Logotipo Imperio" class="LogoFinalPagina" src="../assets/LOGO2.png"></a>
        <p class="Copyright">© 2020 Practicas Web Dinámica Inc.</p>
        </footer>
      </div>
</template>

<style>


h2 .sin_enlace a {
color: #ffffff;
}
.col{

    color: white;
}
.col li{

    text-align: start;
}
.col p {
display: block;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px
    
}
.apoyos li a {
    
    text-align: center;
    text-decoration: none;
    color: white;
    padding: auto;
}
.col hr{
        display: block;
    unicode-bidi: isolate;
    margin-block-start: 0.5em;
    margin-block-end: 0.5em;
    margin-inline-start: auto;
    margin-inline-end: auto;
    overflow: hidden;
    border-style: inset;
    border-width: 1px;
}

.col ul{

    display: block;
    list-style-type: disc;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    padding-inline-start: 40px;
}
.col h2{
text-align: start;
        display: block;
    font-size: 1.8em;
    margin-block-start: 0.83em;
    margin-block-end: 0.83em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    font-weight: bold;
}

.footer{

    display: block;
}
.Tabla{
    
    
    display: grid;
    font-size: calc(0.2em + 0.85vw);
    grid-gap: 0.5rem;
    grid-template-columns: 100%;
    text-decoration: none;
    padding: 5%;
    padding-bottom: 10%;
    padding-top: 10%;
}

.LogoFinalPagina{
    align-content: center;
    width: 5%;
    margin: auto;
    display: block;
}

.Copyright{

    padding: 2%;
    color: white;
}


</style>
