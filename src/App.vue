<template>
  <div id="app">
    <Header />
    <br>
    <ExamDescription />
    <br>
    <StudentInformation />
    <br>
    <MCQQuestions />
    <br>
    <TrueOrFalseQuestions />
    <br>
    <NumericalQuestions />
    <br>
    <DescriptiveQuestions />
    <br>
    <SubmitExam />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import ExamDescription from './components/ExamDescription.vue';
import StudentInformation from './components/StudentInformation.vue';
import MCQQuestions from './components/MCQQuestions.vue';
import DescriptiveQuestions from './components/DescriptiveQuestions.vue';
import TrueOrFalseQuestions from './components/TrueOrFalseQuestions.vue';
import NumericalQuestions from './components/NumericalQuestions.vue';
import SubmitExam from './components/SubmitExam.vue';

export default {
  components: {
    Header,
    ExamDescription,
    StudentInformation,
    MCQQuestions,
    DescriptiveQuestions,
    TrueOrFalseQuestions,
    NumericalQuestions,
    SubmitExam
  }
};
</script>

<style>
#app {
  /* font-family: Arial, sans-serif; */
  margin: 10px;
}
</style>
