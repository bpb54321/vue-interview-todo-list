<script setup lang="ts">
import { ref } from 'vue'
const title = ref('')
function addTodo(event: Event) {
  event.preventDefault()
  console.log(title.value);
}
</script>

<template>
  <form @submit="addTodo">
    <input type="text" id="new-todo-title" placeholder="The title of the todo" v-model="title" />
    <input type="submit" value="Add"/>
  </form>
</template>
