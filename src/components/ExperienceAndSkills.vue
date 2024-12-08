<template>
    <section class="text-white mt-18" id="skills">
        <div class="absolute right-0 top-[110rem] h-full w-full justify-end">
            <span class="flex opacity-20">
                <span class="w-16 h-32 rounded-l-full flex bg-primary blur-2xl"></span>
                <span class="w-16 h-32 rounded-r-full flex bg-[#f88fc2] blur-2xl mt-14"></span>
            </span>
        </div>
        <div class="md:grid md:grid-cols-2 gap-2 items-center py-8 px-4 xl:gap-16 xl:px-16">
            <div class="mt-4 md:mt-0 text-left flex flex-col  h-full w-[100%]">
                <h2 class="text-4xl font-bold text-white text-left mb-4">My 
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">Skills</span>
                </h2>
                <div class="grid md:grid-cols-4 sm:grid-cols-2 p-2.5 mt-8 gap-2 w-full">
                    <div class=""  v-for="skill in Skills" :key="skill.id">
                        <Button :label="skill.name" icon="pi pi-check" severity="warn" rounded iconPos="right"/>
                    </div> 
                </div>
               
              
            </div>
            <div data-aos="flip-left">
                <h2 class="text-4xl font-bold text-white text-left  md:text-center md:mt-0">My Experiences</h2>
                 <div class="space-y-8 py-8" data-aos="fade-left">
                    <div v-for="element in Experinces" :key="element.id"
                    class="flex  items-center rounded-xl p-4 bg-[#111a3e] shadow-lg border border-[#1f1641]"
                    >
                    <div class="w-1/4">
                        <img src="https://img.icons8.com/ios-filled/100/ffffff/lawyer.png" alt="lawyer">
                    </div>
                    <div class="w-3/4 pl-4">
                        <h3 class="text-2xl font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">
                            {{ element.role }}
                        </h3>
                        <p class="text-white">{{ element.company }}</p>
                        <p class="text-white">{{ element.date }}</p>
                    </div>
                </div>
                </div> 
          
            </div>
        </div>
    </section>
</template>
<script setup>
import { ref } from 'vue';
import Button from 'primevue/button';
const Skills =ref([
    {
        id:1,
        name:'HTmL & CSS',
        width:'85%'
    },
   
    {
        id:3,
        name:'JavaScript',
        width:'98%'
    },
    {
        id:4,
        name:'Vue js',
        width:'91%'
    },
    {
        id:5,
        name:'React js',
        width:'70%'
    },
    {
        id:5,
        name:'Vuex',
        width:'70%'
    },
    {
        id:5,
        name:'Pinia',
        width:'70%'
    },
    // {
    //     id:5,
    //     name:'Payment GateWay',
    //     width:'70%'
    // },
    {
        id:'6',
        name:"Axios"
    },
    {
        id:'7',
        name:'Saas'
    },
    {
        id:'8',
        name:'Nuxt Js'
    },
    {
        id:'9',
        name:"Vuetify"
    },
    {
        id:'10',
        name:"Redux"
    },
    {
        id:'11',
        name:"Prime Vue"
    },
    {
        id:'12',
        name:"Node js"
    },
    {
        id:'13',
        name:"Express js"
    },
    {
        id:'14',
        name:"Tailwind css"
    },
    {
        id:'15',
        name:"Quasar"
    },
    {
        id:'16',
        name:"Bootstrap"
    },
    {
        id:'17',
        name:"Github"
    },
    {
        id:'18',
        name:"Bitbucket"
    },
    {
        id:'19',
        name:"Authentication"
    },
    {
        id:'20',
        name:"Mongo DB"
    },
    {
        id:'21',
        name:"Kendo Ui"
    },
   
    // AxiosSassReduxVue CliVuexNuxtjsVuetifyVue.jsReact.jsCSSHTMLJavascript
]);

const Experinces =ref([
    {
        id:1,
        role:'Web Developer',
        company:'Dollop Infotech Pvt Ltd',
        date:'Oct 2020 - Mar 2021'
    },
    {
        id:2,
        role:'Web Developer',
        company:'Dollop Infotech Pvt Ltd',
        date:'Apr 2021 - Dec 2022'
    },
    {
        id:3,
        role:'Web Developer',
        company:'Coding Age Pvt Ltd',
        date:'Jan 2023 - Mar 2023'
    },
    {
        id:3,
        role:'Web Developer',
        company:'Chetu India Pvt Ltd',
        date:'Mar 2023 -  Present'
    },
])
</script>
