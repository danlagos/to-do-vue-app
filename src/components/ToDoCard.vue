<template>
  <div class="to-do">
    <span
      >{{ todo.title }}: {{ todo.description }}
      <input
        type="checkbox"
        name="checkbox"
        id="checkbox"
        v-model="todo.checked"
      />
      <label for="checkbox"></label>
    </span>
  </div>
</template>

<script>
export default {
  name: "ToDos",
  props: {
    todo: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.to-do {
  padding: 20px;
  width: 500px;
  min-width: 500px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px;
}

.to-do:hover {
  transform: scale(1.01);
  box-shadow: 0 3px 12px 0 rgba(0, 0, 0, 0.2);
}
</style>
