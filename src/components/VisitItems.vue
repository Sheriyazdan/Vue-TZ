<script>
export default {
    props: {
        title: String,
        text: String,
        image: String
    }
}
</script>

<template>
    <div class="visit-city__item">
        <div class="city__img">
            <img :src="image" alt="">
        </div>
        <div class="city__title">{{title}}</div>
        <div class="city__text">{{text}} </div>
    </div>
</template>


<style scoped lang="scss">
.visit-city__item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.city__img {
    position: relative;
    z-index: 3;
    cursor: pointer;

    img {
        width: 130px;
        height: 130px;
        object-fit: cover;
        border-radius: 50%;
        filter: drop-shadow(0px 26px 20px rgba(1, 24, 50, 0.65));
    }

    &:hover {
        &::after {
            transition: 0.2s;
            content: '';
            position: absolute;
            background-image: url(images/item-bue-shadow.png);
            width: 150px;
            height: 150px;
            left: -10px;
            top: -10px;
            z-index: -1;
            background-size: initial;
            background-position: center;
        }
    }
}

.city__title {
    font-weight: 700;
    font-size: 17px;
    line-height: 21px;
    text-transform: uppercase;
    color: #FFFFFF;
    margin-top: 26px;
    white-space: nowrap;
}

.city__text {
    font-weight: 400;
    font-size: 14px;
    line-height: 17px;
    color: #FFFFFF;
}
</style>