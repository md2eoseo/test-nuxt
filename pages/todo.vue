<template>
  <v-row>
    <v-col class="text-center">
      <h1>Todo</h1>
      <v-list>
        <v-list-item v-for="(todo, i) in todos" :key="i">
          <div>{{ todo.title }}</div>
          <div>{{ todo.date }}</div>
        </v-list-item>
      </v-list>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "TodoPage",
  data() {
    return {
      todos: [
        { id: 1, title: "Hello", date: "2022-03-25" },
        { id: 2, title: "World", date: "2022-03-25" },
        { id: 3, title: "Nuxt", date: "2022-03-25" },
      ],
    };
  },
};
</script>
