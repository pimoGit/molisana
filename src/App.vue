<template>
  <div id="app">
    <Header :links="menu"/>

    <main>
      <Products/>
    </main>

    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Products from './components/Products.vue'



export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Products
  },
  data(){
    return {
        menu: [
            {
                text: "Home",
                url: "#",
                current: false
            },
              {
                text: "Prodotti",
                url: "#",
                current: true
            },
              {
                text: "Chi Siamo",
                url: "#",
                current: false
            },
              {
                text: "Contatti",
                url: "#",
                current: false
            },
        ],
    }
}
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
