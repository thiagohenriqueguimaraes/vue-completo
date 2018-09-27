<template>
  <div id="app">

    <nav class="navbar navbar-expand-md navbar-dark bg-dark fixed-top">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExampleDefault" aria-controls="navbarsExampleDefault" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarsExampleDefault"></div>
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
                  <router-link class="nav-link" to="/">Home</router-link> |
            <!-- <a class="nav-link" href="\">Home <span class="sr-only">(current)</span></a> -->
          </li>
          <li class="nav-item">
            <a class="nav-link" href="\about">About</a>
          </li>
        </ul>
      </div>
    </nav>


    <div id="nav">
      <router-link class="nav-link" to="/">Home</router-link> |
      <router-link to="/about">Sobre</router-link> |
      <router-link to="/produto">Produtos</router-link>
    </div>
    <router-view/>
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
