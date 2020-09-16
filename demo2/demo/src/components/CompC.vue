<template>
  <div>
    CompC
    <input type="text" v-model="value" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: "",
    };
  },
  inject: ["change"],
  watch: {
    value(newVal) {
      this.change(newVal);
    },
  },
};
</script>

<style scoped></style>
