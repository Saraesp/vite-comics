<script>
    export default {
        data(){
            return{
                menu: [
                    {
                      label: 'CHARACTERS',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'COMICS',
                      url: '#',
                      active: true
                    },
                    {
                      label: 'MOVIES',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'TV',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'GAMES',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'COLLECTIOBLES',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'VIDEOS',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'FANS',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'NEWS',
                      url: '#',
                      active: false
                    },
                    {
                      label: 'SHOP',
                      url: '#',
                      active: false
                    }
                ]
            }
        }
    }
</script>

<template lang="">
    <header class="container">
        <a href="">
            <img class="logo" src="/image/dc-logo.png" alt="">
        </a>
        <nav>
            <ul>
                <li v-for="(item, index) in menu" :key="index" :class="item.active ? 'active' : ''">
                    <a :href="item.url">
                        {{item.label}}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    header{
        height: 150px;
        @include center;
        justify-content: space-between;
        margin: 10px;

        nav{
            @include center;
            height: 100%;
            
            ul{
                height: 100%;
                list-style: none;
                margin: 2rem 1rem;
                @include center;

                li{
                    height: 100%;
                    padding: 1rem;
                    font-size: 13px;
                    font-family: 'Roboto', sans-serif;
                    font-weight: 500;
                    @include center;
                    
                    &.active {
                        border-bottom: $border-bottom;
                            
                        a{
                            color: $color-blue;
                        }
                        
                    }

                    &:hover{
                        border-bottom: $border-bottom;
                    }

                    a:hover{
                        color: $color-blue;
                    }
            }
            
            }
        }


    }

    .logo{
        width: 90px;
        margin-right: 100px;
    }
</style>