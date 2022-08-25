<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(tools, index) in navTools" :key="index">
                    <a :href="tools.url">
                        <img :src="tools.img" alt="">
                        <p>{{tools.text}}</p>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'midBand',
    data(){
        return{
            navTools:[
                {
                    img:require('../assets/img/buy-comics-digital-comics.png'),
                    text:'DIGITAL COMICS',
                    url:'#'
                },
                {
                    img:require('../assets/img/buy-comics-merchandise.png'),
                    text:'DC MERCHANDISE',
                    url:'#'
                },
                {
                    img:require('../assets/img/buy-comics-subscriptions.png'),
                    text:'SUBSCRIPTION',
                    url:'#'
                },
                {
                    img:require('../assets/img/buy-comics-shop-locator.png'),
                    text:'COMIC SHOP LOCATOR',
                    url:'#'
                },
                {
                    img:require('../assets/img/buy-dc-power-visa.svg'),
                    text:'DC POWER VISA',
                    url:'#'
                },
            ]
        }
    }
}
</script>

<style scoped  lang="scss">
    @import '../styles/vars.scss';
    section{
    height: 155px;
    background-color: $brand_primay_color;
        div{
        height: 100%;
            ul{
            height: 100%;
            width: 100%;
                li{
                height: 100%;
                width: 20%;
                display: inline-block;
                padding: 20px;

                    a{
                        display: flex;
                        align-items: center;
                        height: 100%;
                            img{
                            height: 55px;
                            margin-right: 20px;
                            }
                            p{
                            font-size: 13px;
                            color: $primary_text_color;
                            }
                    }
                }
            }
        }
    }  
</style>