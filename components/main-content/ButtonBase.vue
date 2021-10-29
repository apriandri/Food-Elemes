<template>
    <div>
        <button class="px-4 py-2 rounded-full" :class="type" :disabled="disabled">
            <slot>{{ buttonText }}</slot>
        </button>
    </div>
</template>

<style>
</style>

<script>
export default {
    name: 'ButtonBase',
    props: {
        buttonText : {
            type: String,
            require: true
        },
        type: String,
        disabled: Boolean

    },
}
</script>