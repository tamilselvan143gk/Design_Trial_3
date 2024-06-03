<template>
  <div class="mt-8">
    <div class="text-center mb-10 text-3xl font-medium">
        <p>Explore Our Product</p>
        <div class="h-[3px] w-52 mx-auto bg-orange-500 mt-5"></div>
    </div>
    <div class="flex gap-5 max-sm:block">
        <div class="bg-[url(public/img/bluetooth.jpg)] h-[450px] w-[380px] bg-no-repeat rounded-2xl bg-cover bg-center flex items-center max-sm:w-[350px]">
            <div class="relative z-20 ml-10">
                <p class="text-white text-sm pl-1">Enjoy</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">With</p>
                <p class="text-gray-400 text-5xl font-medium pt-1">EARPHONE</p>
                <button class="text-white text-xs font-bold bg-red-600 px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
        <div class="bg-[url(public/img/watch.jpg)] h-[450px] w-[380px] bg-cover bg-left  bg-no-repeat rounded-2xl flex items-center max-sm:w-[350px] max-sm:mt-5">
            <div class="relative z-20 ml-10">
                <p class="text-white text-sm pl-1">New</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">Wear</p>
                <p class="text-yellow-200 text-5xl font-medium pt-1">GADGET</p>
                <button class="text-yellow-400 text-xs font-bold bg-white px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
        <div class="bg-[url(public/img/laptop.jpg)] h-[450px] w-[750px] bg-cover bg-center bg-no-repeat rounded-2xl flex items-center max-sm:w-[350px] max-sm:mt-5">
            <div class="relative z-20 ml-20 max-sm:ml-10">
                <p class="text-white text-sm pl-1">Trend</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">Devices</p>
                <p class="text-red-300 text-5xl font-medium pt-1">LAPTOP</p>
                <button class="text-red-500 text-xs font-bold bg-white px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
    </div>
    <div class="flex gap-5 mt-5 max-sm:block">
        <div class="bg-[url(public/img/gaming-console.jpg)] h-[450px] w-[750px] bg-no-repeat bg-cover bg-center rounded-2xl flex items-center max-sm:w-[350px]">
            <div class="relative z-20 ml-20 max-sm:ml-10">
                <p class="text-white text-sm pl-1">Best</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">Gaming</p>
                <p class="text-gray-400 text-5xl font-medium pt-1">CONSOLE</p>
                <button class="text-white text-xs font-bold bg-red-600 px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
        <div class="bg-[url(public/img/game-oculus.jpg)] h-[450px] w-[350px] bg-no-repeat bg-cover bg-center rounded-2xl flex items-center max-sm:w-[350px] max-sm:mt-5">
            <div class="relative z-20 ml-10">
                <p class="text-white text-sm pl-1">Play</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">Game</p>
                <p class="text-green-400 text-5xl font-medium pt-1">OCULUS</p>
                <button class="text-green-500 text-xs font-bold bg-white px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
        <div class="bg-[url(public/img/amazon-speaker.jpg)] h-[450px] w-[350px] bg-no-repeat bg-cover bg-center rounded-2xl flex items-center max-sm:w-[350px] max-sm:mt-5">
            <div class="relative z-20 ml-10">
                <p class="text-white text-sm pl-1">New</p>
                <p class="text-white text-3xl font-medium pt-1 pl-1">Amazon</p>
                <p class="text-indigo-300 text-5xl font-medium pt-1">SPEAKER</p>
                <button class="text-indigo-500 text-xs font-bold bg-white px-6 py-2 rounded-full mt-5">Browse</button>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'ProductBrowse'
}
</script>