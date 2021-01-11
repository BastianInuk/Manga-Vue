<template>
    <div v-for="todo in todos" :key="todo.id">
        <p>{{todo.text}}</p>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export class TodoType {
  id: number;

  text: string;

  constructor(id: number, text: string) {
    this.id = id;
    this.text = text;
  }
}

export default defineComponent({
  name: 'TodoView',
  props: {
    todos: {
      type: [TodoType],
      required: true,
    },
  },
});
</script>
