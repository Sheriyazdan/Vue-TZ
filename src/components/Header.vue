
<script>
import dropdown from 'vue-dropdowns';

export default {
    data() {
        return {
            arrayOfObjects: [],
            object: {
                name: 'RU',
            }
        }
    },

    components: {
        'dropdown': dropdown,
    },

    methods: {
        methodToRunOnSelect(payload) {
            this.object = payload;
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="header-logo">
                <img src="icons/logo.svg" alt="">
            </div>
            <div class="header-items">
                <div class="header-links">
                    <div class="header-links__item">Tourism</div>
                    <div class="header-links__item">Invest</div>
                    <div class="header-links__item">Convention bureau</div>
                </div>
                <div class="header-networks">
                    <div class="instagram-logo">
                        <a href="#"> <svg width="21" height="21" viewBox="0 0 21 21" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M10.4999 0.083252C13.3301 0.083252 13.6833 0.0936686 14.7937 0.145752C15.903 0.197835 16.6583 0.371794 17.3228 0.630127C18.0103 0.89471 18.5895 1.25304 19.1687 1.83117C19.6984 2.35189 20.1082 2.98178 20.3697 3.677C20.627 4.34054 20.802 5.09679 20.8541 6.20617C20.903 7.31659 20.9166 7.66971 20.9166 10.4999C20.9166 13.3301 20.9062 13.6833 20.8541 14.7937C20.802 15.903 20.627 16.6583 20.3697 17.3228C20.109 18.0184 19.699 18.6485 19.1687 19.1687C18.6478 19.6982 18.018 20.108 17.3228 20.3697C16.6593 20.627 15.903 20.802 14.7937 20.8541C13.6833 20.903 13.3301 20.9166 10.4999 20.9166C7.66971 20.9166 7.31659 20.9062 6.20617 20.8541C5.09679 20.802 4.34159 20.627 3.677 20.3697C2.98151 20.1087 2.35151 19.6988 1.83117 19.1687C1.30138 18.648 0.891514 18.0181 0.630127 17.3228C0.371794 16.6593 0.197835 15.903 0.145752 14.7937C0.0967936 13.6833 0.083252 13.3301 0.083252 10.4999C0.083252 7.66971 0.0936686 7.31659 0.145752 6.20617C0.197835 5.09575 0.371794 4.34159 0.630127 3.677C0.89079 2.98136 1.30076 2.35129 1.83117 1.83117C2.35166 1.3012 2.98162 0.891303 3.677 0.630127C4.34159 0.371794 5.09575 0.197835 6.20617 0.145752C7.31659 0.0967936 7.66971 0.083252 10.4999 0.083252ZM10.4999 5.29159C9.11858 5.29159 7.79382 5.84032 6.81707 6.81707C5.84032 7.79382 5.29159 9.11858 5.29159 10.4999C5.29159 11.8813 5.84032 13.206 6.81707 14.1828C7.79382 15.1595 9.11858 15.7083 10.4999 15.7083C11.8813 15.7083 13.206 15.1595 14.1828 14.1828C15.1595 13.206 15.7083 11.8813 15.7083 10.4999C15.7083 9.11858 15.1595 7.79382 14.1828 6.81707C13.206 5.84032 11.8813 5.29159 10.4999 5.29159ZM17.2708 5.03117C17.2708 4.68583 17.1336 4.35464 16.8894 4.11046C16.6452 3.86627 16.314 3.72909 15.9687 3.72909C15.6233 3.72909 15.2921 3.86627 15.048 4.11046C14.8038 4.35464 14.6666 4.68583 14.6666 5.03117C14.6666 5.3765 14.8038 5.70769 15.048 5.95188C15.2921 6.19607 15.6233 6.33325 15.9687 6.33325C16.314 6.33325 16.6452 6.19607 16.8894 5.95188C17.1336 5.70769 17.2708 5.3765 17.2708 5.03117ZM10.4999 7.37492C11.3287 7.37492 12.1236 7.70416 12.7096 8.29021C13.2957 8.87626 13.6249 9.67112 13.6249 10.4999C13.6249 11.3287 13.2957 12.1236 12.7096 12.7096C12.1236 13.2957 11.3287 13.6249 10.4999 13.6249C9.67112 13.6249 8.87626 13.2957 8.29021 12.7096C7.70416 12.1236 7.37492 11.3287 7.37492 10.4999C7.37492 9.67112 7.70416 8.87626 8.29021 8.29021C8.87626 7.70416 9.67112 7.37492 10.4999 7.37492Z"
                                    fill="white" />
                            </svg>
                        </a>
                    </div>
                    <div class="youtube-logo">
                        <a href="#"> <svg width="25" height="19" viewBox="0 0 25 19" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="M24.836 4.26514C24.836 2.06787 23.2198 0.300293 21.2227 0.300293C18.5176 0.173828 15.7588 0.125 12.9395 0.125H12.0606C9.2481 0.125 6.48443 0.173828 3.77935 0.300781C1.78716 0.300781 0.170951 2.07812 0.170951 4.27539C0.0488809 6.01318 -0.0028769 7.75146 5.27871e-05 9.48974C-0.00483003 11.228 0.0505085 12.9679 0.166068 14.7095C0.166068 16.9067 1.78228 18.689 3.77447 18.689C6.61626 18.8208 9.5313 18.8794 12.4952 18.8745C15.4639 18.8843 18.3708 18.8224 21.2159 18.689C23.2129 18.689 24.8292 16.9067 24.8292 14.7095C24.9463 12.9663 25.0001 11.228 24.9952 9.48486C25.0062 7.74658 24.9532 6.00667 24.836 4.26514ZM10.1075 14.2798V4.68506L17.1876 9.47998L10.1075 14.2798Z"
                                    fill="white" />
                            </svg>
                        </a>
                    </div>
                    <div class="facebook-logo">
                        <a href="#"> <svg width="21" height="21" viewBox="0 0 21 21" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd"
                                    d="M4.24992 0.083252C1.94873 0.083252 0.083252 1.94873 0.083252 4.24992V16.7499C0.083252 19.0511 1.94873 20.9166 4.24992 20.9166H9.83225V12.8462H7.37492V9.68872H9.8269V7.37152C9.8269 4.67647 11.3247 3.20842 13.5062 3.20842C14.2417 3.20526 14.9769 3.24698 15.7083 3.33338V6.14846H14.2051C13.0188 6.14846 12.7886 6.77229 12.7886 7.68343V9.69462H15.6235L15.2566 12.8521H12.7886V20.9166H16.7499C19.0511 20.9166 20.9166 19.0511 20.9166 16.7499V4.24992C20.9166 1.94873 19.0511 0.083252 16.7499 0.083252H4.24992Z"
                                    fill="white" />
                            </svg>
                        </a>
                    </div>
                </div>
                <div class="header-search">
                    <img src="icons/search.svg" alt="">
                </div>
                <div class="burger-menu">
                    <div class="burger-menu__item"></div>
                    <div class="burger-menu__item"></div>
                    <div class="burger-menu__item"></div>
                </div>
                <dropdown class="my-dropdown-toggle" :options="arrayOfObjects" :selected="object"
                    v-on:updateOption="methodToRunOnSelect" :placeholder="'Select an Item'"
                    :closeOnOutsideClick="boolean">
                </dropdown>
                <div class="header-card">
                    <div class="shopping-card">
                        <img src="icons/shopping-card.svg" alt="">
                    </div>
                    <div class="header-card__item">
                        <div class="card_title">КОРЗИНА</div>
                        <div class="card_price">0 ТГ.</div>
                    </div>
                </div>
            </div>

        </div>
    </header>
</template>



<style scoped lang="scss">
header {
    background: rgba(1, 24, 50, 0.3);
    backdrop-filter: blur(15px);
    height: 75px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 99;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 1320px;
        width: 100%;
        margin: 0 auto;
        height: 100%;

        @media (max-width:1200px) {
            padding: 0 29px;
        }
    }

    .header-links {
        display: flex;
        gap: 60px;

        @media (max-width:1200px) {
            display: none;
        }

        &__item {
            padding: 6px 16px;
            font-weight: 500;
            font-size: 16px;
            line-height: 20px;
            text-transform: uppercase;
            color: #FFFFFF;
            transition: 0.2s;
            cursor: pointer;
            border-radius: 29px;


            &:hover {
                background: #FFFFFF;
                color: #011832;
            }
        }
    }

    .header-networks {
        display: flex;
        gap: 27px;
        align-items: center;

        @media (max-width:1200px) {
            display: none;
        }

        svg {
            path {
                fill: grey;
                cursor: pointer;
                transition: 0.2s;
            }

            &:hover {
                path {
                    fill: white;
                }
            }
        }
    }

    .header-search {
        width: 25px;
        height: 25px;

        img {
            cursor: pointer;
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }

    .burger-menu {
        display: flex;
        flex-direction: column;
        align-items: flex-end;
        gap: 6.25px;
        cursor: pointer;

        &__item {
            background-color: #fff;
            height: 2px;
            width: 16px;

            &:nth-child(1) {
                width: 10px;
            }

            &:nth-child(3) {
                width: 6px;
            }
        }
    }

    .my-dropdown-toggle {
        .li {
            color: #fff !important;
        }
    }

    .header-card {
        display: flex;
        align-items: center;
        gap: 10px;

        @media (max-width:1200px) {
            display: none;
        }

        .shopping-card {
            width: 30px;
            height: 30px;

            img {
                width: 100%;
                height: 100%;
                object-fit: contain;
            }
        }

        &__item {
            .card_title {
                font-weight: 500;
                font-size: 16px;
                line-height: 20px;
                color: #FFFFFF;
            }

            .card_price {
                font-weight: 500;
                font-size: 9px;
                line-height: 11px;
                text-transform: uppercase;
                color: #FFFFFF;
            }
        }

    }

    .header-items {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 80%;

        @media (max-width:1200px) {
            justify-content: flex-end;
            gap: 10px;
        }
    }

    .header-logo {
        width: 144px;
        height: 41.71px;

        img {
            width: 100%;
            height: 100%;
            object-fit: contain;
        }
    }
}
</style>