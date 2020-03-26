<template>
  <div id="app">
    <Login v-if="showLogin" @onLogin="login" />
    <Dashboard v-else />
  </div>
</template>

<script>
import Login from './pages/login';
import Dashboard from './pages/dashboard';

export default {
  name: 'App',
  data: () =>({
    showLogin: true
  }),
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Login,
    Dashboard
  },
  methods: {
    login() {
      this.showLogin = false
    }
  },
}
</script>

<style src="./styles/global.css" />
