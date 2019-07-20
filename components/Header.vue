<template>
  <nav class="navbar is-fixed-top itchio-navbar">
    <div class="navbar-brand itchio-navbar-brand">
      <button class="mobile-nav-button">
        <div class="mobile-nav-icon">
          <div class="mobile-nav-bar"></div>
          <div class="mobile-nav-bar"></div>
          <div class="mobile-nav-bar"></div>
        </div>
      </button>
      <a class="navbar-item header-logo-container">
        <img class="header-logo" src="~/assets/logo-black-new.svg"/>
      </a>
      <div class="login-container">
        <button class="button login-button">Log in</button>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.itchio-navbar {
  box-shadow: 0 1px 2px rgba(0,0,0,0.1);
  min-height: 3rem;
  height: 50px;
}
.itchio-navbar-brand {
  min-height: 3rem;
}
.mobile-nav-button {
  background: none;
  display: block;
  padding: 16px 20px;
  border: 0;
}
.mobile-nav-button .mobile-nav-icon {
  position: relative;
  height: 17px;
  width: 25px;
  margin-top: 1px;
}
.mobile-nav-icon .mobile-nav-bar:first-child {
  bottom: auto;
}
.mobile-nav-icon .mobile-nav-bar:last-child {
  top: auto;
}
.mobile-nav-icon .mobile-nav-bar {
  background: #222222;
  position: absolute;
  height: 3px;
  margin: auto;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
}
.header-logo-container {
  padding: 0;
}
.header-logo {
  max-height: 2rem;
  height: 30px;
  width: 117px;
}
.login-container {
  margin: auto 10px auto auto;
  text-align: center;
}
.login-button {
  height: 30px;
  padding: 0 15px;
  line-height: 26px;
  font-family: 'Lato';
  font-size: 14px;
  font-weight: bold;
  word-spacing: 0px;
  border: 2px solid;
  border-color: #dadada;
  border-radius: 3px;
}
.login-button:hover {
  color: #ff2449;
}
</style>
