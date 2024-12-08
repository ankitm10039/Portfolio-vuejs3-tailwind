<template >
    <section class="text-white mt-20" id="services">
        <div class="px-4 xl:pl-16">
            <h2 class="text-4xl font-medium text-white mb-4">My Services</h2>
        </div>
        <div class="py-8 xl:px-16 px-4 sm:py-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3">
            <div v-for="service in services" :key="service.id" data-aos="fade-up"
            class="px-8 py-12 rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641]"
            >
                <div class="mx-auto h-24 w-24 text-center xl:h-28 xl:w-28">
                    <div>
                        <img :src="service.icon" alt="service icon">
                    </div>
                </div>
                <div class="text-center">
                    <h3 class="pt-8 text-lg font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary lg:text-xl">
                        {{ service.name }}
                    </h3>
                    <p class="text-grey pt-4 text-sm group-hover:text-white md:text-base">
                        {{ service.description }}
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>
<script setup>
import {ref} from 'vue';
const services =ref([
    {
        id:1,
        icon:'https://img.icons8.com/ios-filled/100/ffffff/google-code.png',
        name:'WEB DEVELOPMENT',
        description:'Have hands-on experience creating UI development using React Js, Vue Js, Nuxt js, Microsoft Authentication, stripe payment gateway, kendo UI, Vuetify, Query Builder, Eye gaze tracking, Quasar, Tailwind CSS , Pinia, Vuex and Bootstrap To make the Creating Custom Component in React Js based on client requirements. Designed, developed, debugged, and modified code Determining operational feasibility by defining the problem, analyzing requirements, and assessing proposed solutions.'
    },
    {
        id:2,
        icon:'https://img.icons8.com/external-vectorslab-glyph-vectorslab/100/fffeee/external-Technical-Writing-mobile-app-development-vectorslab-glyph-vectorslab.png',
        name:'Technical Writing',
        description:'A technical writer may be writing for a specific industry, in which case the language tailors toward the education level of its audience. However, sometimes a technical writer is writing for a general audience. Many of the details provided by technical writers are complex, so the process of writing involves analyzing the information and presenting it in a way that easy for anyone reading it to understand, even someone who does not have a lot of experience with the topic'
    },
    {
        id:3,
        icon:'https://img.icons8.com/external-solid-design-circle/100/ffffff/external-Mobile-Development-digital-marketing-solid-design-circle.png',
        name:'Mobile Development',
        description:'The software can be preinstalled on the device, downloaded from a mobile app store or accessed through a mobile web browser. The programming and markup languages used for this kind of software development include Java, Swift, C# and HTML5 Mobile app development is rapidly growing. From retail, telecommunications and e-commerce to insurance, healthcare and government, organizations across industries must meet user expectations for real-time, convenient ways to conduct transactions and access information'
    },
    {
        id:4,
        icon:'https://img.icons8.com/ios-filled/100/ffffff/email-open.png',
        name:'WEB DEVELOPMENT',
        description:'Experienced in HTML5, CSS3, JavaScript, React Js, Vue Js, Quasar, Tailwind CSS, GIT, Jira, Bitbucket, Bootstrap, and Pinia Technologies. Depth understanding of VueJs, ReactJs, and Quasar Framework of Software Development Lifecycle.'
    },
    {
        id:5,
        icon:'https://img.icons8.com/ios-filled/100/ffffff/windows10-personalization.png',
        name:'Unit Testing',
        description:'Unit testing is the process of testing the smallest functional units of code, or "units", in a software application. A unit is usually a single function, method, procedure, module, or class.'
    },
    {
        id:6,
        icon:'https://img.icons8.com/ios-filled/100/ffffff/web-design.png',
        name:'Web Design',
        description:'It represents both functional and non-functional requirements in an organized manner to implement by developers to make a system. It usually consists of diagrams or models as visual aids representing the architecture and interactions between different building blocks in the system'
    },
    ])
</script>

