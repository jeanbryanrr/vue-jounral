<template>
  <div
    @click="$router.push({ name: 'entry', params: { id: 10 } })"
    class="entry-container mb-3 poiner p-2"
  >
    <div class="entry-title d-flex">
      <span class="text-success fs-5 fw-bold">15</span>
      <span class="mx-1 fs-5">Julio</span>
      <span class="m-2 fw-light">2021, jueves</span>
    </div>
    <div class="entry-description">
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolore deleniti
      quaerat reiciendis nemo saepe? Debitis, eveniet? Expedita, magni nostrum
      atque exercitationem, laboriosam saepe possimus molestiae obcaecati quae,
      quo debitis optio!
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped >
.entry-container {
  border-bottom: 1px solid #2c3e50;
  transition: 0.3 all ease-in;
  &:hover {
    background-color: lighten(gray, 45%);
  }
  .entry-description {
    font-size: 12px;
  }
}
</style>