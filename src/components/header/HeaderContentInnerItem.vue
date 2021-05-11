<template>
  <div class="HeaderContentInnerItem" style="display: contents">
      <div>
            <p>{{data.name}}</p> 
      </div>
       <div>
            <p class="quantity">{{data.quantity}}</p>
       </div>
       <div>
            <q-btn color="deep-blue" glossy :label="data.buttonText" />

       </div>
  </div>
</template>


<style lang="scss" scoped>
    .HeaderContentInnerItem div{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    // .HeaderContentInnerItem{
    //     display: flex;
    //     align-items: center;
    //     justify-content: space-around;
    // }
    // .HeaderContentInnerItem *{
    //    margin: 0;
    // }
    // .HeaderContentInnerItem  .quantity{
    //     color: black;
    //     font-size: 27px;
    // }
    p{
        margin: 0;
        text-align: center;
    }
    .quantity{
         color: black;
         font-size: 27px;
     }
</style> 


<script>
export default {
    name: "HeaderContentInnerItem",
    props: ["data"]
 
}

</script>
