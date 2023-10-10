<template>
    <div class="card bg-gray-200 rounded-lg p-4 w-96 mx-auto text-center my-20">
        <img class="mx-auto text-center" width="150" :src="imageSrc" alt="CardImage" />
        <h2 class="font-bold text-xl my-4">{{ title }}</h2>
        <p>{{ description }}</p>
    </div>
</template>

<script>
export default {
    props: {
        imageSrc: String,
        title: String,
        description: String,
    },
};
</script>


