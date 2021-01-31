<template>
<div class="cartas" >
  <b-card
    overlay
    :img-src="src"

    img-alt="Card Image"
    text-variant="white"
  >

  <b-card-text v-if="texto">
          {{texto}}
        </b-card-text>


    <b-button :to="link" variant="third" v-if="link">Ampliar</b-button>
  </b-card>
</div>
</template>

<script>
export default {
  name: 'Card1',
  props: [
    'src', 'texto', 'link'
  ]

}
</script>
