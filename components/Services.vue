<template>
    <div>
        <Heading title="What we can do for your salon?"
            description="Start your day with Salonnz. Business management software that's flexible, dependable, and affordable. Automate appointments, track inventory, master marketing, integrate payments and more. Optimize operations with Salonnz."
            :features="salonFeatures" />
    </div>
    <div>
        <swiper :slidesPerView="4" :spaceBetween="10" :centeredSlides="true" :pagination="{ clickable: true }"
            :modules="modules" class="mySwiper">

            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/9ZL0pxz/Rectangle-9135-6.png" title="Website Design" />
                </swiper-slide>
            </swiper-slide>
            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/hX5FdJL/Rectangle-9135-4.png" title="Digital Marketing" />
                </swiper-slide>
            </swiper-slide>
            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/6N6By94/Rectangle-9135-5.png" title="Logo & Graphics" />
                </swiper-slide>
            </swiper-slide>
            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/mcyb9tv/Rectangle-9135-1.png" title="Custom Salon Apps" />
                </swiper-slide>
            </swiper-slide>
            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/kgPDfMd/Rectangle-9135.png" title="Salon Software" />
                </swiper-slide>
            </swiper-slide>
            <swiper-slide>
                <swiper-slide>
                    <CardCarousel imageSrc="https://i.ibb.co/NFTZMYv/Rectangle-9135-2.png" title="SEO" />
                </swiper-slide>
            </swiper-slide>

        </swiper>
    </div>
</template>

<script>
import Heading from '@/components/Heading.vue';
import CardCarousel from "@/components/CardCarousel.vue";
import { Swiper, SwiperSlide } from 'vue-awesome-swiper';
import 'swiper/swiper-bundle.css';

export default {
    components: {
        Heading,
        CardCarousel,
        Swiper,
        SwiperSlide,
    },


};
</script>