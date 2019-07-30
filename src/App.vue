<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Gallery title="Minha galeria" :images="images"/>
  </div>
</template>

<script>
import Gallery from './components/Gallery'

export default {
  name: 'App',
  components: {
    Gallery
  },
  data() {
    return {
      images: [],
    };
  },
  mounted() {
    setTimeout(() => {
      this.images = [
        {
          url: 'https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80',
          title: 'Gatinho',
          description: 'Foto de um gatinho',
        },
        {
          url: 'https://iriscaoc.files.wordpress.com/2016/01/paisagem-natural-1.jpg',
          title: 'Paisagem Natural',
          description: 'Foto em uma praia',
          css: 'column-8'
        },
        {
          url: 'https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80',
          title: 'Gatinho',
          description: 'Foto de um gatinho',
          css: 'column-8'
        },
        {
          url: 'https://iriscaoc.files.wordpress.com/2016/01/paisagem-natural-1.jpg',
          title: 'Paisagem Natural',
          description: 'Foto em uma praia'
        },
        {
          url: 'https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80',
          title: 'Gatinho',
          description: 'Foto de um gatinho',
        },
      ];
    }, 3000);
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
