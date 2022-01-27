<template>
    <footer>
        <div class="ft-top">
            <ul>
                <li>
                    <img src="@/assets/buy-comics-digital-comics.png" alt="digital comics">
                    digital comics
                </li>

                <li>
                    <img src="@/assets/buy-comics-merchandise.png" alt="merchandise">
                    dc merchandise
                </li>

                <li>
                    <img src="@/assets/buy-comics-subscriptions.png" alt="subscription">
                    subscription
                </li>

                <li>
                    <img src="@/assets/buy-comics-shop-locator.png" alt="shop-locator">
                    comic shop locator
                </li>

                <li>
                    <img src="@/assets/buy-dc-power-visa.svg" alt="dc power visa">
                    dc power visa
                </li>
            </ul>
        </div>
        <div class="ft-center"></div>
        <div class="ft-bottom"></div>

    </footer>
</template>

<script>
export default {
   name: 'FooterDc'
}
</script>

<style lang="scss" scoped>
    @import '@/style/variables.scss';

    .ft-top {
        height: 150px;
        background-color: $blue-dc;
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding: 0 30px;

        ul {
            display: flex;
            
            li {
                display: flex;
                align-items: center;
                text-transform: uppercase;
                margin-right: 35px;
                color: #fff;
            }
        
            li > img {
                width: 45px;
                height: 60px;
                margin-right: 10px ;
            }
        }
    }



</style>