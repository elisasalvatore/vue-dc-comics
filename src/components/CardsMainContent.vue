<template>
    <main>
        <div class="container">
            <div class="current-series">
                current series
            </div>

            <div class="cards-box">
                <div v-for="(card, index) in cards" :key="index" class="card">
                    <img :src="card.thumb" alt="">
                    <div>{{card.series}}</div>
                </div>
            </div>

            <button class="load-more">load  more</button>
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

    .current-series {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 220px;
        height: 60px;
        background-color: $blue-dc;
        font-size: 22px;
        font-weight: 700;
        text-transform: uppercase;
        color: #fff;
    }

    .container {
        margin: 0 auto;
        width: 1200px;
        padding-bottom: 20px;
    }

    .cards-box {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;

        .card {
            width: calc(100% / 6);
            margin: 20px 0;
            color: #fff;
            font-size: 13px;
            text-transform: uppercase;

            img {
                width: 200px;
                height: 200px;
                padding: 10px;
                object-position: top;
                object-fit: cover;
            }

            > div {
                padding: 0 10px;
            }
        }
    }

    .load-more {
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        width: 180px;
        height: 35px;
        background-color: $blue-dc;
        font-size: 12px;
        font-weight: 700;
        color: #fff;
        text-transform: uppercase;

        &:hover {
            background-color: #fff;
            color: $blue-dc;
        }
    }
}
</style>