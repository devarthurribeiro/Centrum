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
          <CardProject v-for="project in projects" :project="project" :key="project.name" />
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
import CardProject from '../components/CardProject';

export default {
  name: 'Dashborad',
  data: () => ({
    projects: [
      {
        name: "RocketApi",
        description: "A free, fast and beautiful API builder 🚀",
        img: "https://image.flaticon.com/icons/svg/544/544578.svg"
      },
      {
        name: "COVID19 Brazil API",
        description: "API com dados atualizados sobre o status do COVID-19 🦠",
        img: "https://github.com/devarthurribeiro/covid19-brazil-api/raw/master/api/public/logo.svg?sanitize=true"
      },
      {
        name: "CoronaReport",
        description: "Reports about COVID19",
        img: "https://image.flaticon.com/icons/svg/2746/2746595.svg"
      }
    ]
  }),
  components: {
    CardProject
  }
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

</style>