<template>
    <div class="card">
        <a href="#">
            <div class="picture">
                <img :src="details.thumb" alt="">
            </div>
            <p>{{details.series}}</p>      
        </a> 
    </div>
</template>
<script>
export default {
    name:'singleProduct',
    props:{
        details:Object
    }
}
</script>

<style scoped lang="scss">
@import '../styles/vars.scss';
.card{
width: calc(100% / 6);
height: 250px;
    &:hover p{
    color: $secondary_text_color;
    }
    .picture{
    overflow: hidden;
    height: 185px;
    }
    p{
    text-transform: uppercase;
    font-size: 14px;
    color: $primary_text_color;
    display: inline-block ;
    width: 192px;
    padding-top: 15px;
    }
}
</style>