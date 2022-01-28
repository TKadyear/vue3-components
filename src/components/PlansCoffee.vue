<template>
  <div class="content flex flex-col justify-center w-2/4 m-auto">
    <h1>Coffee Plans</h1>
    <h2>We travel the world to surce the very best single origin coffee for you</h2>
    <PlanPicker></PlanPicker>
  </div>
</template>
<script>
import PlanPicker from './PlanPicker.vue'
export default {
  name: 'PlansCoffee',
  components: {
    PlanPicker
  }
}
</script>
<style scoped>
h1 {
  @apply font-sans font-bold my-2 text-5xl;
}
h2 {
  @apply font-sans font-bold my-2 text-lg;
}
</style>
