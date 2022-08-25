<template>
    <footer>
        <section id="upper_footer">
            <div class="container">

                <div class="columns">
                    <div>
                        <div>
                            <h3>{{comicsLinkList.title}}</h3>
                            <ul>
                                <li v-for="(link, index) in comicsLinkList.links" :key="index">
                                    <a :href="link.url"> {{link.text}}</a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <h3>{{shopLinkList.title}}</h3>
                            <ul>
                                <li v-for="(link, index) in shopLinkList.links" :key="index">
                                    <a :href="link.url"> {{link.text}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div>
                        <h3>{{dcLinkList.title}}</h3>
                        <ul>
                            <li v-for="(link, index) in dcLinkList.links" :key="index">
                                <a :href="link.url"> {{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3>{{sitesLinkList.title}}</h3>
                        <ul>
                            <li v-for="(link, index) in sitesLinkList.links" :key="index">
                                <a :href="link.url"> {{link.text}}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div>
                    <img src="@/assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>
        <section id="lower_footer">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <div>
                    <h3>FOLLOW US</h3>
                    <!-- <a v-for="(social, index) in iconlist" :key="index" href="icon.url">
                        <img :src="'@/assets/img/footer-'+ social.icon +'.png'" alt="">
                    </a> -->
                    <img src="@/assets/img/footer-facebook.png" alt="">
                    <img src="@/assets/img/footer-twitter.png" alt="">
                    <img src="@/assets/img/footer-youtube.png" alt="">
                    <img src="@/assets/img/footer-pinterest.png" alt="">
                    <img src="@/assets/img/footer-periscope.png" alt="">

                </div>
            </div>
        </section>
    </footer>
</template>
    
<script>
export default {
    name: 'FooterSection',
    data(){
        return{
            comicsLinkList:{
                title: 'DC COMICS',
                links:[
                    {
                        text: 'Characters',
                        url: '#'
                    },
                    {
                        text: 'Comics',
                        url: '#'
                    },
                    {
                        text: 'Movies',
                        url: '#'
                    },
                    {
                        text: 'TV',
                        url: '#'
                    },
                    {
                        text: 'Games',
                        url: '#'
                    },
                    {
                        text: 'Videos',
                        url: '#'
                    },
                    {
                        text: 'News',
                        url: '#'
                    },
                ]
            },
            shopLinkList:{
                title: 'SHOP',
                links:[
                    {
                        text: 'Shop DC',
                        url: '#'
                    },
                    {
                        text: 'Shop DC Collectibles',
                        url: '#'
                    }
                ]
            },
            dcLinkList:{
                title: 'DC',
                links:[
                    {
                        text: 'Terms of Use',
                        url: '#'
                    },
                    {
                        text: 'Privacy policy(New)',
                        url: '#'
                    },
                    {
                        text: 'Ad Choices',
                        url: '#'
                    },
                    {
                        text: 'Advertising',
                        url: '#'
                    },
                    {
                        text: 'Jobs',
                        url: '#'
                    },
                    {
                        text: 'Subscriptions',
                        url: '#'
                    },
                    {
                        text: 'Talent Workshops',
                        url: '#'
                    },
                    {
                        text: 'CPSC Certificates',
                        url: '#'
                    },
                    {
                        text: 'Ratings',
                        url: '#'
                    },
                    {
                        text: 'Shop Help',
                        url: '#'
                    },
                    {
                        text: 'Contact Us',
                        url: '#'
                    }
                ]
            },
            sitesLinkList:{
                title: 'SITES',
                links:[
                    {
                        text: 'DC',
                        url: '#'
                    },
                    {
                        text: 'MAD Magazines',
                        url: '#'
                    },
                    {
                        text: 'DC Kids',
                        url: '#'
                    },
                    {
                        text: 'DC Universe',
                        url: '#'
                    },
                    {
                        text: 'DC Power Visa',
                        url: '#'
                    }
                ]
            },

            iconlist:[
                {
                    icon:'facebook',
                    url:'#'
                },
                {
                    icon:'twitter',
                    url:'#'
                },
                {
                    icon:'youtube',
                    url:'#'
                },
                {
                    icon:'pinterest',
                    url:'#'
                },
                {
                    icon:'periscope',
                    url:'#'
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../styles/vars.scss';
    footer{
        #upper_footer{
        background-image: url('../assets/img/footer-bg.jpg');
            .container{
            height: 370px;
            overflow: hidden;
            display: flex;
            justify-content: space-between;
            align-items: center;
                .columns{
                display: flex;
                color: $primary_text_color;
                    div{
                    margin: 0 1rem;
                        li{
                        padding: 3px 0 ;
                            &:hover{
                            color: $secondary_text_color;
                            }

                            a{
                            color:inherit;
                            font-size: 12px;
                            font-weight:100;
                            }
                        }
                    }
                }
            }
            .columns h3{
                padding: 1rem 0 1rem;
            }
        }

        #lower_footer{
        height: 110px;
        background-color: $footer_back_color;
            button{
            background-color: $footer_back_color;
            font-size: 17px;
            font-weight: 900;
            color: $primary_text_color;
            padding: 8px;
            border: solid 2px $brand_primay_color;
            }
            div{
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
                h3{
                    display:inline-block;
                    color: $secondary_text_color;
                    margin: 20px;
                }
                img{
                    margin: 8px;
                }
            }
        }
    }
</style>