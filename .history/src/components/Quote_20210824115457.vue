<template>
  <section class="quote">
      <div class="quote-content">
          Content goes here..
      </div>
      <div class="quote-info">
        <div class="quote-anime">
            Life
        </div>
        <div class="quote-author">
            Me
        </div>
      </div>
  </section>
</template>

<script>
export default {
  props: ['quote']
}
</script>


<style Lang="sass" scoped>
.quote{
    position: relative;
    margin: 0 auto;
    padding: 32px;
    max-width: 720px;
}
.quote-content{
    position: relative;
    font-size: 28px
}
</style>
