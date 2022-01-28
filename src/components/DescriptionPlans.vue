<template>
  <p class="text-green-900 p-3 font-bold bg-white rounded">{{ name }}</p>
</template>
<script>
export default {
  name: 'DescriptionPlans',
  props: {
    name: { type: String }
  }
}
</script>
<style scoped>
p {
  transition: 200ms;
}
p:hover {
  box-shadow: 0 2px 4px #00000080;
}
</style>
