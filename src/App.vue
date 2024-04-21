<script setup>
import InputText from './components/InputText.vue'
import InputSelect from './components/InputSelect.vue'
import { ref } from 'vue'
const srs = ref("")
const textValue = ref("")
</script>

<template>
  <div class="py-12">
          <h2 class="text-2xl font-bold">Simple</h2>
          <div class="mt-8 max-w-md">
            <div class="grid grid-cols-1 gap-6">
              <InputText v-model="textValue"/>
              {{ textValue }}
              <InputSelect label="Вхідна система кординат" v-model="srs"/>
              {{ srs }}
            </div>
          </div>
        </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
