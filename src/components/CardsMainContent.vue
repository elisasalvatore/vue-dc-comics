<template>
    <main>
        <div class="container">
            <div v-for="(card, index) in cards" :key="index" class="card">
                <img :src="card.thumb" alt="">
                <div>{{card.series}}</div>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: 'CardsMainCOntent',
    props: {
        cards: Array
    }
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';

main{
    background-color: #333;

    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        margin: 0 auto;
        width: 1200px;

        .card {
            width: 200px;
            margin: 20px 0;
            color: #fff;
            font-size: 13px;
            text-transform: uppercase;

            img {
                width: 200px;
                height: 200px;
                padding: 10px;
            }

            > div {
                padding: 0 10px;
            }
        }
    }
}
</style>