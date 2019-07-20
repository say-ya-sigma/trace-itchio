<template>
  <section class="blog-content-section">
    <h2 class="section-title">From the blog</h2>
    <ul class="blog-list">
      <li class="blog-item" v-for="item in items" :key="item.id">
        <div class="blog-image-container">
          <img class="blog-image" :src="item.image">
        </div>
        <a class="blog-title">{{item.title}}</a>
        <p class="blog-description">{{item.description}}</p>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { id: 1,
          image: require('@/assets/blog-image-1.png'),
          title: 'How to get started on itch.io',
          description: 'In my day-to-day I get asked a lot about how to get started on itch.io. This comes from established developers looking t...'
        },
        { id: 2,
          image: require('@/assets/blog-image-2.png'),
          title: 'itch.io Recommends: four machine games',
          description: 'This week’s recommendations are all about machines. Building them, using them, and.. what it means for them to be'
        },
        { id: 3,
          image: require('@/assets/blog-image-3.png'),
          title: 'Fill up July with a bunch of great game jams!',
          description: 'Are you worried that you don’t have enough things to do? Have you somehow run out of games to play and'
        },
        { id: 4,
          image: require('@/assets/blog-image-4.png'),
          title: 'itch.io Recommends: games that aren\'t even out yet! (And one that is)',
          description: 'We’re getting weird with time this week as we recommend two pre-release games (and one that’s already out).'
        },
        { id: 5,
          image: require('@/assets/blog-image-5.png'),
          title: 'Tips and tricks to help your itch.io launch',
          description: 'In the interest of transparency, we’re going to do something a bit differently on the blog this week: we’re lifting...'
        },
        { id: 6,
          image: require('@/assets/blog-image-6.png'),
          title: 'itch.io Recommends: a whole bunch of animals',
          description: 'How about that itch.io sale that just ended? Pretty wild huh? Well we’re back with a new batch of games to'
        },
        { id: 7,
          image: require('@/assets/blog-image-7.png'),
          title: 'The itch.io Summer Sale is here!',
          description: 'Take a vacation into the land of hot deals with the itch.io Summer Sale! From the time you’re reading this until'
        },
        { id: 8,
          image: require('@/assets/blog-image-8.png'),
          title: 'itch.io Recommends: experimental new games',
          description: 'Let’s get experimental y’all. This week’s recommendations are a pair of games that don’t really behave like any...'
        },
      ]
    }
  }
}
</script>

<style scoped>
.blog-content-section {
  margin: 20px auto 40px auto;
  font-family: 'Lato';
  word-spacing: 0px;
  line-height: 1.25;
}
.section-title {
  margin: 0 0 20px 10px;
  font-size: 16px;
  font-weight: 900;
}
.blog-list {
  padding: 0 10px;
  white-space: nowrap;
  overflow-x: auto;
}
.blog-item {
  display: inline-block;
  width: 50vw;
  margin-right: 15px;
  padding-bottom: 12px;
  white-space: normal;
  vertical-align: top;
}
.blog-image-container {
  background-color: rgba(0, 0, 0, 0.05);
  padding-bottom: 55.25%;
  position: relative;
  overflow: hidden;
}
.blog-image {
  display: block;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
}
.blog-title {
  display: block;
  font-size: 14px;
  font-weight: bold;
  color: #222222;
  line-height: 20px;
  margin: 5px 0;
}
.blog-description {
  font-size: 12px;
  color: #222222;
  line-height: 18px;
}
</style>
