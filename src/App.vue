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
    background-image: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
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
    width: 80%;
    min-height: 80%;
    margin: 3rem;
    /* box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24); */
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
  }
  .app__container {
    min-height: 80%;
  }
</style>
