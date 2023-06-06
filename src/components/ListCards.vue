<script>

export default {
  name : "ListCards",


  

}
</script>

<template>

   <section id="main-container">

    <div id="footer-list">
        <p>paperino</p>
    </div>

   </section>
       

  
</template>

<style lang="scss" scoped >

@use "../styles/general.scss" as* ;

#main-container {
    width: 80%;
    height: 1000px;
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
}




</style>