<template>
    <header>
        <div class="container">
            <a href="#">
                <img src="@/assets/img/dc-logo.png" alt="DC logo">
            </a>
            <ul>
                <li v-for="(link, index) in navbarLinks" :key="index">
                    <a :href="link.url">{{link.text}}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderSection',
    data() {
        return {
            navbarLinks:[
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'TV',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: 'false'
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: 'false'
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '../styles/vars.scss';
    header{
    background-color: $header_back_color;
        div{
        height: 120px;
        display: flex;
        align-items: center;
        justify-content: space-between;

            img{
            height: 80px;
            }

            ul{
            height: 100%;
            display: flex;

                li{
                display: flex;
                align-items: center;
                font-size: 0.8rem;
                font-weight: 900;
                height: 100%;
                border-bottom:solid 5px $header_back_color;

                    &:hover{
                    border-bottom:solid 5px $brand_primay_color;
                    }

                    &:hover>a{
                    color: $brand_primay_color;
                    }

                    a{
                    color: #000;
                    padding: 0.5rem;
                    }
                }
            }
    }
    }
</style>