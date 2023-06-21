<template>
    <section class="container">
        <div class="home">
            <h1 class="home_title"> Numērisk by Isoskēle,<br>la plateforme qui lutte <br> pour la sécurité <br> numérique des jeunes </h1>
        </div>
        <div class="image_container">
            <img src="../assets/flower.svg" alt="petite image de fleur" class="home_flower">
            <img src="../assets/homeImg.png" alt="picture little chdldrien crying under the bed" class="home_img">
        </div>
    </section>
    <imageCard />
</template>

<script setup>
import imageCard from '../components/imageCard.vue';

</script>

<style lang="scss" scoped>
.container {
    position: relative;
    display: flex;
    justify-content: space-between;
    margin-top: 6%;

    .home {
        padding-left: 5vw;
        z-index: 10;

        &_title {
            font-family: "Unbounded";
            font-size: 70px;
            font-weight: bold;
            color: #ffff;
            text-decoration: none;
        }

        &_flower {
            position: absolute;
            z-index: 99;
            right: 5vw;
            top: -5vh;
        }

        &_flower:hover {
            transform: rotate(180deg);
            transition-delay: 0;
            transition: all 1s;
        }

    }

    .home_img {
        position: absolute;
        right: 0px;
        width: 45vw;
        height: 50vh;
        border-top-left-radius: 10%;
        border-bottom-left-radius: 10%;
        border: 2px solid #ffff;

    }

}
</style>