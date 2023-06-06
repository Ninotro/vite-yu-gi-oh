<script>

export default {
  props: {
    details: Object

  },
  name : "SingleCard",


  

}
</script>

<template>

   <div class="card">
    <div class="container-img">
        <img :src="details.card_images[0].image_url" alt="">
    </div>
    <div class="description">
        <div class="text">{{details.name}}</div>
        <div class="type-card"> {{details.archetype}}</div>
    </div>  
   </div>

  
</template>

<style lang="scss" scoped >

@use "../styles/general.scss" as* ;

.card {
    
    
    width: calc(100%/5 - 20px);
    background-color: orange;
    .container-img {
        height: 600px;
        width: 100%;
        

        img{
            width: 100%;
            height: 100%;
            object-fit: fill ;
        }

    }

    .description {
        height: 200px;
        background-color: orange;
        text-align: center;
        font-size: 30px;
        color: white;
        font-weight: bold;
        .text {
       
       
       margin-top: 30px;
       margin-bottom: 30px;
     
       
   }
   .type-card {
       text-align: center;
       
   }
    }
   
}



</style>