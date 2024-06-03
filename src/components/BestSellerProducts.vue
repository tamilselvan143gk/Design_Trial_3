<template>
  <div class="mx-3">
    <div class="text-center mt-32">
        <p class="text-4xl font-medium">Best Seller Products</p>
        <p class="text-sm text-gray-500 mt-2">Speaker there are many variation passages</p>
        <div class="h-[3px] w-20 mx-auto bg-orange-500 mt-5"></div>
    </div>
    <div class="grid grid-cols-4 gap-x-10 gap-y-20 mt-20 max-sm:block">
        <div v-for="product in products" :key="product" class="max-sm:mt-5">
            <div class="relative">
                <img :src="product.img" class="h-60 w-[350px] rounded-3xl">
                <p v-if="product.sale === 'Sale'" class="absolute top-5 left-5 bg-red-500 text-white text-sm font-medium py-3.5 px-3 rounded-full">{{ product.sale }}</p>
            </div>
            <div>
                <p class="text-lg font-medium">{{ product.name }}</p>
                <p class="font-medium text-lg">₹{{ formatAmount(product.amount) }}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BestSellerProduct',
    data() {
        return {
            products: [
                { name: 'Beats', amount: 995, img: '../../public/img/bst/beats.jpg', sale: '' },
                { name: 'Rocky Mountain', amount: 8250, img: '../../public/img/bst/rocky-mountain.jpg', sale: '' },
                { name: 'Game Console Controller Cable', amount: 8250, img: '../../public/img/bst/game-console-controller.jpg', sale: '' },
                { name: 'White ElitBook Tablet 810', amount: 9950, img: '../../public/img/bst/white-elitbook-tablet.jpg', sale: 'Sale' },
                { name: 'Gore Wear C7', amount: 499, img: '../../public/img/bst/gore-wear-c7.jpg', sale: '' },
                { name: 'Wireless Audio System Multiroom 360', amount: 8250, img: '../../public/img/bst/wireless-audio-system.jpg', sale: '' },
                { name: 'Beats', amount: 9950, img: '../../public/img/bst/beats-2.jpg', sale: 'Sale' },
                { name: 'Smartwatch 2.0 LTE W6', amount: 499, img: '../../public/img/bst/smart-watch.jpg', sale: '' },
            ]
        }
    },
    methods: {
    formatAmount(amount) {
      return amount.toLocaleString('en-IN');
    }
  }
}
</script>