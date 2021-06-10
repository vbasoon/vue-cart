<template>
  <div id="nav">
    <router-link :class="{ active: $route.name === 'Home' }" to="/"
      >Home</router-link
    >
    |
    <router-link :class="{ active: $route.name === 'Cart' }" to="/cart"
      >Cart</router-link
    >
  </div>
  <router-view />
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.text-center {
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 10px;
  width: 100%;
  height: 30px;
  background-color: whitesmoke;
  line-height: 30px;

  a {
    font-weight: bold;
    color: darkgrey;
    text-decoration: none;
    margin: 0 5px 0 5px;
    font-size: 1.25rem;

    &.active {
      color: #2c3e50;
    }
  }
}

html,
body {
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}

body {
  background-color: rgb(245, 245, 245);
}
</style>
