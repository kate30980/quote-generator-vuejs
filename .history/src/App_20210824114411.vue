<template>
  <div class="app">
    <Header title="The Anime Quoter/>
  </div>
</template>

<script>

import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
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
