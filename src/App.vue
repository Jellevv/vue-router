<script>
    import NavComponent from '@/components/NavComponent.vue'
    import HeaderComponent from '@/components/HeaderComponent.vue'
    import FooterComponent from '@/components/FooterComponent.vue'

import router from './router'
    
    export default {
        data() {
            return {
                
            }
        },
        components: {
            NavComponent,
            HeaderComponent,
            FooterComponent,
        }
    }
</script>

<template>
    <NavComponent/>
    <HeaderComponent
        :mainTitle="mainTitle" 
        :subTitle="subTitle"
    />
    <router-view> </router-view>

    <FooterComponent
        :mainTitle="mainTitle" 
        :subTitle="subTitle"
    />
</template>