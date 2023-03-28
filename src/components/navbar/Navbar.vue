<script setup>

</script>

<template>
    <div class="navbar">
        <div class="container">
            <div class="nav_main">
                <div class="nav_links">
                    <a href="#">Home</a>
                    <a href="#">About</a>
                    <a href="#">Contact</a>
                    <a href="#">Product</a>
                    <a href="#">Services</a>
                    <a href="#">Comments</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

.navbar{
    position: relative;
    width: 100%;
    height: 60px;
    align-items: center;
    background-color: #363636;
}

.nav_main{
    width: 100%;
    position: relative;
}

.nav_links{
    align-items: center;
    display: flex;
    justify-content: space-around;
    padding-top: 7px;
}

.nav_links a{
    text-decoration: none;
    color: white;
    display: inline-block;
    padding: 10px;  
    transition: all ease-in-out 0.5s;
}

.nav_links a:hover{
    background-color: rgb(215, 125, 125);
}

</style>