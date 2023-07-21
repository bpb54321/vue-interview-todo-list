<script setup lang="ts">
import { type Todo } from "@/types/Todo"
import TodoItem from "@/components/TodoItem.vue";
import AddTodoForm from "@/components/AddTodoForm.vue"
const todos: Todo[] = [
  {
    title: "Faire mes valises",
    id: "0",
  },
  {
    title: "Laver la vaisselle",
    id: "1",
  },
  {
    title: "Aller à l'épicerie",
    id: "2",
  },
]
</script>

<template>
  <ul>
    <TodoItem v-for="todo in todos" :key="todo.id" :todo="todo"/>
  </ul>
  <AddTodoForm />
</template>
