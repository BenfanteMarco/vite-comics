<script>
export default {
    name: 'AppComics',
    data(){
        return{

        }
    },
    props: {
        img: String,
        title: String
    },
    
}
</script>
<template lang="">
        <div class="col-2">
            <div class="thumbnails mt-5">
                <img :src="img" :alt="title" class="img-fluid">
                <p class="text-uppercase">{{title}}</p>
            </div>
        </div>
</template>
<style lang="scss" scoped>
@use '../styles/generals.scss';

.thumbnails {

    img {
        width: 100%;
        height: 300px;
    }

    p {
        color: white;
        font-weight: bold;
        margin-top: 10px;
        text-align: center;
    }
}
    
</style>