<!-- Menu.vue -->
<template>
    <div class="menu">
        <h1>Menu</h1>
        <ul>
            <li v-for="item in menu" :key="item.id" @click="showAlert(item.name)">
                {{ item.name }}

            </li>

        </ul>
        <router-link to="/">
            Back to Home
        </router-link>
    </div>
</template>

<script setup>
import { ref } from 'vue';

const menu = ref([
    { id: 1, name: 'Coffee' },
    { id: 2, name: 'Tea' },
    { id: 3, name: 'Croissant' },
    { id: 4, name: 'Muffin' }
])
const showAlert = ((itemName) => {
    alert(`You selected: ${itemName}`);

})

</script>

<style scoped>
.menu {
    margin-top: 50px;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    cursor: pointer;
    padding: 10px;
    margin: 5px;
    background-color: #f2f2f2;
    border-radius: 4px;
}

li:hover {
    background-color: #ddd;
}
</style>