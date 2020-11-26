<template>
  <base-card>
    <base-button @click="selectedTab('stored-resources')">Stored Resurces</base-button>
    <base-button @click="selectedTab('add-resource')">Add Resurce</base-button>
  </base-card>
  <component :is="selectedTab"></component>
  <!-- <stored-resources></stored-resources>
  <add-resource></add-resource> -->
</template>

<script>
import StoredResources from './StoredResources'; 
import AddResource from './AddResource'; 
import AddResource from './AddResource .vue';

export default {
  components: {
    StoredResources,
    AddResource
    AddResource
  },
  data() {
    return {
      selectedTab: 'stored-resources'
    };
  },
  methods: {
    setSelectedTab(tab) {
      this.selectedTab = tab
    },
  },
  };
</script>

