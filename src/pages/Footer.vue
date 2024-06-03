<template>
  <div class="flex justify-between mt-20 max-sm:block max-sm:text-center">
    <div>
      <p class="text-xl tracking-widest text-red-500 cursor-pointer">PHLOX</p>
      <p class="text-sm mt-5 text-gray-500 max-sm:mt-2">The are many variations <br> passages of Lorem Ipsum availaple, <br> but the majority have</p>
      <div class="flex gap-5 mt-2 text-2xl max-sm:justify-center">
        <i class="icon ion-logo-instagram"></i>
        <i class="icon ion-logo-linkedin"></i>
        <i class="icon ion-logo-facebook"></i>
        <i class="icon ion-logo-twitter"></i>
      </div>
    </div>
    <quick-links></quick-links>
    <contact-for-footer></contact-for-footer>
    <subscipe></subscipe>
  </div>
</template>

<script>
import QuickLinks from '@/components/QuickLinks.vue';
import ContactForFooter from '@/components/ContactForFooter.vue';
import Subscipe from '@/components/Subscipe.vue';

export default {
  components: { QuickLinks, ContactForFooter, Subscipe },
  name: 'Footer',
}
</script>