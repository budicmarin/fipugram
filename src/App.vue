<template>
  <div id="app">

    <nav class="navbar navbar-expand-lg navbar-light bg-light mb-5">
      <router-link class="navbar-brand" to="/">Our App</router-link>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
    
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li>Todo stranica</li>
        </ul>
        <router-link  class="btn btn-info my-2 my-sm-0 mr-2" to="/login">Login</router-link>
        <span>
          
          <a  class="btn btn-info my-2 my-sm-0 mr-2" href="#">Logout</a>
        </span>
        <router-link class="btn btn-outline my-2 my-sm-0 mr-2" to="/signup">Signup</router-link>
      </div>
    </nav>

    <router-view/>

    <div id="footer" class="text-center mt-5">Ovo je footer. (c) 2019 mi svi skupa.</div>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  background-color: white important;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
