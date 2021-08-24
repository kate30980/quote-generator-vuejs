<template>
  <section class="quote-list">
      <div class="quote" v-for="(quote, i) in quotes.slice().reverse()" :key="i">
          <div class="quote-content">
              {{ quote.content }}
          </div>
      </div>
  </section>
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>


<style scoped>

</style>
