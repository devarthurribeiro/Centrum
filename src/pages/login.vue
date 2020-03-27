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
        <Card style="height: 180px;" title="Login">
          <input placeholder="Usuário" />
          <button @click="$emit('onLogin')" class="full-width">
              Entrar
          </button>
        </Card>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '../components/Card';

export default {
  name: "PageLogin",
  components: {
    Card
  }
}
</script>

<style>
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