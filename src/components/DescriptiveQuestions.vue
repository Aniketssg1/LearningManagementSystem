<template>
    <div class="card">
        <div class="card-header">
            <b>Descriptive Questions</b>
        </div>
        <div class="card-body">
            <div v-for="(question, index) in questions" :key="index">
                <p>{{ index + 1 }}. {{ question.text }}</p>
                <textarea v-model="answers[index]" rows="4" cols="100" class="textArea"></textarea>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            questions: [
                { text: 'Differentiate between biodegradable and non-biodegradable substances with the help of one example each. List two changes in habit that people must adapt to dispose non-biodegradable waste for saving the environment.' },
                { text: 'How does Plasmodium reproduce? Is this method sexual or asexual?' },
                // Add more questions as needed
            ],
            answers: []
        };
    }
};
</script>

<style>
.textArea {
    position: relative;
}
</style>
