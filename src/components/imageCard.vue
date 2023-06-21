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
        <div class="imageCard">
            <div class="imageCard_titleContainer2">
                <h3>J’accède aux ressources</h3>
            </div>
            <img src="../assets/cardImage2.png" alt="help me" class="image">
        </div>
        <div class="imageCard">
            <div class="imageCard_titleContainer3">
                <h3>Je suis intervenant.e</h3>
            </div>
            <img src="../assets/cardImage3.png" alt="help me" class="image">
        </div>
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
    margin-top: 30vh;
    display: flex;
    flex-direction: row;
    justify-content: space-around;


    .imageCard {
        position: relative;
        background-color: white;
        display: flex;
        flex-direction: column;
        width: 21vw;
        height: 40vh;
        border-top-left-radius: 2vw;
        border-top-right-radius: 2vw;
        border-bottom-left-radius: 2vw;
        border-bottom-right-radius: 2vw;


        &_titleContainer1 {
            text-align: center;
            padding: 2% 3%;
            background-color: #F5F2A9;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        &_titleContainer2 {
            text-align: center;
            padding: 2% 3%;
            background-color: #CEBDEC;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        &_titleContainer3 {
            text-align: center;
            padding: 2% 3%;
            background-color: #B8E4BC;
            border-top-left-radius: 2vw;
            border-top-right-radius: 2vw;
        }

        h3 {
            font-family: "Unbounded";
            color: black;
            font-size: 30px;
            font-weight: 300;
        }
    }

    .image {
        padding: 2%;
        max-width: 15vw;
        max-height: 25vh;
        align-self: center;
    }
}
</style>