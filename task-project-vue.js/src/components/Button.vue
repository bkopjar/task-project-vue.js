<template>
    <button @click="onClick()" :style="{background:color}" 
    class="btn">{{ text }}
    </button> <!-- Instead of @click you can put v-on:click="onClick()" -->   
</template>

<script>
export default {
    name: 'Button',
    props: {
        text: String,
        color: String,
    },
    methods: {
        onClick() {
            console.log('click')
        }
    }
}
</script>