<template>
    <div class="flex flex-col bg-white px-2 rounded-lg text-grey-7 overflow-hidden">
        <div class="py-4">
            <section class="flex-row inline-flex w-full justify-between">
                <div class="flex justify-between">
                    <svg viewBox="0 0 1024 1024" class="icon h-6" version="1.1" xmlns="http://www.w3.org/2000/svg"
                        fill="#000000">
                        <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                        <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                        <g id="SVGRepo_iconCarrier">
                            <path
                                d="M523.9 788.3H166.4V169c0-4.3 3.4-7.7 7.6-7.7h490.8c4.2 0 7.6 3.5 7.6 7.7v190h45.8V169c0-29.9-24-54.2-53.4-54.2H174c-29.5 0-53.4 24.3-53.4 54.2v689c0 29.9 24 54.2 53.4 54.2h359.1c-5.9-11.6-9.3-24.8-9.3-38.7v-85.2z m-102.6 96.2c-17 0-30.9-14-30.9-31.3s13.8-31.3 30.9-31.3c17 0 30.9 14 30.9 31.3-0.1 17.3-13.9 31.3-30.9 31.3z m442.9-479H607.9c-21.1 0-38.2 17.4-38.2 38.7v429.3c0 21.3 17.1 38.7 38.2 38.7h256.3c21.1 0 38.2-17.4 38.2-38.7V444.2c0-21.4-17.1-38.7-38.2-38.7zM736.1 888.9c-12.7 0-22.9-10.4-22.9-23.2 0-12.8 10.3-23.2 22.9-23.2 12.6 0 22.9 10.4 22.9 23.2 0 12.8-10.3 23.2-22.9 23.2z m120.5-69.7H615.5V451.9h241.1v367.3z"
                                fill="#5F9BEB"></path>
                        </g>
                    </svg>
                    <strong class="text-base text-xl mx-2 text-grey-7">Technology</strong>
                </div>

                <svg viewBox="0 0 1024 1024" class="icon h-6 " version="1.1" xmlns="http://www.w3.org/2000/svg"
                    fill="#000000">
                    <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                    <g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
                    <g id="SVGRepo_iconCarrier">
                        <path
                            d="M928.7 312.5L532.9 126.3c-15.2-7.1-33.6-7.1-48.7 0L88.3 312.5c-14.5 6.8-23.5 21-23.5 37s9 30.1 23.5 37l118.9 55.9v329.4c0 19.3 9.3 37.4 24.8 48.2 81.4 56.8 177 86.8 276.5 86.8s195.2-30 276.6-86.8c15.5-10.8 24.8-28.9 24.8-48.2V442.4l118.9-55.9c14.5-6.8 23.5-21 23.5-37-0.1-16-9.1-30.2-23.6-37zM760.8 771.8c0 3.3-1.5 6.3-3.8 8-73.1 51-159 78-248.5 78-89.4 0-175.4-27-248.5-78-2.4-1.6-3.8-4.7-3.8-8V465.4l228 107.3c7.6 3.6 16 5.4 24.4 5.4 8.4 0 16.8-1.9 24.3-5.4l228-107.3v306.4zM512 528.3c-2.2 1.1-4.7 1.1-6.9 0L124.9 349.5 505 170.6c2.2-1.1 4.7-1.1 6.9 0L892 349.5 512 528.3z"
                            fill="#3CB87F"></path>
                    </g>
                </svg>
            </section>
            <p class="text-grey-7 text-baseline text-center">
                Last updated: Mar 04, 2022, 2:06 PM
            </p>
        </div>
        <q-separator />
        <div class="my-3 flex justify-between">
            <span>
                History
            </span>
            <q-icon name="add" class="my-auto" size="20" />
        </div>
        <q-separator />
        <div class="my-3 font-bold flex justify-between">
            <span>
                Insights
            </span>
            <q-icon name="add" class="my-auto" size="20" />
        </div>

        <div class="pt-4 pb-2 flex justify-between">
            <span
                class="inline-block bg-gray-200 rounded-lg px-7 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">Book</span>
            <span
                class="inline-block bg-white rounded-lg  px-7 border py-1 text-sm font-semibold text-grey-7 mr-2 mb-2">Current
                Note</span>
        </div>
        <div class="px-6 py-4">
            <div class="flex-col space-y-2">
                <div class="col-span-1">
                    <span class="font-bold text-md ">4 notes</span>
                </div>
                <div class="col-span-1">
                    <span class="font-bold text-md ">32 photos</span>
                </div>
                <div class="col-span-1">
                    <span class="font-bold text-md ">4 videos</span>
                </div>
                <!-- ... more items here -->
            </div>
        </div>
        <div class="mt-4 pb-2">
            <q-separator />
            <div class="my-3 flex justify-between">
                <span>
                    Share
                </span>
                <q-icon name="add" class="my-auto" size="20" />
            </div>
            <q-separator />
            <div class="my-3 flex justify-between">
                <span>
                    Comments
                </span>
                <q-icon name="add" class="my-auto" size="20" />
            </div>
        </div>

        <!-- ... more sections here -->
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup() {
        // 
    },
})
</script>



  