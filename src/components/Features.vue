<template>
  <div class="mt-20 mb-5">
    <div class="flex justify-between mx-10 max-sm:grid max-sm:grid-cols-2 max-sm:mx-0 max-sm:gap-5">
        <div v-for="feature in features" :key="feature" class="flex items-center gap-5 max-sm:block max-sm:text-center max-sm:p-2">
            <div>
                <i class="text-2xl text-red-600" :class="[feature.icon, { 'border-2 px-2 rounded-full border-red-600': feature.icon === 'icon ion-md-checkmark' }]"></i>
            </div>
            <div>
                <p class="text-sm font-bold">{{ feature.title }}</p>
                <p class="text-xs text-gray-600">{{ feature.content }}</p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Features',
    data() {
        return {
            features: [
                { title: 'Free Shipping', content: 'Free Shipping On All Orders', icon: 'icon ion-ios-briefcase' },
                { title: 'Money Guarantee', content: '30 Days Money Back', icon: 'icon ion-md-checkmark' },
                { title: 'Online Support 24/7', content: 'Technical Support 24/7', icon: 'icon ion-ios-call' },
                { title: 'Secure Payment', content: 'All cards accepted', icon: 'icon ion-md-wallet' },
            ]
        }
    },
}
</script>