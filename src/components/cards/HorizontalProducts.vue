<template>
   <v-card 
        class="mt-3 pa-4" 
        outlined
        min-width="100%"
        
        >
       <div class="d-flex">
           <div>
               <v-img
                :src="product.image"
                width="120px"
                height="120px"
               />
           </div>
           <div class="d-flex flex-column ">
                <v-card-title class="pb-2">{{product.name}}</v-card-title>
                <v-card-subtitle class="pb-2">{{product.price}}</v-card-subtitle>
                <v-btn 
                    color="error"
                    class="ml-4"
                    outlined
                >
                    <v-icon small left>fa-minus</v-icon>
                    Remove product
                </v-btn>
           </div>
       </div>
   </v-card>
</template>

<script>
export default {
     props: {
        product: Object,
        updateCart: Function,
        btnAction: String,
        i: Number
    }
}
</script>