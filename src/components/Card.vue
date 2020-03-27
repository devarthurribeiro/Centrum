<template>
  <div class="card bg-secondary">
    <h1 v-if="title" class="title">{{title}}</h1>
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: ['title']
}
</script>

<style>
.card {
  width: 100%;
  height: auto;
  padding: 1em;
  border-radius: 8px;
}

.card .title {
  font-size: 24px;
  margin-bottom: 16px;
}
</style>