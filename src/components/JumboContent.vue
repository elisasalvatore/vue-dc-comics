<template>
    <div class="jumbo">
         CONTENT GOES HERE
    </div>
</template>

<script>
export default {
   name: 'JumboContent'
}
</script>

<style lang="scss" scoped>
    @import '@/style/variables.scss';

    .jumbo{
        width: 100vw;
        height: 80vh;
        background: url('../assets/jumbotron.jpg') no-repeat;
        background-size: cover;
        font-size: 40px;
        color:#fff;
        text-align: center;
        line-height: 80vh;
    }
</style>