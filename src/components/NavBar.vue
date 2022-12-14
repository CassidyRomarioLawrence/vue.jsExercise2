<template>
    <nav>
        <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/about">About</router-link></li>
            <li><router-link to="/products">Products</router-link></li>
            <li><router-link to="/admin">Admin</router-link></li>
            <li><router-link to="/contact">Contact</router-link></li>
        </ul>
    </nav>
</template>

<script>
    export default {
        name:'NavBar'
    }
</script>

<style scoped>


ul{
    display: flex;
    list-style: none;
}

ul li{
    margin: 0 8px;
    font-size: 20px;
}
</style>