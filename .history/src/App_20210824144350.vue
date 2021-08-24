<template>
  <div class="app">
    <Header title="The Anime Quoter" />
    <Quote :quote="quote " />
  </div>
</template>

<script>

import Header from './components/Header.vue';
import Quote from './components/Quote.vue'

export default {
  name: 'App',
  components: {
    Header,
    Quote
  },
  data(){
    return{
      quote: {
        content: 'Content goes here',
        anime: 'Naruto',
        character: 'Madara'
      },
      quotes: [],
    }
  },
  methods: {
    async getQuote(){
      const data = await fetch('https://animechan.vercel.app/api/random').then(res => res.json());

      this.quote = {
        content: data.quote,
        anime: data.anime,
        character: data.character,
      };
    }
  },
  create(){
    this.getQuote();
  }
}
</script> 

<style Lang="sass">
:root{
  --primary: #D81E58;
  --secondary: #8A4FFF;
  --tertiary: #32CBDD;
  --dark: #131A26;
  --light: #EEE;
  --grey: #848484;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira Sans', sans-serif;
}
</style>
