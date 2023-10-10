<template>
    <button
      class="bg-[#ED2D66] hover:bg-[#9d6072bf] text-white font-bold py-2 px-5 rounded"
      @click="handleClick"
    >
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