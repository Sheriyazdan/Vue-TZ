<template>
    <section class="reasons-city">
        <div class="container">
            <div class="title_item">
                <div class="reasons-text">
                    <h2>#Nur-Sultan</h2>
                    <span>6 причин посетить город</span>
                </div>
                <div class="more">Подробнее</div>
            </div>

            <div class="reasons-items">
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/baiterek.png" alt="">
                    </div>
                    <div class="reasons-title">Достопримечательности</div>
                    <div class="reasons-desc">Футуристический город посреди степи — левый берег, олицетворяющий
                        техногенное будущее.</div>
                </div>
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/hospitality.png" alt="">
                    </div>
                    <div class="reasons-title">Гостеприимство</div>
                    <div class="reasons-desc">Если вы заблудились, местные никогда не откажут в помощи. Дружелюбие
                        казахов не знает границ.</div>
                </div>
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/khan-shatyr.png" alt="">
                    </div>
                    <div class="reasons-title">Самый большой шатёр в мире</div>
                    <div class="reasons-desc">ТРЦ Хан Шатыр является первым и единственным лайфстайл-центром, который
                        объединяет шопинг и развлечения мирового уровня под одной крышей.</div>
                </div>
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/opera.png" alt="">
                    </div>
                    <div class="reasons-title">Самая большая опера</div>
                    <div class="reasons-desc">Своим величием он поразил немало туристов, а внутри здание украшено еще
                        лучше, чем снаружи.</div>
                </div>
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/architecture.png" alt="">
                    </div>
                    <div class="reasons-title">Уникальная архитектура</div>
                    <div class="reasons-desc">Самая молодая и динамично развивающаяся столица стран СНГ. Возможно,
                        именно поэтому архитектура города столь необычна и поразительна.</div>
                </div>
                <div class="reasons-item">
                    <div class="reason-img">
                        <img src="images/peoples.png" alt="">
                    </div>
                    <div class="reasons-title">Люди</div>
                    <div class="reasons-desc">Несмотря на климат столицы, люди в городе очень добрые и всегда готовы
                        прийти на помощь.</div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.reasons-city {
    padding: 130px 0;
}

.title_item {
    display: flex;
    align-items: center;
    gap: 53px;
    @media (max-width:768px) {
        flex-wrap: wrap;
        gap: 21px;
    }

    .reasons-text {
        display: flex;
        flex-direction: column;

        h2 {
            font-weight: 600;
            font-size: 64px;
            line-height: 78px;
            letter-spacing: -0.03em;
            color: #000000;
        }

        span {
            font-weight: 400;
            font-size: 24px;
            line-height: 29px;
            letter-spacing: -0.03em;

            color: #444444;
        }
    }

    .more {
        cursor: pointer;
        font-weight: 500;
        font-size: 18px;
        line-height: 22px;
        letter-spacing: -0.03em;
        color: #03B0CD;
        display: flex;
        gap: 17px;

        &::after {
            content: url(icons/arrow-right.svg);
        }
    }
}

.container {
    max-width: 1080px;
    margin: 0 auto;

    @media (max-width:991px) {
        max-width: 768px;
    }

    @media (max-width:768px) {
        padding: 0 30px;
    }
}

.reasons-items {
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
    justify-content: space-between;
    max-height: 800px;
    margin-top: 40px;
    row-gap: 35px;
    @media (max-width:768px) {
        max-height: fit-content;
        justify-content: center;
    }
    .reasons-item {
        width: calc(33% - 53px/3);
        display: flex;
        flex-direction: column;
        gap: 15px;

        @media (max-width:768px) {
            width: 100%;
        }

        &:nth-child(3) {
            flex-direction: column-reverse;
            @media (max-width:768px) {
                flex-direction: column;
            }
        }

        .reason-img {
            width: 100%;
            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }
        .reasons-title {
            font-weight: 700;
            font-size: 18px;
            line-height: 22px;
            color: #000000;
        }

        .reasons-desc {
            font-weight: 400;
            font-size: 14px;
            line-height: 23px;
            color: #444444;
        }
    }
}
</style>