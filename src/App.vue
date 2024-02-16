<template>
  <h1>{{ courseName }}</h1>
  <p>Course by {{ mentor }}</p>

  <button @click="count++">+</button>
    <h3>{{ count }}</h3>
  <button @click="count--">-</button>
</template>

// options API
<!-- <script>
export default{
  data(){
    return {
      courseName: "Vue js 3 masterclass",
      mentor: "Sujon",
      count: 0,
    }
  }
}
</script> -->
// Composition API
<!-- <script>
export default{
  setup() {
    let count = 0;
    const courseName = "Vue 3 Masterclass";
    const mentor = "Sujon";

    return {count, courseName, mentor}
  }
}
</script> -->

<script setup>
import { ref } from 'vue';
    let count = ref(0);
    const courseName = ref("Vue 3 Masterclass");
    const mentor = ref("Sujon");
</script>