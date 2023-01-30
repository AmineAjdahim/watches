<template lang="">
    <div class="nav w-full bg-[#F9F9F9] flex items-center min-h-[80px] max-h-[80px] ">
        <div class="allnavs justify-between container flex items-center mx-auto px-4 py-1">
            <div class="logo-title flex  items-center">
                <div class="logo w-[30px]">
                    <img class="w-[30px]" src="/logo.svg" alt="">
                </div>
                <div class="tit text-[22px] px-2">
                    <h1>Watch Faces</h1>
                </div>
        
            </div>
            <div class="list  text-[16px] flex-col hidden lg:flex">
                <div class="lo flex justify-center ">
                    <li class="ls flex justify-center flex-col item-center cursor-pointer px-[28px]" v-for="list in listofnav" :key="list.id">
                       <p> {{list.title}} </p>
                       
                       <p v-if="list.title == 'Home'" class="flex  w-[28px] justify-center  mx-auto h-[1px]  bg-[#5A45D6]"></p>
                    </li>
                </div>
            </div>
            <div class="list ls hidden lg:flex w-[160px] h-[40px] text-center justify-center text-white rounded-[69px] bg-[#5A45D6] text-[14px]">
                <button>Try it Now</button>
            </div>
            <div class="vector lg:hidden flex">
                    <svg width="26" height="18" viewBox="0 0 26 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                         <path d="M1 9H25M1 1H25M9 17H25" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>

            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            listofnav:[{title:"Home"},{title:"Blog"},{title:"Contact"}]
        }
    },
    
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/hk-groteks');
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');

.tit {
    font-family: 'HK Grotesk', sans-serif;
    font-weight: 700;

}
.ls{
    font-family: 'SF Pro Display', sans-serif;
                                                
}
</style>