<template>
  <div class="app">
    <nav>
      <router-link to="/">Home</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  background-color:ghostwhite;
}
#app{
     font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      width: 100%;
      max-width: 600px;
      margin: 0px auto;
}


</style>
