<template>
  <div class="home">
    <button @click="goToDayBook" type="button" class="btn btn-primary">Primary</button>
    <button type="button" class="btn btn-secondary">Secondary</button>
    <button type="button" class="btn btn-success">Success</button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  methods: {
    goToDayBook() {
      this.$router.push({ name: "no-entry" });
    },
  },
};
</script>
