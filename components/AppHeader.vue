<template>
    <header class="header">
        <a class="logo">
            <img src="../assets/logo.svg" alt="Mekel Verellino's Logo">
        </a>
        
        <ul>
            <li>
                <nuxt-link to="/works">WORKS</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/about">ABOUT</nuxt-link>
            </li>
            <li>
                <nuxt-link to="/contact">CONTACT</nuxt-link>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'AppHeader'
}
</script>

<style>
.header{
    position: fixed;
    display: flex;
    width: calc(100vw - 160px);
    margin-top: 40px;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
    mix-blend-mode: difference;
}
.header ul{
    display: flex;
}
.header li{
    display: inline-block;
    padding: 0 1rem;
    font-family: Rakkas;
}
.logo{
    height: 40px;
}
</style>