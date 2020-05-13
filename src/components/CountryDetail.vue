<template lang="html">
  <div v-if='country'>
    <h3>{{country.name}}</h3>
    <p>Name: {{country.name}}</p>
    <p>Capital City: {{country.capital}}</p>
    <p>Population: {{country.population}}</p>
    <p>Languages Spoken: {{country.languages}}</p>
    </div>
</template>

<script>
import { eventBus } from '../main.js';

export default {
  name: 'country-detail',
  props: ['country']
}

</script>

<style lang="css" scoped>


h3 {
    color: purple;
}
p {
    color: yellow;
    
  }
</style>
