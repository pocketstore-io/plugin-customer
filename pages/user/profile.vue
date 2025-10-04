<template>
  <section class="bg-white xl:mx-auto mx-3 px-3 py-3 max-w-6xl">
    User {{ route.query.id ?? 'Id Missing' }}
  </section>
</template>

<script setup lang="ts">
import { useRoute } from 'vue-router'
const route = useRoute()
</script>