<template>
  <div class="home">
    <Scrollview/>
    <div class="container-lg">
      <h1>PRIMERA TRIOLOGIA</h1>
          <b-card-group columns>
            <div class="home_cards" columns v-for="img in peliculas1" :key="img.id">
                <Card1 :src="img.srcimg" link="/PrimeraTriologia"></Card1> 
            </div>
           </b-card-group>
      <h1>SEGUNDA TRIOLOGIA</h1>
          <b-card-group columns>
            <div class="home_cards" columns v-for="img in peliculas2" :key="img.id">
                <Card1 :src="img.srcimg" link="/SegonaTriologia"></Card1> 
            </div>
           </b-card-group>
      <h1>TERCERA TRIOLOGIA</h1>
          <b-card-group columns>
            <div class="home_cards" columns v-for="img in peliculas3" :key="img.id">
                <Card1 :src="img.srcimg" link="/TerceraTriologia"></Card1> 
            </div>
           </b-card-group>
       </div>
  </div>
</template>


<script>
// @ is an alias to /src
import Card1 from '@/components/Card1.vue'
import Scrollview from '@/components/Scrollview.vue'
const peliculas1_path = '../Peliculas1.json'
const peliculas2_path = '../Peliculas2.json'
const peliculas3_path = '../Peliculas3.json'



export default {
  name: 'Home',
  components: {
    Card1, Scrollview
  },
  data: function(){

    return {

      peliculas1: [],
      peliculas2: [],
      peliculas3: []

    }

  },
  
   mounted() {

      this.prepare();
      
    },

    methods: {

        fetchData: async function(path) {
          const res = await fetch (path);
          const val= await res.json();
          return val;
        },
        prepare: async function(){

          this.peliculas1= await this.fetchData(peliculas1_path)
          this.peliculas2= await this.fetchData(peliculas2_path)
          this.peliculas3= await this.fetchData(peliculas3_path)

        }
  }
}


</script>

<style>

.carousel-caption h3{
    font-size: calc(0.5em + 0.95vw);

}
.container-lg h1{

font-size: calc(0.5em + 1.95vw);
  margin: 2%;
 /*font-size: 180%;*/
  background-color: rgb(241, 219, 16);
 border-radius: 50px;
   font-weight: bold;
  color: rgb(0, 0, 0);
}
.card-columns .card {
    margin-bottom: 3.75rem;
}
.cartas{

width: 100%;
padding-top: 5%;
padding-bottom: 30%;

}


.card-body{

background-color: rgba(255, 255, 255, 0);

}

.card-img
{
 width: 100%;
}
.card-img-overlay{
 top: 100%;
}

.btn{
    font-size: calc(0.5em + 0.65vw);
  margin-top: 5%;
  background-color: rgb(255, 255, 255);
  border-radius: 30px;
   font-weight: bold;
}

@media (max-width: 575px ) {

  .home_cards > .cartas{

    margin: 0 auto;
    width: 50%;
    padding-bottom: 10%;

  }
}
</style>