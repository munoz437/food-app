<template>
  <div id="app">
    <div class="navbar-container">
      <div class="navbar-content">
        
          <router-link to="/">
            <i class='bx bx-home-alt bx-sm' ></i>
          </router-link>

          <router-link to="/mas">
          <i class='bx bx-message-square-detail bx-sm' ></i>
          </router-link>
          <!--
          <router-link to="/deseos">
            <i class='bx bx-heart bx-sm' ></i>
          </router-link> hola-->

        
          <router-link to="/usuario">
          <i class='bx bx-user bx-sm' ></i>
          </router-link>

          

          
      </div>
    </div>

    <router-view/>
  </div>
</template>

<style lang="less">

.navbar-container{
  width: 100%;
  position: fixed;
  bottom: 0;

  .navbar-content{
    padding: 20px;
    display: flex;
    justify-content: space-between;
    a{
      color: rgba(163,163,163);
      &.router-link-exact-active {
      color:rgba(255,131,62);
    }

    }

  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
}
*{
  font-family: 'Josefin Sans', sans-serif;
  margin: 0px;
  padding: 0px;
}
</style>
