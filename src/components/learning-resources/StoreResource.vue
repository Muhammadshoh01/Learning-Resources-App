<template>
  <ul>
    <stored-resources
      v-for="resource in resources"
      :key="resource.id"
      :id="resource.id"
      :title="resource.title"
      :description="resource.description"
      :link="resource.link"
    ></stored-resources>
  </ul>
</template>

<script>
import StoredResources from './StoredResources.vue';

export default {
  components: { StoredResources },
  inject: ['resources'],
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
