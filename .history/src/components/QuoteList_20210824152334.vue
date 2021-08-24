<template>
  <section class="quote-list">
      <div class="quote" 
      v-for="(quote, i) in quotes.slice().reverse()" 
      :key="i">
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
.quote-list{
    padding: 32px;
    max-width: 720px;
    margin: 0 auto;
}
.quote{
    background-color: var(--light);
    padding: 16px;
    border-radius: 16px;
    margin-bottom: 16px;
}
.quote-content{
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    line-height:18px;
    max-height: 18px;
}
.quote-content:hover{
    white-space: unset;
    max-height: unset;
}
</style>
