<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>
  <Fab icon="fa-plus"></Fab>
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  components: {
    Fab: defineAsyncComponent(() => import("../components/Fab")),
  },
};
</script>

<style scoped lang="scss">
div {
  height: 100%;
}
</style>