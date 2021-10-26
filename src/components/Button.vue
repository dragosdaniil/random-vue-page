<template>
    <button class="w-32 h-10 rounded-xl border-2 p-4 border-gray-700 hover:bg-green-700 text-white flex flex-row justify-between items-center">
        <span class="iconify" data-icon="jam:inboxes"></span>
        <span class="">{{content}}</span>
    </button>
</template>
<script>

export default {
    name:'Button',
    props:{
        content:String
    },
    data() {
        return {
            
        }
    },
    methods: {
        
    },
    mounted() {
        console.log(this.content);
    },
    updated() {
        
    },
}

</script>