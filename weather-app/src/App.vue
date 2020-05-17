<template>
  <div id="app" class="app">
    <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>
    <main>
      <div class="container">
        <router-view />
        <form class="form-inline my-2 my-lg-0">
          <input
            class="form-control mr-sm-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      apiKey: "274eb1179f56f14a7296cacd9d3d352d"
    };
  }
};
</script> 
<style lang="scss">
#app {
  background: url(./assets/img/winter.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: bottom;
  transition: 0.4;
  height: 100vh;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
main {
  min-height: 100vh;
  min-width: 100vw;
  background-image: linear-gradient(
    to bottom,
    rgba(0, 0, 0, 0.25),
    rgba(0, 0, 0, 0.75)
  );
}
</style>
