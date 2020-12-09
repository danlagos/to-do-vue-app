<template>
  <div class="to-do">
    <input
      type="checkbox"
      name="checkbox"
      id="checkbox"
      :checked="todo.checked"
      @change="$emit('update: todo.checked', $event.target.checked)"
    />
    <label for="checkbox"> {{ todo.title }}: </label>
    <span> {{ todo.description }} </span>
    <!-- Need edit button give it an icon-->
    <input type="button" value="edit" />
    <label for="edit"></label>
    <!-- need delete button give it a trash icon-->
    <input type="button" value="delete" />
    <label for="delete"></label>
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
