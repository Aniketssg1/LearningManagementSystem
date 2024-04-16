<template>
    <div class="card">
        <div class="card-header">
            <b>True Or False Questions</b>
        </div>
        <div class="card-body">
            <div v-for="(question, index) in questions" :key="index">
                <p>{{ index + 1 }}.{{ question.text }}</p>
                <label v-for="(option, optionIndex) in question.options" :key="optionIndex">
                    <input type="radio" :name="'question' + index" :value="answers[index]">
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
            questions: [
                {
                    text: 'Water is optically denser than glass.',
                    options: ['True', 'False']
                },
                {
                    text: 'A concave mirror converges the light-rays, but a convex mirror diverges them.',
                    options: ['True', 'False']
                },
                {
                    text: 'Light travels at a lower speed in water than in air.',
                    options: ['True', 'False']
                },
                {
                    text: ' Rays of light incident parallel to the principal axis pass through the focus after re ection from a concave mirror.',
                    options: ['True', 'False']
                },
                {
                    text: ' A virtual image formed by a spherical mirror is always erect and situated behind the mirror.',
                    options: ['True', 'False']
                }
            ],
            answers: []
        }
    }
};
</script>