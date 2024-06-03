<template>
  <div class="p-5">
    <div class="flex max-sm:block justify-between items-center pb-5">
        <div class="flex gap-10">
            <p class="text-2xl tracking-widest text-red-500 cursor-pointer max-sm:pl-32">PHLOX</p>
            <div :class="{'max-sm:block': isMenuVisible, 'max-sm:hidden': !isMenuVisible}" class="max-sm:absolute max-sm:h-[500px] max-sm:w-[370px] max-sm:top-0 max-sm:mt-2 max-sm:right-[0px] max-sm:mx-2 max-sm:bg-black max-sm:text-left max-sm:z-30 max-sm:duration-500">
                <i class="icon ion-md-close max-sm:block text-white max-sm:m-[10px] hidden cursor-pointer text-2xl" @click="menuHandle"></i>
                <ul class="flex gap-10 text-gray-500 text-lg max-sm:block max-sm:text-center pt-0.5">
                    <li class="cursor-pointer max-sm:py-[5px] max-sm:px-[50px] max-sm:duration-500 max-sm:text-white max-sm:mt-5 max-sm:hover:text-orange-500">Home</li>
                    <li class="cursor-pointer max-sm:py-[5px] max-sm:px-[50px] max-sm:duration-500 max-sm:text-white max-sm:mt-5 max-sm:hover:text-orange-500">Shop</li>
                    <li class="cursor-pointer max-sm:py-[5px] max-sm:px-[50px] max-sm:duration-500 max-sm:text-white max-sm:mt-5 max-sm:hover:text-orange-500">About Us</li>
                    <li class="cursor-pointer max-sm:py-[5px] max-sm:px-[50px] max-sm:duration-500 max-sm:text-white max-sm:mt-5 max-sm:hover:text-orange-500">Blog</li>
                    <li class="cursor-pointer max-sm:py-[5px] max-sm:px-[50px] max-sm:duration-500 max-sm:text-white max-sm:mt-5 max-sm:hover:text-orange-500">contact Us</li>
                </ul>
            </div>
            <i class="icon ion-md-menu absolute top-0 right-0 max-sm:block max-sm:m-[10px] hidden cursor-pointer text-2xl pb-3" @click="menuHandle"></i>
        </div>
        <div class="flex justify-between text-right bg-gray-200 h-10 pl-5 rounded-full">
            <input class="bg-gray-200 outline-none" type="text" name="search" placeholder="Search product">
            <i class="icon ion-ios-search bg-green-500 px-7 pt-1 text-xl rounded-full"></i>
        </div>
    </div>
    <div class="bg-[url(../../public/img/main-page.jpg)] h-[600px] max-sm:h-[570px] container bg-no-repeat bg-center bg-cover relative p-10 rounded-3xl">
        <div class="absolute top-0 bottom-0 right-0 left-0 bg-[rgba(0,0,0,0.5)] z-10 rounded-3xl"></div>
        <div class="z-20 relative mt-24 ml-24 max-sm:m-0 max-sm:pt-24">
            <div class="leading-6">
                <p class="text-gray-400 text-lg font-medium pl-2 max-sm:text-sm max-sm:pl-0">Beats Solo</p>
                <p class="text-gray-400 text-5xl font-medium pl-2 max-sm:text-4xl max-sm:pl-0 max-sm:pt-1">Wireless</p>
                <p class="text-white text-9xl max-sm:text-5xl max-sm:pt-1">HEADPHONE</p>
                <button class="text-white text-xs bg-red-600 px-6 py-2 rounded-full font-medium mt-3 max-sm:mt-3">Shop By Category</button>
            </div>
        </div>
        <div class="text-white z-20 relative w-full text-right mt-5 max-sm:mt-12 pr-24 max-sm:pr-0">
            <p class="font-medium text-lg">Description</p>
            <p class="text-sm">There are many variations passages of <br> Lorem Ipsum availaple, but the majority <br> have suffered alteration</p>
        </div>
    </div>
    <product-browse></product-browse>
    <features></features>
    <smile></smile>
    <best-seller-products></best-seller-products>
    <hours></hours>
    <recent-news></recent-news>
    <Footer></Footer>
  </div>
</template>

<script>
import ProductBrowse from '@/components/ProductBrowse.vue';
import Features from '@/components/Features.vue';
import Smile from '@/components/Smile.vue';
import BestSellerProducts from '@/components/BestSellerProducts.vue';
import Hours from '@/components/Hours.vue';
import RecentNews from '@/components/RecentNews.vue';
import Footer from './Footer.vue';

export default {
  components: { ProductBrowse, Features, Smile, BestSellerProducts, Hours, RecentNews, Footer },
    name: 'Home',
    data() {
        return {
            isMenuVisible: false,
        }
    },
    methods: {
      menuHandle(){
        this.isMenuVisible = !this.isMenuVisible
      }
    },
}
</script>