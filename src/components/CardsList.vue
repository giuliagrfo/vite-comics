<script>
import Card from "./Card.vue";
import comics from "../data/comics.js";

export default {
    components: {
        Card
    },
    data() {
        return {
            comics: comics
        }
    }
}
</script>

<template>
    <div class="content">
        <div class="container">
            <div class="cards row row-cols-6">
                <Card v-for="item in comics" :image="item.thumb" :title="item.series" />
            </div>
        </div>
    </div>
</template>