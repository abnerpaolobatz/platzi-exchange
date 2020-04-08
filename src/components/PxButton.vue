<template>
    <button
        @click="buttonClick"
        class="bg_transparente hover:bg-green-500 text-green-700 font-semicolon"
    >
        <slot> </slot>
    </button>
</template>

<script>
export default {
    name: 'PxButton',

    methods: {
        buttonClick() {
            this.$emit('click')
        }
    }
}
</script>
