<template>
    <div class="group p-2 flex justify-between items-center hover:bg-dark-light rounded">
        <div class="w-1/3 pl-4 flex items-center gap-x-4">
            <div class="w-6">
                <div class="group-hover:hidden">{{ trackNumber }}</div>
                <svg class="group-hover:block hidden top-[30%] left-[30%] w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M5.25 5.653c0-.856.917-1.398 1.667-.986l11.54 6.348a1.125 1.125 0 010 1.971l-11.54 6.347a1.125 1.125 0 01-1.667-.985V5.653z" />
                </svg>
            </div>
            <div class="relative">
                <img class="w-12 group-hover:brightness-50" :src="image" alt="">
            </div>
            <div>
                <h3>{{ trackName }}</h3>
            </div>
        </div>

        <div class="text-light-secondary group-hover:text-light-primary">
            12.023.023
        </div>

        <div class="flex gap-x-4">
            <div class="px-5">
                <Like
                    :like="like"
                >
                </Like>
            </div>
            <div class="text-light-secondary">
                {{ duration }}
            </div>
            <div>
                <svg class="opacity-0 group-hover:opacity-100 w-6 h-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M6.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM12.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0zM18.75 12a.75.75 0 11-1.5 0 .75.75 0 011.5 0z" />
                </svg>
            </div>
        </div>
    </div>
</template>

<script setup>
import Like from './Like.vue';

defineProps({
    trackNumber: Number,
    image: String,
    trackName: String,
    duration: String,
    like: Boolean,
});
</script>
