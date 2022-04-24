<template>
  <h1>Welcome to the forum!</h1>
  <ThreadList :threads="threads" />
</template>
<script>
  import ThreadList from "@/components/ThreadList";
  import data from "@/data.json";
  export default {
    components: {
      ThreadList,
    },
    data() {
      return {
        threads: data.threads,
      };
    },
  };
</script>

<style scoped></style>
