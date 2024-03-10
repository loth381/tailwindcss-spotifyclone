<template>
    <div class="relative">
        <div @click="showMenu = false" @contextmenu.prevent="showMenu = true" class="group pt-1 h-[17rem] bg-dark hover:bg-dark-light rounded cursor-pointer">
            <div class="relative">
                <div
                    class="w-36 h-36 mx-auto mt-4 overflow-hidden"
                    v-bind:class="{
                        'rounded': shape == 'square',
                        'rounded-full': shape != 'square',
                    }"
                >
                    <img class="w-full h-full object-cover" v-bind:src="image" >
                </div>
                <button class="absolute right-5 bottom-1 opacity-0 group-hover:opacity-100 translate-y-5 group-hover:translate-y-0 transition">
                <svg class="w-16 h-16 text-green-primary" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                    <path stroke-linecap="round" stroke-linejoin="round" d="M15.91 11.672a.375.375 0 010 .656l-5.603 3.113a.375.375 0 01-.557-.328V8.887c0-.286.307-.466.557-.327l5.603 3.112z" />
                </svg>
                </button>
            </div>
            <div class="mx-5 mt-4">
                <h3 class="font-bold text-light-primary">{{ title }}</h3>
                <p class="text-sm overflow-hidden text-ellipsis line-clamp-2 text-light-secondary">{{ subTitle }}</p>
            </div>
        </div>

        <Dropdown
            v-if="showMenu"
            :style="`left: ${x}px; top: ${y}px;`"
            :items="[
                {
                    title: 'Seguir',
                    icon: null,
                    items: null,
                },
                {
                    title: 'Ir a radio del artista',
                    icon: null,
                    items: null,
                },
                {
                    title: 'Denunciar',
                    icon: 'ArrowTopRightOnSquare',
                    items: null,
                },
                {
                    title: 'Compartir',
                    icon: 'ChevronRight',
                    items: [
                        {
                            title: 'Copiar URI de Spotify',
                            icon: null,
                            items: null,
                        },
                        {
                            title: 'Insertar artista',
                            icon: null,
                            items: null,
                        },
                    ],
                },
                {
                    title: 'Abrir en la aplicación del ordenador',
                    icon: null,
                    items: null,
                },
            ]"
            ></Dropdown>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import Dropdown from './Dropdown.vue';
defineProps({
    title: String,
    subTitle: String,
    image: String,
    shape: String,
});

const x = 70;
const y = 50;
const showMenu = ref(false);
</script>
