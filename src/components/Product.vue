<template>

       <div class="card-prod" >
        <img :src="details.src" :alt="details.titolo">
        <h4>{{details.titolo}}</h4>
      </div>

</template>

<script>
export default {
  name: 'Product',
  props: {
      details: Object
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.card-prod {
  flex-basis: 25%;

  img {
    max-width: 100%;
  }
}


</style>
