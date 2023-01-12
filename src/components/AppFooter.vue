<script>
export default {
    data(){
        return{
            image: '/footer-bg.jpg'
        }
    },
    methods: {
        getImageUrl($img){
            return new URL(`../assets/image/`)
        }
    }
    
}
</script>

<template lang="">
    <footer>
        <div class="container">
            <div class="background-prim">

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
    
            <div class="background-second">
    
            </div>
        </div>

    </footer>
</template>

<style lang="scss">
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;


</style>