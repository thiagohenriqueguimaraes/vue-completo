<template>
  <div id="app">

    <nav class="navbar navbar-expand-md navbar-dark bg-dark fixed-top">
      <a class="navbar-brand" href="#">Vue</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExampleDefault" aria-controls="navbarsExampleDefault" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarsExampleDefault"></div>
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
             <router-link class="nav-link" to="/"><span class="sr-only">(current)</span>Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Sobre</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/produto">Produtos</router-link>
          </li>
          <li class="nav-item">
            <router-link class="btn btn-sm btn-light" to="/login">Log in</router-link>
          </li>
        </ul>
    </nav>
    <router-view/>


    <!-- <div id="nav">
      <router-link class="nav-link" to="/">Home</router-link> |
      <router-link to="/about">Sobre</router-link> |
      <router-link to="/produto">Produtos</router-link>
    </div>
    <router-view/> -->
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
