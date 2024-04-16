<template>
    <div class="card">
        <div class="card-header">
            <b>Multiple Choice Questions</b>
        </div>
        <div class="card-body">
            <div v-for="(question, index) in questions" :key="index">
                <p>{{ index + 1 }}. {{ question.text }}</p>
                <label v-for="(option, optionIndex) in question.options" :key="optionIndex">
                    <input type="radio" :name="'question' + index" :value="option">
                    {{ option }}
                </label>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            questions: [{
                text: 'A student wants to extract energy from fossil fuels. Which process would help him to extract the energy from fossil fuel?',
                options: ['burning', 'crystallisation', 'condensation', 'distillation'],
            },
            {
                text: 'When a plane mirror is rotated through a certain angle, the reflected ray turns through twice as much and the size of the image:',
                options: ['is doubled', 'is halved', 'becomes infinite', 'remains the same'],
            },
            {
                text: 'The electronic configuration of an element is found to be 2, 4. How many bonds can one carbon atom form in a compound?',
                options: ['1', '2', '4', '6'],
            },
            {
                text: 'Which of the following forms the basis of the modern periodic table?',
                options: ['Atomic mass', 'Atomic number', 'Number of nucleons', 'All of the above'],
            },
            {
                text: 'Which of the following oxides of iron would be obtained on the prolonged reaction of iron with steam?',
                options: ['FeO', 'Fe2O3', 'Fe3O4', 'Fe2O3 and Fe3O4'],
            }],
            answers: []
        };
    }
};
</script>