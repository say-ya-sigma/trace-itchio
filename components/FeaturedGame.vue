<template>
  <section class="featured-game-section">
    <div class="title-container">
      <h2 class="section-title">Latest Featured Games</h2>
      <button class="button featured-button">View all</button>
    </div>
    <ul class="featured-list">
      <li class="featured-item" v-for="item in items" :key="item.id">
        <div class="featured-image-container">
          <img :class="['featured-image', item.id % 2 === 1 ? 'left' : 'right']" :src="item.image">
        </div>
        <div>
          <div :class="['price-tag', item.id % 2 === 1 ? 'left' : 'right']">{{item.price}}</div>
          <a :class="['featured-title', item.id % 2 === 1 ? 'left' : 'right']">{{item.title}}</a>
        </div>
        <p :class="['featured-description', item.id % 2 === 1 ? 'left' : 'right']">{{item.description}}</p>
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
          image: require('@/assets/featured-game-1.png'),
          title: 'Backland',
          description: 'Escape a procedurally generated city. Survive the Backland',
          price: '$4.99'
        },
        { id: 2,
          image: require('@/assets/featured-game-2.png'),
          title: 'Clea',
          description: 'Outwit the Chaos Servants and escape from the Whitlock Mansion.',
          price: '$6'
        }
      ]
    }
  }
}
</script>

<style scoped>
.featured-game-section {
  margin: 20px auto 40px auto;
  font-family: 'Lato';
  word-spacing: 0px;
  line-height: 1.25;
}
.title-container {
  margin: 0 0 20px 10px;
  display: flex;
  text-align: center;
  vertical-align: center;
}
.section-title {
  width: 60%;
  margin-top: 4px;
  font-size: 16px;
  font-weight: 900;
  text-align: left;
}
.featured-button {
  background-color: white;
  display: inline;
  margin-left: auto;
  margin-right: 20px;
  padding: 0 10px;
  height: 28px;
  line-height: 28px;
  font-family: 'Lato';
  font-size: 14px;
  font-weight: bold;
  color: #ff2449;
  border: 1px solid rgba(255, 35, 73, 0.4);
  border-radius: 3px;
}
.featured-button::after {
  content: "→";
  display: inline-block;
  margin-left: 5px;
  font-family: 'Lato';
  font-size: 12px;
  text-align: center;
  text-decoration: none;
}
.featured-item {
  display: inline-block;
  width: 50vw;
  padding-bottom: 12px;
  vertical-align: top;
}
.featured-image-container {
  width: 50vw;
  background-color: white;
  padding-bottom: 74.2%;
  position: relative;
  overflow: hidden;
}
.featured-image {
  display: block;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
}
.price-tag {
  float: right;
  background-color: #737373;
  color: white;
  padding: 2px 5px;
  font-size: 12px;
  font-weight: bold;
  letter-spacing: 0.6px;
  border-radius: 3px;
}
.price-tag.left {
  margin-right: 5px;
}
.price-tag.right {
  margin-right: 10px;
}
.featured-title {
  display: block;
  font-size: 14px;
  font-weight: bold;
  color: #222222;
  line-height: 17px;
  margin: 6px 0 5px 0;
}
.featured-description {
  font-size: 12px;
  color: #222222;
  line-height: 14.4px;
}
.featured-image.left,
.featured-title.left,
.featured-description.left {
  padding: 0 5px 0 10px;
}
.featured-image.right,
.featured-title.right,
.featured-description.right {
  padding: 0 10px 0 5px;
}
</style>
