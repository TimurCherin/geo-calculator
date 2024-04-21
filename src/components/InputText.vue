<script setup>
defineProps({
  label: String,
})
const model = defineModel()
</script>

<template>
  <label class="block">
    <span class="text-gray-700">Full name</span>
    <input type="text" class="mt-1 block w-full rounded-md border-gray-300 shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50" placeholder="" v-model="model">
  </label>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
