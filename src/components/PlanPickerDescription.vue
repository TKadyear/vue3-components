<template>
  <p
    @click="select"
    :class="[selected ? 'text-white bg-[#2c3e50] ' : 'text-[#2c3e50] bg-white ', 'rounded font-bold p-3']"
  >{{ name }}</p>
</template>
<script>
export default {
  name: 'PlanPickerDescription',
  props: {
    name: { type: String },
    selected: { type: Boolean, default: false }
  },
  methods: {
    select() {
      this.$emit('select', this.name)
    }
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
