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
        <div class="second-footer">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-md-4">
                        <h5>DC COMICS</h5>
                        <ul>
                            <li v-for="(item, index) in dccomics" :key="index">
                                <a :href="item.url">{{ item.name }}</a>
                            </li>
                        </ul>
                        <h5>SHOP</h5>
                        <ul>
                            <li v-for="(item, index) in shop" :key="index">
                                <a :href="item.url">{{ item.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-12 col-md-4">
                        <h5>DC</h5>
                        <ul>
                            <li v-for="(item, index) in dc" :key="index">
                                <a :href="item.url">{{ item.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-12 col-md-4">
                        <h5>SITES</h5>
                        <ul>
                            <li v-for="(item, index) in sites" :key="index">
                                <a :href="item.url">{{ item.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="third-footer">
            <div class="container d-flex justify-content-between align-items-center">
                <a href="#">SIGN-UP NOW!</a>
                <div class="d-flex align-items-center">
                    <h5>FOLLOW US</h5>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">
                </div>
            </div>
            
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'FooterComponent',
        data(){
            return {
                dccomics: [
                    {
                        name: 'Characters',
                        url: '#'
                    },
                    {
                        name: 'Comics',
                        url: '#'
                    },
                    {
                        name: 'Movies',
                        url: '#'
                    },
                    {
                        name: 'TV',
                        url: '#'
                    },
                    {
                        name: 'Games',
                        url: '#'
                    },
                    {
                        name: 'Videos',
                        url: '#'
                    },
                    {
                        name: 'News',
                        url: '#'
                    }
                ],
                shop: [
                    {
                        name: 'Shop DC',
                        url: '#'
                    },
                    {
                        name: 'Shop DC Collectibles',
                        url: '#'
                    }
                ],
                dc: [
                    {
                        name: 'Terms Of Use',
                        url: '#'
                    },
                    {
                        name: 'Privacy policy(New)',
                        url: '#'
                    },
                    {
                        name: 'Ad Choices',
                        url: '#'
                    },
                    {
                        name: 'Advertising',
                        url: '#'
                    },
                    {
                        name: 'Jobs',
                        url: '#'
                    },
                    {
                        name: 'Sunscriptions',
                        url: '#'
                    },
                    {
                        name: 'Talent Workshops',
                        url: '#'
                    },
                    {
                        name: 'CPSC Certificates',
                        url: '#'
                    },
                    {
                        name: 'Ratings',
                        url: '#'
                    },
                    {
                        name: 'Shop Help',
                        url: '#'
                    },
                    {
                        name: 'Contact Us',
                        url: '#'
                    }
                ],
                sites: [
                    {
                        name: 'DC',
                        url:'#'
                    },
                    {
                        name: 'MAD Magazine',
                        url:'#'
                    },
                    {
                        name: 'DC Kids',
                        url:'#'
                    },
                    {
                        name: 'DC Universe',
                        url:'#'
                    },
                    {
                        name: 'DC Power Visa',
                        url:'#'
                    }
                ]
            }
        }
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
    div.second-footer{
        color: white;
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        h5{
            padding: 10px;
        }
        ul{
            list-style: none;
            padding: 0 10px;
            a{
                text-decoration: none;
                color: white;
                font-size: 14px;
            }
        }
    }
    div.third-footer{
        background-color: $thirdfooter;
        padding: 40px 0;
        a{
            text-decoration: none;
            color: white;
            border: 2px solid $firstfooter;
            padding: 10px;
        }
        h5{
            color: $firstfooter;
            padding-right: 10px;
        }
        img{
            padding-right: 10px;
        }
    }
</style>