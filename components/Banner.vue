<template>
  <div class="banner">
    <div class="background-container">
      <div>
        <video class="banner-background" src="~/assets/banner-background.mp4" autoplay loop></video>
      </div>
      <div class="banner-content">
        <h2 class="bundle-title">Can Androids Play</h2>
        <div class="bundle-games">
          <img class="game" src="~/assets/can-android-play-1.png">
          <img class="game" src="~/assets/can-android-play-2.png">
          <img class="game" src="~/assets/can-android-play-3.png">
        </div>
        <div class="buy-button-container">
          <button class="button buy-button">Get the bundle</button>
          <div class="summary">
            <p>3 items for $6.99</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.banner {
  width: 100%;
  margin: 0 auto 40px auto;
  padding: 0;
}
.background-container {
  background: linear-gradient(41deg, #2D4D95, #642d95);
  position: relative;
  margin: 0 auto;
  overflow: hidden;
}
.banner-background {
  object-fit: cover;
  width: 100%;
  height: 100%;
  position: absolute;
  opacity: 0.4;
  z-index: 1;
}
.banner-content {
  color: white;
  font-family: 'Lato';
  text-shadow: 0 1px 1px rgba(0, 0, 0, 0.25);
  line-height: 1.25;
  word-spacing: 0px;
  padding: 35px 0;
  position: relative;
  z-index: 2;
}
.bundle-title {
  font-weight: 900;
  text-align: center;
  font-size: 1.25em;
  margin: 0 auto 20px auto;
}
.bundle-games {
  margin: 30px auto;
  text-align: center;
}
.bundle-games .game:first-child {
  margin-left: 0;
}
.bundle-games .game {
  margin-left: 7px;
  width: 25vw;
  position: relative;
  display: inline-block;
}
.buy-button-container {
  margin-top: 20px;
  text-align: center;
}
.buy-button {
  background-color: rgba(0, 0, 0, 0.05);
  height: 29px;
  padding: 3px 10px;
  color: white;
  font-family: 'Lato';
  font-weight: 900;
  font-size: 17.5px;
  line-height: 1.05;
  word-spacing: 0px;
  border: 1px solid white;
}
.buy-button:hover {
  color: #424242;
  background-color: white;
}
.summary {
  margin-top: 12px;
  line-height: 17px;
  font-size: 14px;
}
</style>
