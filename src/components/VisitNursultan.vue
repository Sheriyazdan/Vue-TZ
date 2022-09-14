<script setup>
import VisitItemsVue from './VisitItems.vue';
</script>

<template>
    <section class="visit-city">
        <div class="visit-city__img">
            <img src="images/visit-nursultan.png" alt="">
        </div>
        <div class="container">
            <div class="visit-city__items">
                <VisitItemsVue title="Где остановиться?" text="отели, хостелы..." image="images/stay.png" />
                <VisitItemsVue title="Где поесть?" text="рестораны, кафе..." image="images/eat.png" />
                <VisitItemsVue title="Куда сходить?" text="Театры, кино..." image="images/go-off.png" />
                <VisitItemsVue title="Что посмотреть?" text="Музеи, байтерек..." image="images/look.png" />
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.visit-city {
    padding: 75px 0 53px 0;
    background-image: url(images/bridge-background.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;

    &__img {
        max-width: 868px;
        width: 100%;
        margin: 0 auto;
        padding-top: 252px;

        img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }

    .container {
        max-width: 1080px;
        margin: 0 auto;

        @media (max-width:991px) {
            max-width: 768px;
        }
        @media (max-width:991px) {
            padding: 0 0 0 30px;
        }
    }

    &__items {
        display: flex;
        justify-content: space-between;
        margin-top: 178px;

        @media (max-width:991px) {
            overflow: scroll;
            gap: 60px;  
            padding: 0 0 20px 0;
        }
    }
}
</style>