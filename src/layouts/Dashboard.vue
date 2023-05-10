<template>
    <div class="bg-gray-800 flex text-white max-h-screen h-screen">
        <div class="w-64">
            <span class="font-semibold p-6 block opacity-90">skateboard</span>

        <nav class="p-6">
            <h3 class="opacity-50 uppercase font-semibold tracking-wider mb-3 text-xs">Menu</h3>

            <div class="space-y-6">
                <MenuItems :icon="HomeIcon">Discover</MenuItems>
                <MenuItems :icon="TrendingUpIcon">Trending</MenuItems>
                <MenuItems :icon="TrendingUpIcon">Trending</MenuItems>
                <MenuItems :icon="TrendingUpIcon">Trending</MenuItems>
                <MenuItems :icon="TrendingUpIcon">Trending</MenuItems>
                <MenuItems :icon="TrendingUpIcon">Trending</MenuItems>
            </div>
        </nav>
    </div>
        
        <div class="p-5 flex-1">
            <header class="flex items-center justify-between">
                <InputSearch class="w-96"/>

                <div class="flex items-center ">
                    <div class="flex items-center space-x-3">
                        <div class="w-10 h-10">
                            <Avatar class="rounded-full"/>
                        </div>
                    
                        <span>Thomas</span>
                        <ChevronDownIcon class="w-4 h-4" />
                    </div>

                    <BellIcon class="w-5 h-5 ml-8 opacity-50 hover:opacity-100 cursor-pointer transition duration-100"/>
                </div>
            </header>
        </div>
    </div>
</template>

<script>
import HomeIcon from '../components/icons/HomeIcon.vue'
import TrendingUpIcon from '../components/icons/TrendingUpIcon.vue'
import ChevronDownIcon from '../components/icons/ChevronDownIcon.vue'
import BellIcon from '../components/icons/BellIcon.vue'
import MenuItems from './navs/MenuItem.vue'
import InputSearch from '../components/inputs/InputSearch.vue'
import Avatar from '../components/Avatar.vue'

export default {
    components: {
        HomeIcon,
        TrendingUpIcon,
        ChevronDownIcon,
        BellIcon,
        MenuItems,
        InputSearch,
        Avatar
    },
}
</script>

