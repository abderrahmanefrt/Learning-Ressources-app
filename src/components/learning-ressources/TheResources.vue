<template>
  <base-card>
    <base-button @click="setselectedTab('StoredRessources')">Stored Resources</base-button>
    <base-button @click="setselectedTab('AddResource')">Add resources</base-button>
    <component :is="selectedTab" :resources="storedResources"></component>
  </base-card>
</template>

<script>
import StoredRessources from './StoredRessources.vue'
import AddResource from './AddResource.vue'

export default {
  components: {
    AddResource,
    StoredRessources
  },
  data() {
    return {
      selectedTab: 'StoredRessources',
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'the official guide to the Vue js',
          link: 'https://vuejs.org/guide',
        },
        {
          id: 'google',
          title: 'google',
          description: 'Learn to google',
          link: 'https://google.com',
        },
      ]
    };
  },
  methods: {
    setselectedTab(tab) {
      this.selectedTab = tab;
    }
  }
}
</script>

