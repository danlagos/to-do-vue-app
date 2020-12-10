<template>
  <div class="div-add-todo">
    <input class="add-todo" type="field" name="field" id="field" />
    <label for="field"></label>
    <input class="btn-add-todo" type="submit" value="add" />
  </div>
</template>

<script></script>

<style scoped>
.div-add-todo {
  display: inline-flex;
}

.btn-add-todo {
  height: 2.25rem;
}

.add-todo {
  /* padding: 20px;*/
  width: 500px;
  margin: 5px;
  height: 1.5rem;
  /* min-width: 500px;
  cursor: pointer;
  border: 1px solid #39495c;
  margin-bottom: 18px; */
}
</style>
