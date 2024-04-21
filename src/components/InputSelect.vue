<script setup>
defineProps({
  label: String,
})
const model = defineModel()
</script>

<template>
<label class="block">
<span class="text-gray-700">{{ label }}</span>
<select class="block w-full mt-1 rounded-md border-gray-300 shadow-sm focus:border-indigo-300 focus:ring focus:ring-indigo-200 focus:ring-opacity-50" v-model="model">
    <option>Corporate event</option>
    <option>Wedding</option>
    <option>Birthday</option>
    <option>Other</option>
</select>
</label>
</template>