<template>
    <div>
        <img :src="film.thumb" :alt="film.series">  
        <p> {{ film.series }}</p>
    </div>
       
</template>

<script>
    export default {
        name: 'Series',
        props: ['film']

    }
</script>

<style lang='scss' scoped>
    @import "../style/variables.scss";


    div {
        width: calc(100% / 6);
        padding: 0 10px;

        img {
            width:100%;
            height:130px;
            object-fit: cover;
            object-position: 0 0;
            margin-top: 20px;
            text-align: center;   
        }

        p {
            text-align: center;
            color: white;
            font-weight: 300;
        }
    }

</style>