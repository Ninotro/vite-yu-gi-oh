<script>
import SingleCard from "../components/SingleCard.vue"
import {store} from "../store.js"
import SearchComponent from "../components/SearchComponent.vue";

export default {

  components : {
    SingleCard,
    SearchComponent
  },
  name : "ListCards",

  data() {
    return {
       store
    }
  }


  

}
</script>

<template>

   <section id="main-container">
    <SearchComponent />
    <div id="footer-list">
        <p>paperino</p>
    </div>
    <div id="card-list">
        <SingleCard v-for="character in store.characterList" 
        :details="character" />
    </div>
    

   </section>
       

  
</template>

<style lang="scss" scoped >

@use "../styles/general.scss" as* ;

#main-container {
    width: 80%;
    
    margin: 0 auto;
    background-color: white;
    #footer-list {
        height: 100px;
        background: blue;
        padding-left: 30px;
        display: flex;
        align-items: center;
        p {
            color: white;
            font-size: 20px;


        }
    }

    #card-list {
      padding: 20px 20px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
}




</style>