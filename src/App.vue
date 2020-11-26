<template>
  <the-header title="RememberMe"></the-header>
</template>

<script>
// import StoredResources from './components/lerning-resources/StoredResources'; 
import TheHeader from './components/loyouts/TheHeader';

export default {
  components: {
    TheHeader,
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

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>