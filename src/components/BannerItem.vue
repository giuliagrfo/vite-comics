<script>
export default {
    name: 'Banner',
    data() {
        return {
            itemsList: [
                {
                    image: 'buy-comics-digital-comics.png',
                    text: 'digital comics',
                },
                {
                    image: 'buy-comics-merchandise.png',
                    text: 'dc merchandise',
                },
                {
                    image: 'buy-comics-shop-locator.png',
                    text: 'subescription',
                },
                {
                    image: 'buy-comics-subscriptions.png',
                    text: 'comic shop locator',
                },
                {
                    image: 'buy-dc-power-visa.svg',
                    text: 'dc power visa',
                }
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}

</script>


<template>
    <nav class="banner">
        <div class="container">
            <a href="#" v-for="item in itemsList">
                <img :src="getImageUrl(item.image)" alt="">
                <span>{{ item.text }}</span>
            </a>
        </div>

    </nav>
</template>

