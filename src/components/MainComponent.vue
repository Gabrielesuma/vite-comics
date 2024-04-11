<template>
    <main>
        <div class="container">
            <div class="current">
                CURRENT SERIES
            </div>
            <div class="row">
                <div class="col-12 col-md-6 col-lg-2 mb-4" v-for="(item, index) in comics" :key="index">
                    <CardComponent :image="item.thumb" :title="item.series"/>
                </div>
            </div>
        </div>
        <div class="text-center">
            <button>LOAD MORE</button>
        </div>
        
    </main>
</template>

<script>
    import {comics} from '../data/store.js';
    import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data(){
            return {
                comics: comics
            }
        },
        mounted(){
            console.log(this.comics);
        }
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    main{
        background-color: $link;
        div.row{
            color: white;
            padding: 30px 0;
            font-size: 20px;
        }
        button{
            color: white;
            background-color: $firstfooter;
            padding: 10px;
            border: 2px solid $firstfooter;
            margin-bottom: 30px;
        }
    }
    div.current{
        color: white;
        background-color: $firstfooter;
        margin: 0;
        padding: 10px;
        transform: translateY(-50%);
        width: 150px;
        text-align: center;
    }
</style>