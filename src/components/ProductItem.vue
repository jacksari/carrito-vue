<template>
    <b-card :title="product.name" 
            :img-src="product.picture" 
            :img-alt="product.name" 
            img-top 
            style="max-width: 30rem;" 
            class="mb-2">
        <b-button block variant="warning" @click="$emit('addToCard',product)">Añadir al Carrito</b-button>
    </b-card>
</template>

<script>
export default {
    props:{
        product:{
            type: Object,
            require: true
        }
    },
    methods:{

    }
}
</script>