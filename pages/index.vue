<template>
  <section>
    <Header/>
    <Description/>
    <SubNavigation/>
    <Banner/>
    <BlogContent/>
    <FeaturedGame/>
  </section>
</template>

<script>
import Header from '~/components/Header.vue'
import Description from '~/components/Description.vue'
import SubNavigation from '~/components/SubNavigation.vue'
import Banner from '~/components/Banner.vue'
import BlogContent from '~/components/BlogContent.vue'
import FeaturedGame from '~/components/FeaturedGame.vue'

export default {
  name: 'mainPage',
  components: {
    Header,
    Description,
    SubNavigation,
    Banner,
    BlogContent,
    FeaturedGame
  }
}
</script>

<style>
</style>

