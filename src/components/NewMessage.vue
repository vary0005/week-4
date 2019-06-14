<template>
  <div class="practice">
    <h2>Hello {{ name }}</h2>
    <ul>
      <li>Age: {{age }}</li>
      <li>{{ treat }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ['treat'],
  data() {
    return {
      name: 'Vue',
      age: 6,
      color: 'Black',
    };
  },
};
</script>
<style lang="scss">
h2 {
  color: coral;
}
</style>
