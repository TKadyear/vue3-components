<template>
  <div class="content flex flex-col justify-center w-2/4 m-auto gap-3">
    <h1>Coffee Plans</h1>
    <h2>We travel the world to surce the very best single origin coffee for you</h2>
    <ButtonPlans v-for="plan in plans" :key="plan" :name="plan"></ButtonPlans>
    <ButtonPlans name="The Single"></ButtonPlans>
    <ButtonPlans name="The Curious"></ButtonPlans>
    <ButtonPlans name="The Addict"></ButtonPlans>
  </div>
</template>
<script>
import ButtonPlans from './ButtonPlans.vue'
export default {
  name: 'PlansCoffee',
  components: {
    ButtonPlans
  },
  data() {
    return {
      plans: ['The Single', 'The Curious', 'The Addict']

    }
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
