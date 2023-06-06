<script >
import AppHeader from "./components/AppHeader.vue"
import ListCards from "./components/ListCards.vue"
export default {
  components: {
    AppHeader,
    ListCards,
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
