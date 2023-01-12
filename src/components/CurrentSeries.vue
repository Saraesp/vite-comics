<script>
 export default{
    props:{
        series:{
            series: Object
        }
    }

}

</script>

<template lang="">
    <div class="card">
        <div class="carde-image">
            <img :src="series.thumb" alt="">
        </div>
        <div class="card-title">
            {{series.series}}
        </div>
    </div>
</template>
<style lang="scss">

    .card{
        width: 15%;
        color: white;
        
        .card-image{

        }
        .card-title{
            font-size: 13px;
            font-family: 'Roboto', sans-serif;
            font-weight: 400;
        }
    }
    
</style>