<script setup>
</script>

<template>
    <footer>
        <a href="https://www.linkedin.com">
            <img src="@/assets/images/linkedin.png" alt="Logo Linkedin">
        </a>
        <a href="https://twitter.com">
            <img src="@/assets/images/twitter.png" alt="Logo Twitter">
        </a>
        <a href="https://github.com">
            <img src="@/assets/images/github.png" alt="Logo Github">
        </a>
        <br/>
        <br/>
        <small>
            "Dernière nise à jour le "
            <time datetime="2023-12-04">4 décembre 2023</time>
        </small>
    </footer>
</template>

<style scoped>
    footer {
        background-color: #782221;
        color: white;
        text-align: center;
        padding: 25px;
    }

    footer a:hover {
        opacity: 75%;
    }

    footer img {
        width: 5%;
        height: 5%;
    }
</style>