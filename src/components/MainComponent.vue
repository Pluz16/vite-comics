<template>
    <main>
    <section class="content">
    <h3 class="container">-- Content goes her --</h3>
    </section>

    <section class="merch">
        <div class="flex container">
        <ul class="flex">
            <li v-for="(data, index) in data" :key="index">
                <div class="flex">
                <img :src="data.url" alt="">
                <h4>{{ data.text }}</h4>
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
        data() {
            return {
                data: [
                {
                    text: "Digital Comics",
                    url: "../assets/img/buy-comics-digital-comics.png",
                },
                {
                    text: "Dc Merchandise",
                    url: "../assets/img/buy-comics-merchandise.png",
                },
                {
                    text: "Scubscription",
                    url: "../assets/img/buy-comics-scubscriptions.png",
                },
                {
                    text: "Comic Shop Locator",
                    url: "../assets/img/buy-comics-shop-locator.png",
                },
                {
                    text: "Dc Power Visa",
                    url: "../assets/img/buy-dc-power-visa.png",
                },
                ]
            }
        },  
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
        justify-content: space-around;
        vertical-align: middle;
    }
    ul{
        vertical-align: middle;
        li{
            list-style: none;
            padding: 10px;
        }
        h4{
            text-transform: uppercase;
            padding: 3px;
            font-size: 15px;
        }
    }
</style>
