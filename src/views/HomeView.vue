<template>
    <div>
    <AboutComponent/>
    
    <section class="gallery">
        <div class="cards-wrapper">
            <CardComponent v-for="product in products" 
            v-bind:key="product.id" 
            v-bind:product="product" 
            />
        </div>
    </section>
    </div>
</template>
<script>
import AboutComponent from '@/components/AboutComponent.vue'
import CardComponent from '@/components/CardComponent.vue'

export default {
    components: {
        AboutComponent,
        CardComponent
    },
    data() {
        return {
            mainTitle: "Snaky Sneakers",
                subTitle: "Sneaker Reseller",
                products: [
                    {
                        id: 1,
                        title: 'Yeezy Boost 700',
                        price: 300,
                        imageLink: 'src/assets/images/gallery_1.jpg',
                        imageAlt: 'Image Yeezy Boost 700'
                    },
                    {
                        id: 2,
                        title: 'Air Jordan 4 Retro SE - Black Canvas',
                        price: 280,
                        imageLink: 'src/assets/images/gallery_2.jpg',
                        imageAlt: 'Image Air Jordan 4 Retro SE'
                    },
                    {
                        id: 3,
                        title: 'Wtaps X Authentic Syndicate - Wings',
                        price: 125,
                        imageLink: 'src/assets/images/gallery_3.jpg',
                        imageAlt: 'Image Wtaps X Authentic Syndicate'
                    },
                    {
                        id: 4,
                        title: 'Undefeated X Zoom Kobe 1 ProTro - White Gum',
                        price: 625,
                        imageLink: 'src/assets/images/gallery_4.jpg',
                        imageAlt: 'Image Undefeated X Zoom Kobe 1 ProTro'
                    },
                    {
                        id: 5,
                        title: 'Air Jordan 4 Retro - Red Thunder',
                        price: 360,
                        imageLink: 'src/assets/images/gallery_5.jpg',
                        imageAlt: 'Air Jordan 4 Retro'
                    },
                    {
                        id: 6,
                        title: 'Off-White X Air Force 1 Low - Brooklyn',
                        price: 1325,
                        imageLink: 'src/assets/images/gallery_6.jpg',
                        imageAlt: 'Off-White X Air Force 1 Low'
                    },
                ]
        }
    },
}
</script>
<style lang="scss">
    
</style>