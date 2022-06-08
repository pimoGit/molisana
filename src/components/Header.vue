<template>
 <header>
     <a href="#">
         <img src="../assets/img/la-molisana-logo.png" alt="logo la Molisana">
     </a>
     <nav>
         <ul>
             <li v-for="(link, index) in links" :key="index">
                 <a :href="link.url"
                    :class="link.current ? 'here' : ''"
                 >
                     {{link.text}}
                 </a>
             </li>
         </ul>
     </nav>
 </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
      return {
          links: [
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
    text-align: center;

    ul {
        list-style-type: none;
        margin: 20px 0;

        li {
            display: inline-block;
            padding:10px;

            a {
                text-decoration: none;
                color: #000;
                padding:10px;
                
                
                &:hover{
                    color: violet;
                }
                &.here {
                    background-color: aqua;
                }

            }
        }
    }
}

</style>
