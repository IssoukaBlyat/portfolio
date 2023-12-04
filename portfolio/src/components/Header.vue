<script setup>
</script>

<template>
    <header>
        <section>
            <a href="#provisoire">
                <img id="provisoire" src="@/assets/images/limule.png" alt="Photo de profil">
            </a>
        </section>
        <nav>
            <a href="#presentation">Présentation</a>
            <a href="#creations">Mes créations</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
</template>

<style scoped>
    header {
        background-color: #782221;
        color: white;
    }

    section {
        text-align: center;
    }

    img {
        margin-bottom: 10px;
        margin-top: 10px;
        border-radius: 50%;
        box-shadow: 0 0 10px black;
    }

    nav {
        background-color: #2c1d27;
        justify-content: space-around;
        padding: 20px;
        display: flex;
        flex-direction: row;
    }

    a {
        color: white;
        text-decoration: none;
    }

    nav a:hover {
        text-decoration: underline;
    }
</style>