<script setup>
import { brand } from "../config/brand";
defineProps({ iconOnly: Boolean });
</script>
<template>
  <span class="brand-lockup"
    ><svg viewBox="0 0 48 48" fill="none" aria-hidden="true">
      <path
        d="M18 8H8V18M30 8H40V18M8 30V40H18M40 30V40H30"
        stroke="currentColor"
        stroke-width="3"
        stroke-linecap="square"
      />
      <path
        d="M18 18H30V30H18Z"
        fill="currentColor"
      /></svg
    ><span v-if="!iconOnly">{{ brand.name }}</span></span
  >
</template>
