<template>
    <section class="text-white mt-20" id="contact">
        <h2 class="text-4xl font-bold text-white text-left mb-4 px-4 xl:pl-16">Let's Connect</h2>
        <div class="grid md:grid-cols-2 gap-4 relative px-4 xl:px-16 mt-8" data-aos="zoom-in-up">
            <div>
                <p class="text-[#adb7be]">To build responsive and visually appealing web applications that enhance user experience and meet client needs effectively. I am focused on mastering front-end and back-end technologies to create robust and secure web solutions
                </p>
                <div class="col-lg-4 col-md-4 mb-lg-0 mt-5">
                    <div class="flex mb-10 items-center">
                        <div class="p-2"
                            style="background: #111a3e; width: 50px;height: 46px; display: flex;justify-content: center; border-radius: 50%;
                        overflow: hidden;border: 1px solid#111a3e;backdrop-filter: blur(9px);-webkit-backdrop-filter: blur(9px);">
                            <img src="https://img.icons8.com/metro/50/ffffff/new-post.png" alt="new-post" class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>Email</h4>
                            <p>ankitm.uidev@gmail.com</p>
                        </div>
                    </div>
                    <div class="flex mb-10 items-center">
                        <div class="p-2"
                            style="background: #111a3e; width: 50px;height: 46px; display: flex;justify-content: center; border-radius: 50%;
                        overflow: hidden;border: 1px solid#111a3e;backdrop-filter: blur(9px);-webkit-backdrop-filter: blur(9px);">
                            <img src="https://img.icons8.com/ios-filled/50/ffffff/phone.png" alt="phone" class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>Phone</h4>
                            <p>7674988775</p>
                        </div>
                    </div>
                    <div class="flex mb-10 items-center">
                        <div class="p-2"
                            style="background: #111a3e; width: 50px;height: 46px; display: flex;justify-content: center; border-radius: 50%;
                        overflow: hidden;border: 1px solid#111a3e;backdrop-filter: blur(9px);-webkit-backdrop-filter: blur(9px);">
                            <img src="https://img.icons8.com/ios-filled/50/ffffff/linkedin.png" alt="linkedin"
                                class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>LinkedIn</h4>
                            <p>https://www.linkedin.com/in/ankit-meena</p>
                        </div>
                    </div>
                </div>
            </div>
            <div
            style="background: #111a3e; width: 100%;height: 100%; border-radius: 20px;
            overflow: hidden;border: 1px solid #111a3e;backdrop-filter: blur(9px);-webkit-backdrop-filter: blur(9px);">
            <form class="flex flex-col p-2" data-aos="zoom-in-up" >
                <div class="mb-6 mt-5">
                    <FloatLabel>
            <InputText id="username" type="email" v-model="value" class="input"/>
            <label for="username">Email</label>
        </FloatLabel>
                   
                </div>
                <div class="mb-6 mt-5">
                    <FloatLabel>
            <InputText id="username" type="text" v-model="value" class="input"/>
            <label for="username">Subject</label>
        </FloatLabel>
                </div>
                <div class="mb-6 mt-5">
                    <FloatLabel>
                        <Textarea v-model="value" class="input" rows="5" cols="30" />
            <label for="username">Message</label>
        </FloatLabel>
                    <!-- <label for="message" class="text-white block mb-2 text-sm font-medium">Message</label> -->
                    
                </div>
                <Button label="Send Message" icon="pi pi-check" severity="warn"/>
            </form>
        </div>
        <div class="bg-gradient-to-tr opacity-25 from-[#570cac] to-primary blur-2xl h-20 w-80 z-0 absolute -top-1/2 -left-4 transform -translate-x-2/3 
        -translate-1/2
        "></div>
        </div>
    </section>
</template>
<script setup>

import InputText from 'primevue/inputtext';
import Button from 'primevue/button';
import Textarea from 'primevue/textarea';

import FloatLabel from 'primevue/floatlabel';


</script>
