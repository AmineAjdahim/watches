<template lang="">
  <div class="homepage h-screen">
    <div class="h1  w-full bg-[#F9F9F9] h-screen">
      <div class="nav container mx-auto px-4">
        <Navbar/>
      </div>
      <div class="cont">
        <div class="content ">
        <Hero />
        </div>
        <div class="Most py-6 text-[64px]">
          <Most_Popular/>
        </div>
      </div>
    </div>
  </div>
  
</template>
<script>
import Navbar from '../components/Navbar.vue';
import Hero from '../components/Hero.vue';
import Most_Popular from '../components/Most_Popular.vue';
export default {
  data() {
    return {
      
    }
  },
  components:{
    Navbar,
    Hero,
    Most_Popular
  },  
  
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');
.divider {
  /* Divider */


}
  
</style>