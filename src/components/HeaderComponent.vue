<template>
    <header>
        <div class="flex container">
        <div><img src="../assets/img/dc-logo.png" alt=""></div>
        <div>
        <ul class="flex">
        <li><a href="#">Characters</a></li>
        <li><a href="#">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">Tv</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Collectibles</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">Fans</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Shop</a></li>
        </ul>
        </div>
</div>
    </header> 
</template>
<script>
    export default {
        name: 'HeaderComponent',
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    @use '../assets/styles/partials/mixins' as *;
    @use '../assets/styles/generals.scss' as *;
    img{
        max-width: 50px;
    }
    .flex {
        display: flex;  
        justify-content: space-between;
    }
    ul{
        list-style: none;
        li{
            padding: 3px;
            text-transform: uppercase;
            text-decoration: none;
        }
    }
</style>

