<template>
    <div>
        <v-row
            v-for="product in $store.state.products"
            :key="product.name"
        >
            <HorizontalProducts :product="product"/>
        </v-row>
    </div>
</template>

<script>
import HorizontalProducts from '../cards/HorizontalProducts.vue'
export default {
    components:{
        HorizontalProducts
    }
}
</script>