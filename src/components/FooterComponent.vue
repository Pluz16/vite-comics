<template>
    <footer>
    <div class="container">
    <h3>Dc Comics</h3>
    <ul>
    <li>Characters</li>
    <li>Comics</li>
    <li>Movies</li>
    <li>TV</li>
    <li>Games</li>
    <li>News</li>
    </ul>

    <h3>Shop</h3>
    <ul>
    <li>Shop DC</li>
    <li>Shop Dc Collectibles</li>
    </ul>
    </div>
    </footer>
    <div class="subfooter">
    <div class=" container flex">
    <button>Sign-up Now!</button>

    <div>
    <div><h4>Follow us</h4></div>

    </div>

    </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterComponent',
    }
</script>

<style lang="scss" scoped>
 @use '../assets/styles/partials/variables' as *;
    @use '../assets/styles/partials/mixins' as *;
    @use '../assets/styles/generals.scss' as *;
    footer{
        background-image: url(../assets/img/footer-bg.jpg);
        color: white;
        h3{
            text-transform: uppercase;
        }
        li{
            color: grey;
            text-decoration: none;
            list-style: none;
        }
    }
    .subfooter{
        background-color: $greylight;
    }
    
</style>