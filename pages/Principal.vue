<template>
  <div>
    <div>{ span }</div>
    
    <div v-if="loading"><Loading /></div>
    <div v-else><span>Holaa</span></div>
  </div>
</template>

<script>
import Loading from "../components/Loading";
import axios from 'axios'

export default {
  data() {
    return {
      loading: true,
      pokemons: [],
    }
  },
  component: {
    Loading,
  },
  async created() {
    try {
      const { data } = await axios.get('http://localhost:3001/pokemons');
      this.pokemons = data;
      this.loading = false;
      console.log(data)
    } catch (error) {
      console.error(error)      
    }
  }
};
</script>
