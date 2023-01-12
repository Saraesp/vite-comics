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
                <div v-for="(item, index) in imagesBackgroundBlue" :key="index">
                    <img :src="`/image/${item.image}.png`">
                    <span>{{item.label}}</span>
                </div>
            </div>

            <div class="background-image">
                <div>
                    <h4></h4>
                    <nav>
                        <ul>
                            
                        </ul>
                    </nav>
                </div>

                <div>
                    <h4></h4>
                    <nav>
                        <ul>
                            
                        </ul>
                    </nav>
                </div>
    
                <div>
                    <h4></h4>
                    <nav>
                        <ul>
                            
                        </ul>
                    </nav>
                </div>
    
            </div>
    
            <div class="background-black">
    
            </div>
    </footer>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    .background-blue{
        height: 100px;
        display: flex;
        justify-content: space-between;
        background-color: $color-blue;

        span{
            text-transform: uppercase;
            color: white;
            vertical-align: middle;
        }
    }



</style>