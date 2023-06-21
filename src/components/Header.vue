<template>
    <header class="header">
        <div class="container">
            <img src="../assets/Logo_numerisk.svg" class="container_img" />
            <div class="container_menu">
                <a href="" class="container_menu_title">
                    <span>Ressources</span>
                </a>
                <a href="" class="container_menu_title">
                    <span>Quiz</span>
                </a>
                <a href="" class="container_menu_title">
                    <span>Aide</span>
                </a>
                <div class="contact">
                    <a href="" class="container_menu_title">
                        <span>Contact</span>
                    </a>
                </div>
            </div>
        </div>
    </header>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.header {
    width: 100%;
    border-bottom: 2px solid #ffff;

    .container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 90%;
        margin: 0.5vh auto;

        &_img {
            width: 10vw;
            height: 10vw;
        }

        &_menu {
            align-self: center;
            display: flex;
            flex-direction: row;
            gap: 2VW;

            &_title {
                font-family: "Unbounded";
                font-size: 32px;
                color: #ffff;
                text-decoration: none;
            }

            &_title:hover:not(:last-child) {
                span {
                    border-bottom: 4px solid #B8E4BC;
                    rotate: 90deg;
                }
            }
        }
    }


}

.contact {
    background-color: #CEBDEC;
    rotate: -6deg;
    padding: 1%;

    span {
        color: rgb(0 0 0);
    }
}

.contact:hover {
    background-color: #F5F2A9;
    transform: rotate(10deg);
    transition-delay: 0;
    transition: all 0.6s;

}
</style>