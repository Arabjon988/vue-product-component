<script setup>


</script>


<template>
    <div class="product">
        <div class="product_list" v-for="item in products">
            <div class="product_box" :id="item.id">
                <p class="new_text">New</p>
                <img v-bind:src="item.img" class="product_img" alt="rasm mavjud">
                <p class="product_title"> {{ item.title }} </p>
                <li> price: 
                    <b>{{ item.price }}</b>
                    <del>{{ item.delPrice }}</del>
                </li>
                <div class="buy_item">
                    <button class="buy_btn">Buy</button>
                    <a href="#">Learn more</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

import rasm1 from '../../assets/rasm1.jpg'
import rasm2 from '../../assets/rasm2.jpg'
import rasm3 from '../../assets/rasm3.jpg'
import rasm4 from '../../assets/rasm4.jpg'

export default {
    data: () => ({
        products: [
            {
                "id": 1,
                "title": "apple for everyone, now buy and give me",
                "price": 159000,
                "delPrice": 170000,
                "img": rasm1,
            },
            {
                "id": 2,
                "title": "apple for everyone, now buy and give me",
                "price": 189000,
                "delPrice": 195000,
                "img": rasm2,
            },
            {
                "id": 3,
                "title": "apple for everyone, now buy and give me",
                "price": 119000,
                "delPrice": 120000,
                "img": rasm3,
            },
            {
                "id": 4,
                "title": "apple for everyone, now buy and give me",
                "price": 129000,
                "delPrice": 130000,
                "img": rasm4,
            },
        ]
    }),


}


</script>  

<style scoped>
.product{
    margin-top: 20px;
    display: flex;
    justify-content: space-between;
    width: 100%;
    margin-bottom: 10px;
}

.product_list{
    position: relative;
    width: 220px;
}

.new_text{
    color: white;
    font-weight: bold;
    display: inline-block;
    padding: 12px 4px;
    position: absolute;
    background-color: rgb(205, 155, 155);
    left: 30px;
    top: -2px;
}

.product_box{
    width: 100%;
    border-radius: 10px;
    height: 350px;
    transition: all ease-in-out 0.4s;
    border: 2px solid transparent;
}

.product_box:hover{
    
    border: 2px solid burlywood;
}


li, .product_title{
    margin: 10px 0px;
    margin-left: 20px;
}

.product_title:hover{
    color: yellowgreen;
}


.product_img {
    padding-top: 30px;
    width: 100%;
    padding: 10px;
    height: 200px;
}

li b{
    font-size: 20px;
}

li del{
    margin-left: 10px;
    color: yellowgreen;
}

.buy_item{
    margin-top: ;
    align-items: center;
    position: relative;
    margin: 10px 20px;
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.buy_btn{
    border-radius: 7px;
    padding: 7px 35px;
    border: none;
    background-color: yellowgreen;
}

.buy_btn:hover{
    background-color: rgb(142, 125, 158);
}

.buy_item a{
    font-size: 14px;
    margin-right: 25px;
    text-decoration: none;
}
</style>