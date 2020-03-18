<template>
  <div class="card text-white bg-primary mb-3" style="max-width: 14rem;">
    <div class="card h-50">
      <img :src="products.imageLink" class="card-img-top" alt="...">
      <div class="card-body" >
        <h5 class="card-title">{{products.name}}</h5>
        <p>{{products.price}}</p>
        <p>{{products.specs}}</p>
        <button class="btn btn-primary">Buy In</button>
      </div>

    </div>
  </div>
 

</template>

<script>
export default {
  props: ['products']
}
</script>