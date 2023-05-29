<template>
  <main>
    <card :title="'Creat User'" @backhome="back" />
  </main>
</template>

<script>
import Card from "../components/Card.vue";
export default (await import("vue")).defineComponent({
  components: {
    Card,
  },
  methods: {
    back() {
      this.$router.go(-1);
    },
  },
});
</script>
