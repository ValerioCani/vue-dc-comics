<template>
    <footer>
        <section id="upper_footer">
            <div>
                <ul v-for="(list, index) in listArray" :key="index">
                    <h3>{{list.title}}</h3>
                    <li v-for="(link, indice) in listArray[index].links" :key="indice">
                        <a href="link.url">{{link.text}}</a>
                    </li>
                </ul>
            </div>
            <div>
                <img src="@/assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section id="lower_footer">
            <button></button>
            <div>
                <p>FOLLOW US</p>
                <div id="social_icons">
                    
                    <ul>
                        <li v-for="(iconLink, index) in iconlist" :key="index">
                            <a href="iconLink.url">{{iconLink.icon}}</a>
                        </li>
                    </ul>
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
            listArray:[
                {
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
                {
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
                {
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
                {
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
                }
            ],

            iconlist:[
                {
                    icon:'<font-awesome-icon icon="fa-brands fa-facebook-f" />',
                    url:'#'
                },
                {
                    icon:'<i class="fa-brands fa-twitter"></i>',
                    url:'#'
                },
                {
                    icon:'<i class="fa-brands fa-youtube"></i>',
                    url:'#'
                },
                {
                    icon:'<i class="fa-brands fa-pinterest-p"></i>',
                    url:'#'
                },
                {
                    icon:'<i class="fas fa-map-marker-alt"></i>',
                    url:'#'
                }
            ]
        }
    }
}
</script>

<style>

</style>