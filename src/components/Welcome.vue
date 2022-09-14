<template>
    <section class="welcome-city">
        <div class="container">
            <div class="welcome__text">
                <h2 class="title">
                    Добро пожаловать в Нур-Султан
                </h2>
                <div class="desc">
                    <span>Нур-Султан</span> - столица независимого Казахстана. Это молодой, современный, комфортный
                    и динамичный город в котором каждый человек почувствует гостеприимность и радушие столицы.
                </div>
                <div class="welcome__items">
                    <div class="welcome__item">
                        <img src="images/attraction.png" alt="">
                    </div>
                    <div class="welcome__item">
                        <img src="images/food.png" alt="">
                    </div>
                    <div class="welcome__item">
                        <img src="images/event.png" alt="">
                    </div>
                </div>
            </div>
        </div>
        <div class="partner-item">
            <img src="icons/nursultan-icon.png" alt="">
        </div>
    </section>
</template>

<style scoped lang="scss">
.welcome-city {
    padding: 60px 0 121px 0;
    background-image: url(images/welcome-nursultan.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    position: relative;

    @media (max-width:768px) {
        background-position: -400px;
        padding: 0 0 62px 0;
    }
}

.container {
    max-width: 1080px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: flex-end;

    @media (max-width:991px) {
        max-width: 768px;
    }

    @media (max-width:768px) {
        padding: 0 30px;
    }
}

.desc {
    margin-top: 22px;
    max-width: 645px;
    font-weight: 600;
    font-size: 18px;
    line-height: 30px;
    color: #FFFFFF;

    @media (max-width:768px) {
        font-size: 14px;
        line-height: 23px;
    }

}

.welcome__text {
    width: 60%;

    @media (max-width:768px) {
        width: 100%;
    }
}

.title {
    font-weight: 800;
    font-size: 46px;
    line-height: 56px;
    display: flex;
    align-items: center;
    text-transform: uppercase;
    color: #FFFFFF;
    max-width: 578px;

    @media (max-width:768px) {
        font-weight: 800;
        font-size: 25px;
        line-height: 30px;
    }
}

.welcome__items {
    margin-top: 31px;
    display: flex;
    align-items: center;
    justify-content: space-between;


    @media (max-width:991px) {
        flex-direction: column;
        align-items: flex-end;
        gap: 20px;
    }

    .welcome__item {
        max-width: 167px;
        width: 100%;

        img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }
}

.partner-item {
    position: absolute;
    right: 79px;
    bottom: 74px;
    width: 103.36px;
    height: 103.36px;
    @media (max-width:1200px) {
        display: none;
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        border-radius: 50%;
    }

}
</style>