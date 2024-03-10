<template>
    <div class="absolute z-10 flex flex-col w-64 p-1 text-sm rounded shadow bg-dark-light">

        <button
            v-for="item in items"
            class="relative flex items-center justify-between p-3 text-left rounded group hover:bg-dark-lighter"
        >
            <div>{{ item.title }}</div>
            <div>
                <ArrowTopRightOnSquare v-if="item.icon == 'ArrowTopRightOnSquare'"></ArrowTopRightOnSquare>
                <ChevronRight v-if="item.icon == 'ChevronRight'"></ChevronRight>
            </div>

            <div class="absolute hidden group-hover:block left-[100%] top-0">
                <Dropdown
                    v-if="item.items != null"
                    :items="item.items"
                ></Dropdown>
            </div>
        </button>

    </div>
</template>

<script setup>
import ArrowTopRightOnSquare from './Icons/ArrowTopRightOnSquare.vue';
import ChevronRight from './Icons/ChevronRight.vue';

defineProps({
    items: Array,
});
</script>
