<template>
  <div class="content bg-primary">
    <div class="columns">
      <div class="sidenav bg-secondary">
        <div class="logo flex-center">
          <h1>ProjectBox</h1>
          <img src="https://image.flaticon.com/icons/svg/679/679821.svg" alt="">
        </div>
      </div>
      <main>
        <h1 class="page-title">Projetos</h1>
        <div class="grid-3">
          <div class="card card-project bg-secondary">
            <header>
              <img src="https://image.flaticon.com/icons/svg/544/544578.svg" alt="">
              <h1 class="title">RocketApi</h1>
            </header>
            <p>
              A free, fast and beautiful API builder 🚀
            </p>
          </div>
        </div>
      </main>
      <div class="sidenav rigth bg-secondary">
        <div class="menu">
          <div class="avatar">
            <button class="bg-primary">AR</button>
          </div>
          <button>+</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

main {
  padding: 1em;
  margin-top: 1em;
  width: 100%;
}

.sidenav {
  display: flex;
  width: 285px;
  padding: 1em;
}

.avatar button {
  color: #4FFA7B;
  border-radius: 50%;
}

.sidenav.rigth {
  width: 76px;
  padding: 1em;
}

.sidenav.rigth .menu {
  display: flex;
  flex: 1;
  justify-content: space-between;
  flex-direction: column;
}

.sidenav .logo {
  margin-top: 1em;
  height: 60px;
}

.sidenav .logo img {
  height: 60px;
  margin-left: 8px;
}
.card-project header {
  display: flex;
  flex: 1;
  flex-direction: row;
}

.card-project header img {
  width: 65px;
  height: 65px;
  margin-right: 1em;
}

.card-project .title {
  line-height: 65px;
}
</style>