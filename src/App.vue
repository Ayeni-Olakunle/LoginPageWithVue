<template>
  <div id="app">
    <div id="nav">
      <b-container class="bv-example-row">
        <b-row>
          <b-col sm="6">
            <img src="./assets/Work 05.jpg" alt="" class="img">
          </b-col>
          <b-col sm="6">
            <router-view/>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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

.img{
  width: 100%;
  height: 550px;
}
</style>
