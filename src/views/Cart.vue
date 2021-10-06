<template>
    <v-container>
        <v-row>
            <v-col sm="8" md="5" offset-md="2" lg="4" offset-lg="3" class="ma-4">
                <ProductList/>
            </v-col>
            <v-col sm="4" md="3" order="first" order-sm="last">
                <CheckoutBox/>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import CheckoutBox from '../components/card/CheckoutBox.vue'
import ProductList from '../components/card/ProductList.vue'
export default {
    components:{
        CheckoutBox,
        ProductList
    }
}
</script>