<template>
    <v-sheet width="300" class="mx-auto">
        <v-form @submit.prevent>
            <v-text-field v-model="login" :rules="rules" label="First name"></v-text-field>
            <v-text-field v-model="password" :rules="rules" label="First name"></v-text-field>
            <v-btn @click="$router.push('/')" block class="mt-2">Go home</v-btn>
        </v-form>
    </v-sheet>
</template>

<script>
export default {
    data() {
        return {
            login: '',
            password: '',
            rules: [
                value => {
                    if (!value) {
                        return 'You must enter a first name.'
                    }

                    if (value.length < 3) return "min length 3"

                },
            ],
        }
    },
}
</script>