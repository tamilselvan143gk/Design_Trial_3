<template>
  <div class="mx-3">
    <div class="text-center mt-32">
        <p class="text-4xl font-medium">Recent News</p>
        <p class="text-sm text-gray-500 mt-2">There are many variation passages</p>
        <div class="h-[3px] w-20 mx-auto bg-orange-500 mt-5"></div>
    </div>
    <div class="flex gap-10 mt-10 max-sm:block">
        <div v-for="recent in recentNews" :key="recent" class="max-sm:mb-10">
            <div>
                <img class="h-60 w-full rounded-3xl" :src="recent.img">
                <p class="text-sm text-gray-500 mt-5">{{ recent.date }}</p>
            </div>
            <div>
                <p class="font-medium text-lg mt-2">{{ recent.title }}</p>
                <p class="text-xs pr-20 mt-2">{{ recent.content }}</p>
            </div>
        </div>
    </div>
  </div>
  <div class="flex justify-between mt-10 bg-gray-200 p-5 -mx-5 items-center max-sm:block py-10">
    <img class="mix-blend-darken h-28 opacity-50 max-sm:mx-auto" src="../../public/img/golden.jpg">
    <img class="mix-blend-darken h-28 opacity-50 max-sm:mx-auto" src="../../public/img/sweety.jpg">
    <img class="mix-blend-darken h-20 opacity-50 max-sm:mx-auto max-sm:mt-10" src="../../public/img/fastlane.png">
    <img class="mix-blend-darken h-20 opacity-50 max-sm:mx-auto max-sm:mt-20" src="../../public/img/mighty.png">
    <img class="mix-blend-darken h-28 opacity-50 max-sm:mx-auto max-sm:mt-10" src="../../public/img/jr.png">
  </div>
</template>

<script>
export default {
    name: 'RecentNews',
    data() {
        return {
            recentNews: [
                { img: '../../public/img/recent-1.jpg', date: 'May 31, 2024', title: 'How to choose perfect gadgets', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio totam minima quae iste corporis nobis labore sed, quasi sint. ' },
                { img: '../../public/img/recent-2.jpg', date: 'May 31, 2024', title: 'How to choose perfect gadgets', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio totam minima quae iste corporis nobis labore sed, quasi sint. ' },
                { img: '../../public/img/recent-3.jpg', date: 'May 31, 2024', title: 'How to choose perfect gadgets', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio totam minima quae iste corporis nobis labore sed, quasi sint. ' },
            ]
        }
    },
}
</script>