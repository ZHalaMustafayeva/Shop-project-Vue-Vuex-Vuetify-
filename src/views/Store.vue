<template>
    <v-container>
        <v-row>
            <v-col md="3" >
                <Sidebar/>
            </v-col>
            <v-col md="9">
                <Product/>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
import Sidebar from '../components/store/Sidebar.vue'
import Product from '../components/store/Product.vue'
export default {
    components:{
        Sidebar,
        Product
    }
}
</script>