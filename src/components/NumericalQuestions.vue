<template>
    <div class="card">
        <div class="card-header">
            <b>Numerical Questions</b>
        </div>
        <div class="card-body">
            <div v-for="(question, index) in questions" :key="index">
                <p>{{ index + 1 }}. {{ question.text }}</p>
                <input type="number" v-model.number="answers[index]">
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
                    text: 'A torch bulb has a resistance of 1 Ω when cold. It draws a current of 0.2 A from a source of 2 V and glows. Calculate (i) the resistance of the bulb when glowing and (ii) explain the reason for the difference in resistance.'
                },
                {
                    text: 'If 4 x 10 -3 J of work is done in moving a particles carrying a charge of 16 x 10 - 6 C from infinity to point P .What will be the potential at a point?'
                },
                {
                    text: 'Calculate the work done in moving a charge of 5 coulombs from a point at a potential of 210 volts to another point at 240 volts'
                },
                {
                    text: '4.5 cm needle is placed 12 cm away from a convex mirror of focal length 15 cm. Give the location of image and magnification. Describe what happens to the image as the needle is moved farther from the mirror.'
                },
                {
                    text: 'Calculate the potential difference between the two terminals of a battery if 100J of work is required to transfer 20C of charge from one terminal of the battery to the other.'
                }
            ],
            answers: []
        }
    }
}
</script>

<style></style>