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
  html {
    background-color: #CBE9F6;
  }

  body {
    margin-left: auto;
    margin-right: auto;
    width: 1000px;
    background-color: #93BAE7;
  }
</style>
