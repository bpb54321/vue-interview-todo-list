<script setup lang="ts">
import { type Todo } from '@/types/Todo';
defineProps<{
  todo: Todo,
}>()
</script>

<template>
  <li>{{ todo.title }}</li>
</template>
