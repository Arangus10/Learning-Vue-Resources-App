<template>
  <ul>
    <li v-for="resource in storedResources" :key="resource">
        {{ resource }}
    </li>
  </ul>
</template>

<script>
export default {
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
