<template>
  <router-view />
</template>

<script>
import { mapState } from "vuex";

export default {  
  created() {
    
  },
  computed: mapState(["listVideos"]),
};
</script>


<style lang="scss">
*{
  margin: 0;  
  padding: 0;
  border: 0; 
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  position: fixed;
  top: 0;  
  bottom: 0;
  height: 100vh;
  overflow-y: auto;
  width: 100%;
  background-image: url(./assets/bg.jpg);  
  background-repeat: no-repeat;
  background-position: left top;
  background-attachment: fixed;
  background-size: cover;
  padding: 50px 0 0 0;
  display: flex;
  flex-direction: column;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
