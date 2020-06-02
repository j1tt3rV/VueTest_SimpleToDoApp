<template>
  <div>
    <div v-for="todo in todos" v-bind:key="todo.id">
      <TodoItem />
    </div>
  </div>
</template>

<script>
import TodoItem from "@/components/TodoItem";

export default {
  name: "Todos",
  components: {
    TodoItem,
  },
  props: ["todos"],
};
</script>
