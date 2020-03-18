<template>
  <div id="app">
   
     <Header/>
     <div class="row">
<div class="col-3">
     <Category v-for="cat in categories" :categories="cat" :key="cat.id" /> 
</div> 
<div class="col-9">
  <div class="row row-cols-1 row-cols-md-3">
     <Products v-for="product in products" :products="product" :key="product.id"/>
  </div>
</div>
     </div>
    
     
  </div>
</template>

<script>

import Header from '@/components/Header.vue'
import Category from '@/components/Category.vue'
import Products from '@/components/Products.vue'



export default {
  name: 'App',
  components: {
    Header, 
    Category,
    Products

  },
  data(){
    return{
      categories: [
        {
        id: 1, 
        name: "Computing"
      },{
        id: 2, 
        name: "Tablet/Phones"
      },
      {
        id: 3, 
        name: "Fashion"
      },
      {
        id: 4, 
        name: "Accessories"
      },
      

      ],
      products:[{
       imageLink : require('@/assets/lap1.jpg'),
        name: "hp 15",
        price: "$ 200,000",
        specs: "1TB HDD, 16GB RAM",
        categoryId: 1

      },
      {
       id: 2,
          imageLink : require('@/assets/lap1.jpg'),
          name : "hp 15",
          price: "$ 150,000",
          specs : "1TB HDD, 4GBRAM",
           
      },
       {
        id: 3,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 180,000",
           specs : "1TB HDD, 16GBRAM",
      },
       {
       id: 4,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 170,000",
          specs : "500GB HDD, 8GBRAM",
      },
       {
        id: 5,
          imageLink : require('@/assets/lap3.jpg'),
          name : "hp 15",
          price: "$ 150,000",
          specs : "500gb HDD, 4GB RAM",
      },
      {
        id: 6,
          imageLink : require('@/assets/pb1.jpg'),
          name : "hp 15",
          price: "$ 150,000",
          specs : "32gb HDD, 4GB RAM",
      },
      {
        id: 7,
          imageLink : require('@/assets/tab1.jpg'),
          name : "hp 15",
          price: "$ 150,000",
          specs : "32gb HDD, 4GBRAM",
      },
      {
        id: 8,
          imageLink : require('@/assets/tab2.jpg'),
          name : "hp 15",
          price: "$ 150,000",
          specs : "32gb HDD, 4GBRAM",
      },
      {
        id: 9,
          imageLink : require('@/assets/phone1.jpg'),
          name : "iphone",
          price: "$ 550,000",
          specs : "32gb HDD, 6GB RAM",
      },
      

      
      ]
    }
  }
}
</script>

<style>

</style>
