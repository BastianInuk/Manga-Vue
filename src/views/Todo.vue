<template>
  <h1>Here's my personal todos</h1>
  <TodoView todos="currentTodo"/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import TodoView, { TodoType } from '@/components/TodoView.vue';

function getTodo() {
  return { currentTodo: [new TodoType(1, 'I need to get it done!')] };
}

export default defineComponent({
  name: 'Todo',
  components: {
    TodoView,
  },
  data: getTodo,
});
</script>:w
