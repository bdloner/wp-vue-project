<template>
  <header class="site-header">
    <MainMenu :menu="menu" />
  </header>
</template>

<script>

import MainMenu from '../partials/Menu.vue';
import Axios from 'axios';

export default {
  data(){
    return {
      menu: false
    }
  },

  beforeMount(){
    this.fetchMenu();
  },

  methods: {
    fetchMenu(){
      Axios
        .get("/vueproject/wp-json/menus/v1/menus/main-menu")
        .then(response =>{
          this.menu = response.data;
        })
        .catch(error => console.log("not working"));
    }
  },
  
  components:{
    MainMenu
  }
}
</script>