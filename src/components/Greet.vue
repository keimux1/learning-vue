<template>
  <div>
    <button @click="counter++">{{ counter }}</button>
    <h2 v-bind:id="$attrs.id">
      hello {{ name }} aka {{ heroname }} {{ phoneNumber }}
      isPublished-{{ isPublished ? 'yes' : 'no' }}
    </h2>
  </div>
</template>

<script setup>
import { ref, defineProps } from "vue";

const counter = ref(0);
defineProps({
  name: String,
  heroname: String,
  phoneNumber: Number,
  isPublished: Boolean,
});

defineOptions({
    inheritAttrs: false,
})
</script>
