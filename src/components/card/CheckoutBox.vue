<template>
    <div>
        <v-card>
            <v-card-title> Payment details</v-card-title>
            <v-card-text>
                <v-text-field label="name"/>
                <v-text-field label="email"/>
                <p>Total:999$</p>
                <v-btn
                class="primary"
                :click="goToCheckout"
                >
                Checkout
                </v-btn>
            </v-card-text>
            
        </v-card>
    </div>
</template>
<script>
export default {
    data() {
        return {
            checkoutForm: null,
            nameRules: [],
            name: '',
            emailRules: [],
            email: ''
        }
    },
    methods: {
        goToCheckout() {
        this.$router.push({ name: 'checkout' })
        }
    }
}
</script>