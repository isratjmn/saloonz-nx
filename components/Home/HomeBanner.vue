<template>
    <div class="max-w-[1220px] mx-auto justify-center items-center flex-container pt-16 gap-6">
        <div class="left-content items-center mt-7">
            <h1 class="mb-4 font-bold text-5xl">Revolutionize Your Salon with Cutting-Edge Salon Software!</h1>
            <p class="mb-4 text-xl font-normal">Streamline Your Salon Business with Salon Software.</p>
            <div class="mt-12">
                <PrimaryBtn label="Book a Demo" @click="handlePrimaryButtonClick" class="mr-2" />
                <SecondaryBtn label="Contact Us" @click="handleSecondaryButtonClick" class="ml-2" />
            </div>
        </div>
        <div class="right-content">
            <img src="../../public/images/Group 1171276142.png" width="500" alt="Your Image" />

        </div>
    </div>
</template>

<script>
import PrimaryBtn from '@/components/PrimaryBtn.vue';
import SecondaryBtn from '@/components/SecondaryBtn.vue';

export default {
    components: {
        PrimaryBtn,
        SecondaryBtn,
    },
    methods: {
        handlePrimaryButtonClick() {
        },
        handleSecondaryButtonClick() {
        },
    },
};
</script>

<style scoped>
.flex-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.left-content {
    flex: 1;
}

.right-content {
    flex: 1;
    display: flex;
    justify-content: center;
}

.mb-4 {
    margin-bottom: 1rem;
}

.mb-2 {
    margin-bottom: 0.5rem;
}
</style>