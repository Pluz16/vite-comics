<template>
    <main>
    <section class="content">
    <h3 class="container">-- Content goes her --</h3>
    </section>

    <section class="merch">
        <div class="flex container">
        <ul class="flex">
        <li>
        <div class="flex">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <h4>Digital Comics</h4>
        </div>
        </li>

        <li>
        <div class="flex">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <h4>Dc Merchandise</h4>
        </div>
        </li>

        <li>
        <div class="flex">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <h4>Subscription</h4>
        </div>
        </li>

        <li>
        <div class="flex">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <h4>Comic Shop Locator</h4>
        </div>
        </li>

        <li>
        <div class="flex">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <h4>Dc Power Visa</h4>
        </div>
        </li>

        </ul>
        </div>
    </section>

    </main>
</template>

<script>
    export default {
        name: 'MainComponent',
    }
</script>

<style lang="scss" scoped>
 @use '../assets/styles/partials/variables' as *;
    @use '../assets/styles/partials/mixins' as *;
    @use '../assets/styles/generals.scss' as *;
    .content{
        background-color: $greydark;
        color: $white;
    }
    .merch{
        background-color: $blue;
        color: $white;
    }
    img{
        max-width: 30px;
    }
    section{
        padding: 20px;
    }
    .flex {
        display: flex;  
        justify-content: space-between;
        vertical-align: middle;
    }
    ul{
        li{
            list-style: none;
        }
        h4{
            text-transform: uppercase;
        }
    }
</style>
