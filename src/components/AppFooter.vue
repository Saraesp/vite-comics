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
                <h4></h4>
                <nav>
                    <ul>
                        <li><a href=""></a></li>
                    </ul>
                </nav>
    
                <h4></h4>
                <nav>
                    <ul>
                        <li><a href=""></a></li>
                    </ul>
                </nav>
    
                <h4></h4>
                <nav>
                    <ul>
                        <li><a href=""></a></li>
                    </ul>
                </nav>
    
                <h4></h4>
                <nav>
                    <ul>
                        <li><a href=""></a></li>
                    </ul>
                </nav>
    
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