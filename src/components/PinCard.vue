<template>
    <section class="pinCard">
        <div class="pinCard_main">
            <h3>J'ai un code PIN pour le quiz :</h3>
            <p>Vous n’avez pas de code ? Demandez à votre intervenant :) </p>
        </div>
        <div class="pinCard_code">
            <span class="pinCard_input"></span>
            <div class="pinCard_btn">Go</div>
        </div>
    </section>
</template>
<script setup>

</script>
<style lang="scss" scoped>
.pinCard {
    width: 92%;
    background-color: #B8E4BC;
    border-radius: 16px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 6vh;

    &_main {
        font-family: "Unbounded";

        h3 {
            padding-top: 8vh;
            font-weight: 400;
            font-size: 40px;
            text-align: center;
            color: #000;
            margin: 0
        }

        p {
            font-weight: 100;
            color: #000;
            text-align: center;
            margin: 0;
        }
    }

    &_code {
        width: 30vw;
        margin-left: auto;
        margin-right: auto;
        padding-top: 3vh;
        padding-bottom: 10vh;
        display: flex;
        flex-direction: row;
        font-family: "Unbounded";
        cursor: pointer;

        .pinCard_input {
            border-top-left-radius: 8px;
            border-bottom-left-radius: 8px;
            width: 88%;
            background-color: white;
        }

        .pinCard_btn {
            width: 12%;
            text-align: center;
            background-color: #000;
            padding: 2%;
            border-top-right-radius: 8px;
            border-bottom-right-radius: 8px;
        }
    }
}
</style>