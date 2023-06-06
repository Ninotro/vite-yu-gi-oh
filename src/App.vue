<script >
import axios from "axios";
import { store } from "./store.js";
import AppHeader from "./components/AppHeader.vue"
import ListCards from "./components/ListCards.vue"
export default {
  components: {
    AppHeader,
    ListCards,
  },

  data () {
    return {
      store,
    }
    
  },
  methods: {
    getCharacters() {
      axios.get(store.apiUrl)
      .then(res => {
        store.characterList = res.data.data
        store.loading = false
       
      })
      .catch(err => {
        console.log(err);
      })
      

    }
  },
  created() {
    this.getCharacters();
    

  }
}
</script>

<template>
  <AppHeader/>


  
  <main>

    <ListCards/>


  </main>
</template>

<style lang="scss" >
@use "../src/styles/general.scss";

main {
  background-color: orange;
  width: 100%;
  padding-bottom: 100px;
  padding-top: 100px;
}
</style>
