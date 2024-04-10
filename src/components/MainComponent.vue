<template>
    <main>
        <div class="container">
        -->>Content goes here<<--
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MainComponent'
    }
</script>

<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    main{
        background-color: $link;
        div{
            color: white;
            padding: 30px 0;
            font-size: 20px;
        }
    }
</style>