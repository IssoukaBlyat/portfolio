<script setup>
import Footer from '@/components/Footer.vue';
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
</script>

<template>
  <body>
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </body>
  
</template>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,400;0,700;1,400&display=swap');

  @font-face {
    font-family: "Raleway";
    src: url('../fonts/Raleway-VariableFont_wght.woff');
    src: url('../fonts/Raleway-Italic-VariableFont_wght.ttf') format('truetype'),
    url('../fonts/Raleway-VariableFont_wght.ttf') format('opentype');
  }

  h1{
    font-family: "Lato", sans-serif;
  }

  h2{
    font-family: "Lato", sans-serif;
  }

  h3{
    font-family: "Lato", sans-serif;
    background-color: #dbc2a4;
    color: black;
    text-indent: 10px;
  }

  h4{
    font-family: "Lato", sans-serif;
  }

  *{
    font-family: 'Raleway', sans-serif;
  }

  body {
    margin-left: auto;
    margin-right: auto;
    width: 1500px;
  }
</style>
