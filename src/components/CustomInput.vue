<script setup>
   const props =  defineProps({
        text: {
            type: String
        },

        disabled: {
            type: Boolean,
            default: false
        },

        type: {
            type: String,
            default: 'text',
        },

        id: String,

        size: String,

        classes: {
            type: Array,
            default: () => []
        }
    });
</script>

<template>
    <div :class="[...classes, size, 'mb-3']">
        <label 
            :for="id" 
            class="form-label">
            {{ text }}
        </label>
        <input 
            :type="type" 
            class="form-control"
            :id="id" 
            :placeholder="text"
            :disabled="disabled">
    </div>
</template>
