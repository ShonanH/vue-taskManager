<template>
  <header>
    <h1>{{ title }}</h1>
    <Button
      @bttn-click="$emit('toggle-task-form')"
      :text="closeTaskButton ? 'Close' : 'Add Task'"
      :color="closeTaskButton ? 'red' : 'green'"
    />
  </header>
</template>
<script>
import Button from "./Button.vue";

export default {
  name: "Header",
  props: {
    title: String,
    closeTaskButton: Boolean,
  },
  components: { Button },
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  color: white;
}
</style>
