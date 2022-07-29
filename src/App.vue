<template>

<Navbar/>
  <Banner/>

<div class="container mt-4">
  <div class="row">
    <div class="c0l-6 col-sm-4 col-md-3" v-for="i in 10" :key="i">
     <Furniture/>
    </div> 
    </div>
   </div>

</template>

<script>
import Banner from "./components/Banner.vue";
import Furniture from "./components/Furniture.vue";
import Navbar from "./components/Navbar.vue";

export default {
    name: "App",
    data() {
        return {
            nama_website: "furniture"
        };
    },
    components: {
    Banner,
    Furniture,
    Navbar
},
mounted() {
console.log("sudah di render nih")
}
}

</script>
