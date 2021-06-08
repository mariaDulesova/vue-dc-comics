<template>
    <div class="wrap">
        <div>
            <img src="../assets/images/buy-comics-digital-comics.png" alt="Digital Comics">
            <p>Digital Comics</p>
        </div>
        <div>
            <img src="../assets/images/buy-comics-merchandise.png" alt="Merchandise">
            <p>DC Merchandise</p>
        </div>
        <div>
            <img src="../assets/images/buy-comics-subscriptions.png" alt="Subscriptions">
            <p>Subscription</p>
        </div>
        <div>
            <img src="../assets/images/buy-comics-shop-locator.png" alt="Shop Locator">
            <p>Comic Shop Locator</p>
        </div>
        <div>
            <img src="../assets/images/buy-dc-power-visa.svg" alt="Visa">
            <p>DC Power Visa</p>
        </div>
    </div>
    
</template>

<script>
export default {
    name: "Bonus"

}
</script>

<style scoped lang="scss">
    @import "../style/variables.scss";
    @import "../style/mixins.scss";

    .wrap {
        @include wrap;
        @include flex-align-center;
        justify-content: space-between;
        padding: 20px 0;

        div {
            @include flex-align-center;

            img{
            height: 30px;
            }

            p {
                padding-left: 10px;
                text-transform: uppercase;
                font-size: 0.8rem;
                font-weight: 300;
                color: $primary-white

            }

        }

        
    }

</style>