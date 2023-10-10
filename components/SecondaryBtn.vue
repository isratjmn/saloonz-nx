<template>
    <button
        class="border border-pink-500 hover:border-pink-600 text-pink-500 hover:text-pink-600 font-bold py-2 px-5 rounded"
        @click="handleClick">
        {{ label }}
    </button>
</template>
  
<script>
export default {
    props: {
        label: String,
    },
    methods: {
        handleClick() {
            // Handle button click event here
            this.$emit('click');
        },
    },
};
</script>
  