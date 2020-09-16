<template>
  <div>
    CompA
    <CompB></CompB>
  </div>
</template>

<script>
import CompB from "./CompB";
export default {
  components: {
    CompB,
  },
  provide() {
    return {
      change: this.change,
    };
  },

  methods: {
    change(msg) {
      console.log(msg);
    },
  },
};
</script>

<style scoped></style>
