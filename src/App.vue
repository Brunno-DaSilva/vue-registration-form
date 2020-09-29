<template>
  <div class="app">
    <div class="app__container">
      <div class="container__left"></div>
      <div class="container__right">
        <Login />
      </div>
    </div>
  </div>
</template>

<script>
  import Login from "./components/Login.vue";

  export default {
    name: "App",
    components: {
      Login,
    },
  };
</script>

<style>
  *,
  *::before,
  *::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    overflow: hidden !important;
  }
  #app {
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .app {
    border: 1px solid tomato;
    margin: 3rem;
  }
  .app__container {
    min-height: 80%;
    background: #2c3e50;
  }
</style>
