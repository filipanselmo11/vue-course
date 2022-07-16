<script>
import courses from "../courses";
import CourseSummary from "../components/CourseSummary.vue";
export default {
  components: { CourseSummary },
};
</script>

<template>
  <div class="Home Page">
    <header>Site de Curso Online Vue</header>
    <course-summary v-for="course in courses" :key="course.id" :course="course" />
  </div>
</template>
