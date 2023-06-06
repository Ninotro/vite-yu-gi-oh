<script>
import {store} from "../store.js"
export default {
 
  name : "SearchComponent",

  data() {
    return {
       store
    }
  }
  

}
</script>

<template>
<div>
<select id="Option">
    <option value="1">test1</option>
    <option value="2" selected="selected">test2</option>
    <option value="3">test3</option>
  </select>
</div>  
</template>

<style lang="scss" scoped >

@use "../styles/general.scss" as* ;


div {
    background: orange;

    #option {
        
        margin: 20px;
        option {
            height: 100px;
            width: 100px;
            font-size: 30px;
        }
    }
}

</style>