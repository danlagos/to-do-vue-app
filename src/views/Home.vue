<template>
  <div class="todo-Card">
    <h1>To Do List - Vue.js</h1>
    <ToDoCard v-for="todo in todos" :key="todo.id" :todo="todo" />
  </div>
</template>

<script>
// @ is an alias to /src
import ToDoCard from "@/components/ToDoCard.vue";

export default {
  name: "Home",
  components: {
    ToDoCard,
  },
  data() {
    return {
      todos: [
        {
          id: 5928101,
          category: "learning",
          title: "Study Vue",
          description: "Start the Real Word View Course",
          location: "San Diego",
          date: "January 28, 2022",
          time: "12:00",
          checked: false,
        },
        {
          id: 4582797,
          category: "training",
          title: "Run 3 miles",
          description: "Run regular route",
          location: "San Diego",
          date: "January 28, 2022",
          time: "12:00",
          checked: true,
        },
        {
          id: 8419988,
          category: "training",
          title: "learn to make curry paste",
          description: "learn to make curry paste",
          location: "San Diego",
          date: "January 28, 2022",
          time: "12:00",
          checked: false,
        },
      ],
    };
  },
};
</script>

<style scoped>
.todo-Card {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
