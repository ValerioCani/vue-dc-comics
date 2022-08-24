<template>
    <div>
        <img src="@/assets/img/dc-logo.png" alt="">
        <ul>
            <li v-for="(link, index) in navbarLinks" :key="index">
                <a :href="link.url">{{link.text}}</a>
            </li>
        </ul>
    </div>
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

<style>

</style>