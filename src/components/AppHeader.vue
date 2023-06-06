<script>

export default {
  name : "AppHeader",


  

}
</script>

<template>

    
    <header>
      <div class="container-img">
        <img src="https://upload.wikimedia.org/wikipedia/commons/1/11/Yu-Gi-Oh%21_%28Logo%29.jpg" alt="logo">
      </div>
      <h1>Yu-gi-oh Api</h1>
    </header>
       

  
</template>

<style lang="scss" scoped >

@use "../styles/general.scss" as* ;
header {
  height: 100px;
  display: flex;
  gap: 30px;
  align-items: center;
  
  h1 {
    font-size: 40px;
    
  }
  .container-img {
    margin-left: 50px;
    width: 200px;
    height: 100%;
    img {
      height: 100%;
      width: 100%;
      object-fit: fill;
    }
  }


}



</style>