<template>
  <section>
    <div class="navbar is-inline-flex is-transparent">
      <div class="navbar-brand">
        <a class="navbar-item">
          <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28" alt="Bulma">
        </a>
      </div>
      <div class="navbar-menu">
        <div class="navbar-item">
          <div class="control has-icons-left">
            <input class="input is-small has-text-centered" type="text" placeholder="search">
            <span class="icon is-left is-small">
              <i class="material-icons">search</i>
            </span>
          </div>
        </div>
      </div>
      <div class="navbar-item is-flex-touch">
        <a class="navbar-item">
          <i class="material-icons">explore</i>
        </a>
        <a class="navbar-item">
          <i class="material-icons">favorite_border</i>
        </a>
        <a class="navbar-item">
          <i class="material-icons">person_outline</i>
        </a>
      </div>
    </div>
    <div>
      <nuxt/>
    </div>
  </section>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
