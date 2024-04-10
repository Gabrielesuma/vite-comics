<template>
    <header class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo">
        <ul>
            <li v-for="(item, index) in menu" :key="index">
                <a :href="item.url">{{ item.name }}</a>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return {
                menu: [
                    {
                        name: 'CHARACTERS',
                        url: '#'
                    },
                    {
                        name: 'COMICS',
                        url: '#'
                    },
                    {
                        name: 'MOVIES',
                        url: '#'
                    },
                    {
                        name: 'TV',
                        url: '#'
                    },
                    {
                        name: 'GAMES',
                        url: '#'
                    },
                    {
                        name: 'COLLECTIBLES',
                        url: '#'
                    },
                    {
                        name: 'VIDEOS',
                        url: '#'
                    },
                    {
                        name: 'FANS',
                        url: '#'
                    },
                    {
                        name: 'NEWS',
                        url: '#'
                    },
                    {
                        name: 'SHOP',
                        url: '#'
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 10px 0;
        img{
            width: 50px;
        }
    }

    ul{
        list-style: none;
        display: flex;

        li{
            padding: 0 10px;

            a{
                color: $link;
                text-decoration: none;
                font-size: 13px;
                &:hover{
                    color: $hoverlink;
                }
            }
        }

    }
</style>