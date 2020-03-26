<template>
  <div class="content login">
    <div class="columns">
      <div class="flex-center bg-secondary">
        <div class="logo">
           <img src="https://image.flaticon.com/icons/svg/679/679821.svg" alt="">
            <h1>ProjectBox</h1>
        </div>
      </div>
      <div class="flex-center bg-primary">
        <div class="card bg-secondary">
          <h1 class="title">Login</h1>
          <form action="">
            <input placeholder="Usuário" />
            <button @click="$emit('onLogin')" class="full-width">
              Entrar
            </button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageLogin"
}
</script>

<style>

.card {
  width: 300px;
  height: auto;
  padding: 1em;
  border-radius: 8px;
}

.card .title {
  font-size: 24px;
  margin-bottom: 16px;
}

.login .card {
  height: 180px;
}

.logo {
  height: 180px;
  text-align: center;
}

.logo img {
  height: calc(100% - 38px)
}

input {
  width: 100%;
}

button {
  background-color: #49FF78;
}

</style>