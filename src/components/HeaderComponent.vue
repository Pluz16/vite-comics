<template>
    <header>
        <div class="flex container">
        <div><img src="../assets/img/dc-logo.png" alt=""></div>
        <div>
        <ul class="flex">
            <li v-for="(menu, index) in menu" :key="index">
                    <a :href="menu.url" :class="{ 'active': menu.current }">{{ menu.text }}</a>
            </li>
        </ul>
        </div>
</div>
    </header> 
</template>
<script>
    export default {
        name: 'HeaderComponent',
        data() {
            return {
                menu: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
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
    img{
        max-width: 50px;
    }
    .flex {
        display: flex;  
        justify-content: space-between;
    }
    ul{
        list-style: none;
        margin:  1rem 4rem;
            li a{
                display: inline-block;
                padding: 1rem;
                text-decoration: none;
                font-weight: 600;
                color: $greydark;
                text-transform: uppercase;
                &.active,
                &:hover{
                    color: $blue;
                }
            }
    }
</style>

