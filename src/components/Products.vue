<template>
    <div class="container my-cards">
    <div v-for="item in sneakers" :key="item" class="card">
        <img :src="item.image" style="height: 300px;" alt="Product Image">
        <div class="container">
            <h4 class="Title"></h4>
            <p>Color: {{item.color}}</p>
            <p>Price: R{{item.price}}</p>
            <button type="submit">Purchase</button>
        </div>
    </div>
    </div>
</template>

<script>
    export default {
    name: 'Products',
    data() {
        return {
            sneakers: [
                {
                    id: 1,
                    name: "NIKE AIR FORCE 1 LOW 07",
                    image: "https://i.postimg.cc/3Rf5GGLm/Sneaker1.png",
                    color: "WHITE",
                    price: 2899,
                },
                {
                    id: 2,
                    name: "JORDAN 4 RETRO UNIVERSITY BLUE",
                    image: "https://i.postimg.cc/LX1wJW1K/Sneaker2.png",
                    color: "UNIVERSITY BLUE",
                    price: 10999,
                },
                {
                    id: 3,
                    name: "ADIDAS NITEBALL",
                    image: "https://i.postimg.cc/7hLP8DRM/Sneaker3.png",
                    color: "WHITE",
                    price: 2099,
                },
                {
                    id: 4,
                    name: "JORDAN 13 RETRO HE GOT GAME",
                    image: "https://i.postimg.cc/rpP20WZW/Sneaker4.png",
                    color: "WHITE/TRUE RED-BLACK",
                    price: 7199,
                },
            ]
        }
        }
    }
</script>

<style scoped>
.my-cards{
    display: flex;
    justify-content: center;
}

img{
    border-radius: 2px;
    width: 100%;
}

.card{
    margin: 30px;
    border-radius: 4px;
    padding: 10px 4px;
    width: 20rem;
    background-color: rgb(220, 214, 214);
}
button{
    padding: 4px;
    background-color: black;
    color: white;
    border-radius: 4px;
    cursor: pointer;
}
</style>