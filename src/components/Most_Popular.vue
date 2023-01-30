<template lang="">
    <div class="Most_Popular flex justify-center w-full flex-col">
            <div class="title flex flex-col justify-center items-center">
                <h1 class="par mt-5 font-medium text-[#282529]">Most Popular</h1>
                <p class="par text-[18px] font-normal">Most recent Watch Faces shared by our Community</p>
            </div>
            <div class="listofwatch flex  flex-wrap justify-center items-center w-full px-14 container  mx-auto">
                <div class="liof flex justify-start flex-wrap ">
                    <div v-for="item in listofwetches" :key="item.id"  class="watch my-[60px] mx-auto immg h-[380px] flex items-center flex-col justify-center  " >
                        <img class="" :src="item.img" alt="dd">
                        <p class="par text-center text-[20px]">{{item.title}}</p>
                    </div>

                </div>
            </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            listofwetches:[
                {title:'Gucci Gucci',img:'watches/Watch.png'},
                {title:'Rolex #1',img:'watches/Watch1.png'},
                {title:'Breitling classic',img:'watches/Watch2.png'},
                {title:'Gucci Gucci',img:'watches/Watch3.png'},
                {title:'Gucci Gucci',img:'watches/Watch4.png'},
                {title:'Gucci Gucci',img:'watches/Watch5.png'},
                {title:'Gucci Gucci',img:'watches/Watch6.png'},
                {title:'Gucci Gucci',img:'watches/Watch7.png'},
                {title:'Gucci Gucci',img:'watches/Watch8.png'},
                {title:'Rolex #1',img:'watches/Watch9.png'},
                {title:'Breitling classic',img:'watches/Watch10.png'},
                {title:'Gucci Gucci',img:'watches/Watch11.png'},
                {title:'Gucci Gucci',img:'watches/Watch12.png'},
                {title:'Gucci Gucci',img:'watches/Watch13.png'},
                {title:'Gucci Gucci',img:'watches/Watch14.png'},
                {title:'Gucci Gucci',img:'watches/Watch15.png'},
            ]
        }
    },
    
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');

.par {
    font-family: 'SF Pro Display', sans-serif;
    font-style: normal;
    
}
.immg {
    min-width: calc(100% * (1/4) - 10px - 1px);
    /* width: calc(100% * (1/4) - 10px - 1px) */
}
</style>