<template>
  <ul>
    <li>
      <h1>{{ title }}</h1>
      <h2>{{ description }}</h2>
      <a :href="link">View Resource</a>
    </li>
  </ul>
</template>

<script>
export default {
  props: ['title', 'description', 'link'],
};
</script>
