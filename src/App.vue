<template>
  <div id="app">
    <div id="nav">
      <router-link class="a" to="/">แสดงข้อมูลทั้งหมด</router-link> 
    </div>
    <router-view/>
  </div>
</template>

<style>
.a {
  background-color: #ffff00; /* Green */
  border: none;
  color: rgb(252, 237, 237);
  padding: 15px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.a {border-radius: 12px;}

#app {
  background-repeat: no-repeat;
  background-size: auto;
  background-color: #e0fdb0; 
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
