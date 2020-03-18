<template>
  
    <div class="nav flex-column nav-pills" id="v-pills-tab" role="tablist" aria-orientation="vertical">
      <a class="nav-link active" id="v-pills-home-tab" data-toggle="pill" href="#v-pills-home" role="tab" aria-controls="v-pills-home" aria-selected="true">{{categories.name}}</a>
    
  </div>

</template>
<script>
export default {
  props: ['categories']
}
</script>