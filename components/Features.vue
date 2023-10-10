<template>
    <div>
        <Heading title="Why Choose Salonnz ?"
            description="Explore the most exciting feature-driven software design to add positive value to your salon & spa business with its long list of simple and must have features" />
        <div class="flex flex-wrap justify-center items-start mx-auto max-w-[1220px] h-[580px] mt-10">
            <div v-for="(card, index) in cards" :key="index" class="w-full sm:w-1/2 md:w-1/3 lg:w-1/4 xl:w-1/3 p-4">
                <div class="flex flex-col h-[580px] bg-white rounded-lg shadow-md p-4">
                    <img :src="card.imageSrc" :alt="'Card ' + (index + 1)" class="w-[80%] h-[280px] mb-4 object-cover" />
                    <h2 class="text-xl font-semibold mb-2">{{ card.title }}</h2>
                    <p class="text-gray-600">{{ card.description }}</p>

                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            cards: [
                {
                    imageSrc: 'https://i.ibb.co/r7HMxN9/Group-1171276112.png',
                    title: 'Automate Email & SMS',
                    description: 'Send your clients various automated reminders such as appointment reminders, appointment details, booking status, birthday messages and many more. This feature is also inclusive to staff members. Have automated mails sent to your staff reminding them of upcoming, pending, and cancelled appointments. Digitalise customer communication, and spend more time on your work.',
                },
                {
                    imageSrc: 'https://i.ibb.co/KVhGDFF/Group-1171276112-1.png',
                    title: 'Inventory Management',
                    description: 'One of the most difficult challenges in managing a business is effectively tracking and organizing inventory. Salonnz provides you a flow of quick access, easier planning and streamlining of inventory.  Reduce any risk of overselling and avoid excess stock. ',
                },
                {
                    imageSrc: 'https://i.ibb.co/VVZHLym/Group-1171276112-2.png',
                    title: 'Online Appointment Booking',
                    description: 'Most salon owners struggle keeping in touch with their customers and managing appointments at the same time.  Salon Management App is a software that will solve all worries. With our software, your clients can choose what service they want and book their appointments instantly. With an automatic payment system, organizing and managing your salon appointments will be much easier.',
                },
                {
                    imageSrc: 'https://i.ibb.co/MVBnbN4/Group-1171276112-3.png',
                    title: 'Staff Management',
                    description: 'Business grows with productive staffs. Get to know & evaluate their performance easily. Track staff performance, sales & services, Set custom commission rates & Salonnz calculates payroll for staff. Using Salonnz Management App will allow you to pick a time with your preferred staff at your convenience.',
                },
                {
                    imageSrc: 'https://i.ibb.co/PmpZKQ5/Rectangle-9145-1.png',
                    title: 'Notifications & Reminders',
                    description: 'Set reminders to customers regarding Appointments, follow-ups, outstanding, payments, etc to increase sales. Salonnz comes with the functionality to send automated notifications to clients regarding their appointments, payments, and deals.',
                },
                {
                    imageSrc: 'https://i.ibb.co/MMswmFv/Rectangle-9145.png',
                    title: 'Reporting',
                    description: 'Salon management application enables you to track and measure your business achievements through advanced reports. Our platforms enables managers to monitor and control finances and progresses. This feature provides instant visibility and easy access to business reports and statestics. ',
                },

            ],
        };
    },
};
</script>