<template>
  <div class="flex flex-col gap-3 w-1/2">
    <DescriptionPlans v-for="plan in plans" :key="plan" :name="plan"></DescriptionPlans>
  </div>
</template>
<script>
import DescriptionPlans from './DescriptionPlans.vue'
export default {
  name: 'PlanPicker',
  components: {
    DescriptionPlans
  },
  data() {
    return {
      plans: ['The Single', 'The Curious', 'The Addict']

    }
  },
  props: {
    plan: { type: String }
  }
}
</script>
<style scoped>
h1 {
  @apply font-sans font-bold my-2 text-5xl;
}
h1 {
  @apply font-sans font-bold my-2 text-lg;
}
</style>
