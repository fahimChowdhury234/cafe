<!-- Home.vue -->
<template>
    <div class="home">
        <h1>Welcome to Our Cafe!</h1>
        <p>Enjoy our delicious coffee and pastries.</p>
        <router-link to="/menu">
            <button class="btn">View Menu</button>
        </router-link>
    </div>
</template>

<script setup>

</script>

<style scoped>
.home {
    text-align: center;
    margin-top: 50px;
}

.btn {
    padding: 10px 20px;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
}

.btn:hover {
    background-color: #45a049;
}
</style>