<template>
    <footer>
        <div class="first-footer">
            <div class="container">
                <div>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Logo">
                    <span>DIGITAL COMICS</span>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="Logo">
                    <span>DC MERCHANDISE</span>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="Logo">
                    <span>SUBSCRIPTION</span>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="Logo">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="Logo">
                    <span>DC POWER VISA</span>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'FooterComponent'
    }
</script>


<style lang="scss" scoped>
    @use '../assets/styles/partials/variables' as *;
    div.first-footer{
        padding: 50px 0;
        background-color: $firstfooter;
        font-size: 13px;
        color: white;
        div.container{
            display: flex;
            justify-content: space-around;
            align-items: center;
            img{
                width: 40px;
            }
            span{
                padding-left: 10px;
            }
        }
    }
</style>