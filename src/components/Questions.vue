<template>
  <div>
    <div class="questions" v-for="(question, index) in questions" :key="index">
      <h3>{{ question.person }}</h3>
      <p>{{ question.title }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Questions",
  data: () => ({
    questions: [
      {
        person: "Monique",
        title: "This is a question...",
      },
      {
        person: "Ryan",
        title: "This is another question...",
      },
    ],
  }),
};
</script>

<style scoped>
</style>