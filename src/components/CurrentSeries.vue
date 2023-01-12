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
            <img :src="thumb.src" alt="">
        </div>
        <div class="card-title">
            {{series.series}}
        </div>
    </div>
</template>
<style lang="scss">

    .card{
        width: 25%;
        border: 1px solid black;
    }
    
</style>