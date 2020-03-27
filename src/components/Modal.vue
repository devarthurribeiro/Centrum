<template>
  <div v-if="show" class="modal">
    <div @click="$emit('update:show', false)" class="overlay">
      <div class="modal-content">
        <Card :title="title">
          <slot />
        </Card>
      </div>
    </div>
  </div>
</template>

<script>
import Card from './Card';

export default {
  name: 'Modal',
  props: ['show', 'title'],
  components: {
    Card
  }
}
</script>

<style>
.overlay {
  position: fixed;
  width: 100%;
  height: 100vh;
  z-index: 2;
  background-color: rgba(0, 0, 0, 0.5);
}
.modal {
  position: absolute;
  min-width: 400px;
  width: 100%;
  height: 100vh;
  z-index: 999;
}

.modal .modal-content {
  margin: 200px auto;
  width: 400px;
}

.modal::after {
  content: "";
  background-color: red;
}
</style>