<template>
    <div class="text-center">
        <h1 class="text-4xl font-bold mb-4 mt-24">{{ title }}</h1>
        <p class="text-lg w-[919px] mx-auto">{{ description }}</p>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        description: String,
    },
};
</script>
