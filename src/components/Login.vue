<template>
  <div>
    <div class="login">
      <input className="form-input" type="text" />
      <label class="form-input-label">Email</label>
    </div>
    <div class="login">
      <input className="form-input" type="text" />
      <label class="form-input-label">Password</label>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Login",
  };
</script>

<style lang="scss">
  $sub-color: #9b9b9b;
  $main-color: #252525;

  @mixin shrinkLabel {
    top: -2px;
    font-size: 12px;
    color: $main-color;
  }
  .login {
    position: relative;
    margin: 45px 0;

    .form-input {
      background: none;
      background-color: #ffffff;
      color: #444444;
      font-size: 18px;
      padding: 1rem;
      display: block;
      width: 100%;
      border: none;
      border-radius: 0;
      border-bottom: 1px solid $sub-color;
      margin: 25px 0;

      &:focus {
        outline: none;
      }

      &:focus ~ .form-input-label {
        @include shrinkLabel();
        color: $sub-color;
      }
    }

    input[type="password"] {
      letter-spacing: 0.3em;
    }

    .form-input-label {
      color: $sub-color;
      font-size: 16px;
      font-weight: normal;
      position: absolute;
      pointer-events: none;
      left: 5px;
      top: 10px;
      transition: 300ms ease all;

      &.shrink {
        @include shrinkLabel();
        color: $sub-color;
      }
    }
  }
</style>
