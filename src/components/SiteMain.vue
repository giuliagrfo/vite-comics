<script>
import CardsList from './CardsList.vue'
export default {
    name: 'SiteMain',
    components: {
        CardsList
    }
}


</script>

<template>
    <main id="site_main">
        <div class="jumbotron">
            <div class="jumbo-top">

            </div>
            <CardsList />


            <nav class="navbar">
                <div class="container">
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        Digital Comic
                    </a>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        DC Merchandise
                    </a>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        Subscription
                    </a>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        Comic Shop Locator
                    </a>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        DC Power Visa
                    </a>
                </div>

            </nav>
        </div>
    </main>

</template>