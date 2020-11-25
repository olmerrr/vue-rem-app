<template>
  <ul>
    <lerning-resurces v-for="res in storedResources" 
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
    >
    </lerning-resurces>
  </ul>
</template>

<script>
import LerningResurces from "./components/lerning-resources/LerningResurces";

export default {
  components: {
    LerningResurces,
  },
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The official Vue.js documentation.",
          link: "https://vue.js.org",
        },
        {
          id: "google",
          title: "Google",
          description: "Lern to Google...",
          link: "https://google.org",
        },
      ],
    };
  },
};
</script>