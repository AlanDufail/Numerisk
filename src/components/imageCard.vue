<template>
    <section class="imageCards">
        <a href="">
            <div class="imageCard">
                <div class="imageCard_titleContainer1">
                    <h3>J'ai besoin d'aide</h3>
                </div>
                <img src="../assets/cardImage1.png" alt="help me" class="image">
            </div>
        </a>
        <a href="">
            <div class="imageCard">
                <div class="imageCard_titleContainer2">
                    <h3>Ressources</h3>
                </div>
                <img src="../assets/cardImage2.png" alt="help me" class="image">
            </div>
        </a>
        <a href="">
            <div class="imageCard">
                <div class="imageCard_titleContainer3">
                    <h3>Je suis intervenant.e</h3>
                </div>
                <img src="../assets/cardImage3.png" alt="help me" class="image">
            </div>
        </a>

    </section>
</template>

<script setup>
import { ref, defineProps } from 'vue';




const props = defineProps({
    title: String,
    img: String,
    alt: String
})


</script>

<style lang="scss" scoped>
.imageCards {
    position: relative;
    margin-top: 25vh;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    margin-bottom: 16vh;

    .imageCard {
        position: relative;
        background-color: white;
        display: flex;
        flex-direction: column;
        width: 25vw;
        height: 38vh;
        border-top-left-radius: 2vw;
        border-top-right-radius: 2vw;
        border-bottom-left-radius: 2vw;
        border-bottom-right-radius: 2vw;


        &_titleContainer1 {
            max-height: 10vh;
            text-align: center;
            padding: 2% 3%;
            background-color: #F5F2A9;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        &_titleContainer2 {
            max-height: 10vh;
            text-align: center;
            padding: 2% 3%;
            background-color: #CEBDEC;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        &_titleContainer3 {
            max-height: 10vh;
            text-align: center;
            padding: 2% 1%;
            background-color: #B8E4BC;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        h3 {
            font-family: "Unbounded";
            color: black;
            font-size: 28px;
            font-weight: 300;
        }
    }

    .image {
        padding: 4%;
        max-width: 15vw;
        max-height: 25vh;
        align-self: center;
    }
}
</style>