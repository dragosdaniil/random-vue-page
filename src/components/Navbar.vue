<template>
    <aside :class="showBar? 'w-48 p-4 bg-black h-screen flex flex-col items-center gap-8 transition-all	' : 'w-16 p-4 bg-black h-screen flex flex-col items-center gap-8 transition-all	'">
        <button id="toggle-navbar" class="p-2 text-white hover:bg-green-700 rounded" v-on:click="showBar = !showBar">
            <span class="iconify" data-icon="fontisto:nav-icon-a"></span>
        </button>
        <div v-if="showBar" id="container" class="flex flex-col items-center gap-8">
            <Button v-for="(button, index) in buttons" :key="index" :content="button"/>
        </div>
    </aside>
</template>

<script>
import Button from  './Button.vue'
export default {
    name: 'Navbar',
    components:{
        Button
    },
    data() {
        return {
            buttons:['Home','About','Contact','Cart'],
            showBar:false
        }
    },
    methods: {
        
    },
}

</script>