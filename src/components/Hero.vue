<template>
    <div class="jumbo">
        <h2>{{ jumboTitle }}</h2>
        <p>{{ jumboPar }}</p>
    </div>
</template>

<script>

export default {
    name: 'heroJumbo',

    data(){
        return{
            jumboTitle : 'Titolo Jumbo prima app con Vue CLI',
            jumboPar : 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Obcaecati inventore sint officia dolores illum nesciunt dicta quod, molestiae, placeat totam culpa fugit repellendus corrupti consectetur nobis numquam quidem voluptates aliquid.'
        }
    }
}
</script>

<style scoped lang="scss">

    .jumbo{
        width: 100%;
        height: 50vw;
        background-image: url(../assets/IMG_8742.jpg);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        position: relative;
        z-index: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 40px;
        padding: 0 50px;
    }

    .jumbo::after{
        content: '';
        display: block;
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        background-color: rgba(0, 0, 0, 0.6);
        z-index: 1;
    }

    .jumbo h2, .jumbo p{
        color: white;
        z-index: 9999;
    }

    .jumbo h2{
        font-size: 40px;
    }
</style>