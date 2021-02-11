<template>
  <div class="app">
    <div class="app__container">
      <div class="container__left">
        <img
          src="./assets/North-left-img-01.svg"
          alt="main registration picture"
        />
      </div>
      <div class="container__right">
        <div class="registration">
          <div class="registration__img">
            <img src="./assets/logocampass.png" />
          </div>
        </div>

        <form>
          <Login />
        </form>
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
    background-color: #085575;
    background-image: linear-gradient(225deg, #085575 0%, #20cd7e 100%);
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
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
    background: #ffffff;
  }

  .app__container {
    width: 100%;
    height: 50rem;
    display: flex;
    justify-content: flex-start;
    align-items: center;
  }

  .container__right,
  .container__left {
    width: 72%;
    height: 100%;
  }

  .container__left {
    width: 38%;
  }
  .container__left img {
    width: 100%;
    height: 50rem;
    object-fit: cover;
  }

  .container__right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .container__right form {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 70%;
  }
</style>
