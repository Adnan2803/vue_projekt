<template>
  <div id="app">
    <div id="nav">
      <nav class="navbar navbar-light bg-light">
        <div class="col-4">
          <a class="navbar-brand" href="#">
            <img
              src="@/assets/logo.svg"
              width="30"
              height="30"
              class="d-inline-block align-top"
              alt
            />
            Instagram
          </a>
        </div>
        <div class="col-4">
          <div id="search-center">
            <div class="input-group">
              <input
                type="text"
                class="form-control input-lg"
                placeholder="Search"
                style="margin-left: 100px; margin-right: 100px;"
              />
            </div>
          </div>
        </div>
        <div class="col-4">
          <router-link to="/home" class="d-inline-block align-top" style="margin-right: 30px;">
            <img src="@/assets/compass.svg" width="30" height="30" alt />
          </router-link>
          <router-link to="/login" class="d-inline-block align-top" style="margin-right: 30px;">
            <img src="@/assets/heart.svg" width="30" height="30" alt />
          </router-link>
          <router-link to="/signup" class="d-inline-block align-top">
            <img src="@/assets/user.svg" width="30" height="30" alt />
          </router-link>
        </div>
      </nav>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
input {
  text-align: center;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  border-bottom: 1px solid black;
  margin-bottom: 50px;
  margin-left: 9%;
  margin-right: 9%;
  a {
    font-weight: bold;
    color: rgba(0, 0, 0);
    font-family: "Kaushan Script", cursive;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
