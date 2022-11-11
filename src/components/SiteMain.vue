<script>
import CardsList from './CardsList.vue';
import Banner from './BannerItem.vue';

export default {
    name: 'SiteMain',
    components: {
        CardsList,
        Banner
    }
}


</script>

<template>
    <main id="site_main">
        <div class="jumbotron">
            <div class="jumbo-top">

            </div>
            <CardsList />

            <Banner />

        </div>
    </main>

</template>