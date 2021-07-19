<template>
  <banner />
  <article-block />
  <footer-block />
</template>

<script>
import Banner from '@/components/Banner.vue'
import ArticleBlock from '@/components/ArticleBlock.vue'
import FooterBlock from './components/FooterBlock.vue'

export default {
  name: 'App',
  components: {
    Banner, 
    ArticleBlock,
    FooterBlock
  }
}
</script>

<style>

</style>
