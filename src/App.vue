<template>
  <ul>
        <learning-resource v-for="res in storedResources" :key="res.id">
            {{ res }}
        </learning-resource>
  </ul>
</template>

<script>
import LearningResource from './components/learning-resources/learning-components/LearningResource.vue'
export default {
components: {
    LearningResource
},
  data() {
    return {
      storedResources: [
        {
            id:'official-guide',
            title: 'Official Guide',
            description: 'The Official Vue.js documentation',
            link: 'https://vuejs.org'
        },
        {
            id:'google',
            title: 'Google',
            description: 'Learn Vue from Google',
            link: 'https://google.org'
        }
      ],
    };
  },
};
</script>
