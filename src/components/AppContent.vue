<script>
import CurrentSeries from './CurrentSeries.vue';

export default {
    components:{
        CurrentSeries
    },
        data(){
            return{
            series: [
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                        price: "$19.99",
                        series: "ACTION COMICS",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                        price: "$3.99",
                        series: "AMERICAN VAMPIRE 1976",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                        price: "$16.99",
                        series: "AQUAMAN",
                        type: "graphic novel"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                        price: "$2.99",
                        series: "BATGIRL",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        price: "$3.99",
                        series: "BATMAN",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        price: "$2.99",
                        series: "BATMAN BEYOND",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                        price: "$3.99",
                        series: "BATMAN/SUPERMAN",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                        price: "$4.99",
                        series: "BATMAN/SUPERMAN ANNUAL",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                        price: "$5.99",
                        series: "BATMAN: THE JOKER WAR ZONE",
                        type: "comic book"
                    },
                    { 
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                        price: "$6.99",
                        series: "BATMAN: THREE JOKER",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                        price: "$4.99",
                        series: "BATMAN: WHITE KNIGHT PRESENTS: HARLEY QUINN",
                        type: "comic book"
                    },
                    {
                        thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                        price: "$16.99",
                        series: "CATWOMAN",
                        type: "graphic novel"
                    }
                ]
            }
        }
    }
</script>

<template lang="">
    <div class="bg-black">
        <div class="container">
            <div class="row">
                <CurrentSeries v-for="(item, index) in series" :key="index" :series="item"/>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>

    .bg-black{
        background-color: rgb(28, 28, 28);
        padding: 20px 0px;
    }

    .row{
        display: flex;
        flex-wrap: wrap;
    }
    
</style>