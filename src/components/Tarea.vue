<template>
  <li class="list-group-item">
    {{ nombreTarea }}

    <button @click="eliminar" class="btn btn-danger ml-auto">eliminar</button>
  </li>
</template>

<script>
export default {
  props: ["nombreTarea"],
  methods: {
    eliminar() {
      this.$emit("myEvent", null);
    },
  },
};
</script>

<style></style>
