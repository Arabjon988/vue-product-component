<script setup>
import Product from "./Product.vue";

</script>

<template>
    <div class="product_list">
        <div class="container">
            <div class="product_list_main">
                <div class="product_list_info">
                    <h1>Nowadays New Products</h1>
                </div>
                <Product />
            </div>
        </div>
    </div>
</template>

<style scoped>
.product_list{
    width: 100%;
    height: max-content;
    background-color: white;
    height: 380px;
}

.container{
    width: 100%;
    max-width: 1200px;
    margin: auto;
    padding: 0px 10px;
}

.product_list_main{
    width: 100%;
    position: relative;
}

.product_list_info{
    text-align: center;
    margin-top: 20px;
}
</style>