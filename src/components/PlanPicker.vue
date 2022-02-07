<template>
  <div class="flex flex-col gap-3 w-1/2">
    <PlanPickerDescription
      v-for="plan in plans"
      v-on:select="selectPlan"
      :selected="plan === selectedPlan"
      :key="plan"
      :name="plan"
    ></PlanPickerDescription>
  </div>
</template>
<script>
import PlanPickerDescription from './PlanPickerDescription.vue'
export default {
  name: 'PlanPicker',
  components: {
    PlanPickerDescription
  },
  data() {
    return {
      plans: ['The Single', 'The Curious', 'The Addict'],
      selectedPlan: null

    }
  },
  methods: {
    selectPlan(plan) {
      this.selectedPlan = plan
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
