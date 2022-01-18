<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div class="">
      <span class="text-success fs-3 fw-bold"> 15 </span>
      <span class="mx-1 fs-3"> Julio </span>
      <span class="mx-2 fs-4 fw-light"> 2021, jueves </span>
    </div>

    <div class="">
      <button class="btn btn-danger mx-2">
        Borrar
        <li class="fa fa-trash-alt"></li>
      </button>
      <button class="btn btn-success">
        Subir fotos
        <li class="fa fa-upload"></li>
      </button>
    </div>
  </div>
  <hr />
  <div class="d-flex-column px-3 h-75">
    <textarea placeholder="¿Qué sucedió hoy?"> </textarea>
  </div>
  <Fab></Fab>

  <img
    class="img-thumbnail"
    src="https://i0.wp.com/hipertextual.com/wp-content/uploads/2017/02/Universo-1.jpg?fit=700%2C369&ssl=1"
    alt=""
  />
</template>

<script>
import { defineAsyncComponent } from "@vue/runtime-core";
export default {
  components: {
    Fab: defineAsyncComponent(() => import("../components/Fab")),
  },
};
</script>

<style scoped lang="scss">
textarea {
  font-size: 20px;
  border: none;
  height: 100%;
  &:focus {
    outline: none;
  }
}

img {
  width: 250px;
  position: fixed;
  bottom: 150px;
  right: 20px;
  box-shadow: 0px 5px 10 px rgba(#0000, 0.2);
}
</style>