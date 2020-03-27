<template>
  <Card>
    <div class="card-project">
      <header>
        <img :src="project.img" alt="project logo" />
        <h1 class="title">{{project.name}}</h1>
      </header>
      <p>{{project.description}}</p>
    </div>
  </Card>
</template>

<script>
import Card from '../components/Card';

export default {
  name: "CardProject",
  props: ['project'],
  components: {
    Card
  }
}
</script>

<style>
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