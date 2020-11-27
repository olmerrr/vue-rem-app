<template>
  <ul>
    <lerning-resources
      v-for="res in resources"
      :key="res.id"
      :id="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    >
    </lerning-resources>
  </ul>
</template>

<script>
import LerningResources from "./LerningResources";

export default {
  inject: ["resources"],
  components: {
    LerningResources,
  },
};
</script>
<style scoped>
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
    margin: auto;
    max-width: 40rem;
  }
</style>