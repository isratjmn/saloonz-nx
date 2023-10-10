
<template>
    <div class="my-accordion mt-[700px] max-w-[1220px] mx-auto">
        <div v-for="(item, index) in accordionItems" :key="index">
            <div @click="toggleItem(index)" class="accordion-header">
                <h3>{{ item.title }}</h3>
                <span :class="{ 'rotate-arrow': activeItem === index }" class="arrow-button">
                    &#9660; <!-- Down arrow icon -->
                </span>
            </div>
            <div v-show="activeItem === index" class="accordion-content">
                {{ item.content }}
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            accordionItems: [
                {
                    title: "Section 1",
                    content: "lorem30",
                },
                {
                    title: "Section 2",
                    content: "Content for Section 2",
                },
                {
                    title: "Section 3",
                    content: "Content for Section 3",
                },
                {
                    title: "Section 4",
                    content: "Content for Section 4",
                },
            ],
            activeItem: null,
        };
    },
    methods: {
        toggleItem(index) {
            if (this.activeItem === index) {
                this.activeItem = null;
            } else {
                this.activeItem = index;
            }
        },
    },
};
</script>
  
<style>
.my-accordion {
    width: 100%;
}

.accordion-header {
    display: flex;
    justify-content: space-between;
    background-color: #f0f0f0;
    cursor: pointer;
    padding: 10px;
    border: 1px solid #ddd;
}

.arrow-button {
    cursor: pointer;
}

.rotate-arrow {
    transform: rotate(180deg);
}

.accordion-content {
    display: none;
    padding: 10px;
    border: 1px solid #ddd;
}
</style>
  