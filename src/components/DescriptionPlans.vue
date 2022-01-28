<template>
  <p class="btn btn-primary p-3">{{ name }}</p>
</template>
<script>
export default {
  name: 'DescriptionPlans',
  props: {
    name: { type: String }
  }
}
</script>
<style scoped></style>
