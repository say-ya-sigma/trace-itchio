<template>
  <div class="outer">
    <section class="sub-navigation-section">
      <div class="tab-container">
        <a class="header-tab">All Games</a>
        <a class="header-tab">Game jams</a>
        <a class="header-tab">Devlogs</a>
        <a class="header-tab">Community</a>
        <a class="header-tab">Bundles</a>
      </div>
    </section>
  </div>
</template>

<style scoped>
.outer {
  height: 50px;
  border-bottom: 1px;
}
.sub-navigation-section {
  height: 49px;
  width: 100%;
  padding: 0 10px 0 13px;
  font-family: 'Lato';
  font-weight: bold;
  line-height: 1.25;
  word-spacing: 0px;
  overflow-x: auto;
  white-space: nowrap;
  border-color: #dadada;
  display: flex;
  justify-content: center;
  align-items: center;
}
.tab-container {
  width: 100%;
  margin-top: -4px;
}
.header-tab {
  margin-right: 20px;
  margin-left: -3px;
  padding: 12px 0;
  color: #222222;
}
.header-tab:hover {
  color: #da2c49;
  border-bottom: 4px solid #ff2449;
}
</style>
