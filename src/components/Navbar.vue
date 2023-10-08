<template>
    <nav class="navbar">
        <router-link to="/" class="navbar-item">Home</router-link>
        <router-link to="/about" class="navbar-item">About</router-link>
        <router-link to="/portfolio" class="navbar-item">Portfolio</router-link>
        <router-link to="/contact" class="navbar-item">Contact</router-link>
    </nav>
</template>

<style scoped>
.navbar {
    display: flex;
    justify-content: center;
    align-items: center;
}
.navbar-item {
    padding: 10px;
    color: black;
}
.navbar-item:hover {
    background-color: bisque; 
}
</style>