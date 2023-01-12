<script>
export default {
    data(){
        return{
            imagesBackgroundBlue:[
                {
                    image: 'buy-comics-digital-comics.png',
                    label: 'DIGITAL COMICS'
                },
                {
                    image: 'buy-comics-merchandise.png',
                    label: 'DC MERCHANDISE'
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    label: 'SUBSCRIPTION'
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    label: 'COMIC SHOP LOCATOR'
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    label: 'DC POWER VISA'
                },
            ],

           socialLogo:[
            'facebook',
            'twitter',
            'youtube',
            'pinterest',
            'periscope'
           ]
        }
    }
    
}
</script>

<template lang="">
    <footer>
            <div class="background-blue">
                <div class="container">
                    <div class="cols">
                        <div v-for="(item, index) in imagesBackgroundBlue" :key="index">
                            <img :src="`/image/${item.image}.png`">
                            <span>{{item.label}}</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="background-image">
                <div class="container">
                    <div class="footer-sx">

                    </div>
                    <div class="col">
                        <h4>DC COMICS</h4>
                            <ul>
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>Tv</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                            <h4>SHOP</h4>
                            <ul>
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                    </div>
    
                    <div class="col">
                        <h4>DC</h4>
                            <ul>
                                <li>Terms Of Use</li>
                                <li>Privacy policy(New)</li>
                                <li>Ad Choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscriptions</li>
                                <li>Talent Workshops</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop Help</li>
                                <li>Contact Us</li>
                            </ul>
                    </div>
        
                    <div class="col">
                        <h4>SITES</h4>
                            <ul>
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Universe</li>
                                <li>Dc Power Visa</li>
                            </ul>
                    </div>
                     <div class="footer-dx">
                        <img src="/image/dc-logo-bg.png" alt="">
                    </div>
                </div>
            </div>
    
            <div class="background-black">
                <div class="container">
                    <button>SING-UP NOW&#33;</button>

                    <div class="social-link">
                       <h3>FOLLOW US</h3>

                    </div>
                </div>
            </div>
    </footer>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .background-blue{
        background-color: $color-blue;
        
        .cols{
            @include center;
            justify-content: space-between;

            span{
                text-transform: uppercase;
                color: white;
                vertical-align: middle;
            }
        }

    }

    .background-image{
        background-image: url('/image/footer-bg.jpg');
        background-size: cover;

        .container{
            background-image: url('/img/dc-logo-bg.png');
            background-position: right center;
            background-repeat: no-repeat;
            display: flex;
            .footer-sx{
                display: flex;
                margin: 20px 0;
            }

            .col{
                margin: 60px 5px;
                line-height: 2;

                li{
                    color: rgb(167, 163, 163);
                    font-size: 12px;
                }

                h4{
                    color: white;
                    text-transform: uppercase;
                    font-weight: 800;
                    font-family: 'Roboto', sans-serif;
                }

                ul{
                    list-style: none;
                }
            }
        }
    }

    .background-black{
        background-color: rgb(50, 49, 49);
        padding: 30px 0;

        button{
            padding: 10px;
            background-color: transparent;
            border: 2px solid $color-blue;
            color: white;
            cursor: pointer;
        }

        .social-link{
            

            h3{
                color: $color-blue;
                font-family: 'Roboto', sans-serif;
                font-weight: 800;
    
            }
        }
       

        
    }





</style>