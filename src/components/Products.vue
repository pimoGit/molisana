<template>
 <section>
     <h2>Elenco prodotti</h2>

     <div id="card-container">

       <Product v-for="(productiesimo, index) in productslist" :key="index"
          :details="productiesimo"
       />

     </div>
      
    

 </section>
</template>

<script>
import Product from './Product.vue'

export default {
  name: 'Products',
  components: {
    Product
  },
  data() {
        return {
            // Con import file esterno
            //products: ProdItems,
            productslist: [
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/1-spaghetto-quadrato.jpg",
                titolo: "N.4 Spaghetto Quadrato Bucato",
                tipo: "lunga",
                cottura: 6,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/5-fettuccine.jpg",
                titolo: "N.5 Fettuccine",
                tipo: "lunga",
                cottura: 13,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/6-linguine.jpg",
                titolo: "N.6 Linguine",
                tipo: "lunga",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/7-mezze-linguine.jpg",
                titolo: "N.7 Mezze Linguine",
                tipo: "lunga",
                cottura: 11,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/04/11-spaghettino-quadrato.jpg",
                titolo: "n.11 Spaghettino Quadrato",
                tipo: "lunga",
                cottura: 9,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/38-mezze-maniche.jpg",
                titolo: "N.38 Mezze maniche",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/44-sedani.jpg",
                titolo: "N.44 Sedani",
                tipo: "corta",
                cottura: 8,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/49-sedani.jpg",
                titolo: "N.49 Sedanini",
                tipo: "corta",
                cottura: 8,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/53-lumachine.jpg",
                titolo: "N.53 Lumachine",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/55-chifferi-rigati.jpg",
                titolo: "N.55 Chifferi rigati",
                tipo: "corta",
                cottura: 12,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/05/58-misto-corto.jpg",
                titolo: "N.58 Misto corto",
                tipo: "corta",
                cottura: 9,
              },
              {
                src: "https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg",
                titolo: "N.84 Ditale Quadrato",
                tipo: "cortissima",
                cottura: 12,
              },
            ],
        };
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
p {
  margin: 40px 0 0;
  color: blue;
}

#card-container {
  max-width: 90%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
}


</style>
