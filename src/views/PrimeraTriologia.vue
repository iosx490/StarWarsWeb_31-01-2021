<template>
<div>
  <div class="PrimeraTriologia" v-for="img in imgs" :key="img.id">
    <div>
      <Card1 :src="img.srcimg" :texto="img.texto"></Card1> 

    </div>
  </div>
</div>
</template>

<script>
// @ is an alias to /src
import Card1 from '@/components/Card1.vue'
const peliculas_path = '../Peliculas1.json'


export default {
  name: 'PrimeraTriologia',
  components: {
    Card1
  },
  data: function(){

    return {

      imgs: []

    }

  },
  
   mounted() {
      this.fetchData()
    },

    methods: {
        async fetchData() {
          const res = await fetch (peliculas_path);
          const val= await res.json();
          this.imgs=val;
          console.log(val);
        }
}
}


</script>