<template>
    <div class="title">
        <h1>{{ pageTitle }}</h1>
    </div>
</template>

<script>

export default {
    name: 'myTitle',

    data(){
        return{
            pageTitle : 'La mia prima app con Vue CLI!',
        }
    }
}
</script>

<style scoped lang="scss">

</style>