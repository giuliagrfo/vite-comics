<script>
import Card from "./CardItem.vue";
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
        <div class="current_series">
            <h2>Current Series</h2>
        </div>
        <div class="container">

            <div class="cards row row-cols-6">
                <Card v-for="item in comics" :image="item.thumb" :title="item.series" />
            </div>
        </div>
        <div class="load">
            <a href="#">Load More</a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as*;

.content {
    position: relative;

    .current_series {
        position: absolute;
        bottom: 95%;
        left: 10%;
        padding: 1rem 2.5rem;
        background-color: $secondary;
        text-transform: uppercase;
    }

    .load {
        text-align: center;
        margin-top: 3rem;
        margin-bottom: 1rem;

        a {
            background-color: $secondary;
            padding: 0.5rem 3rem;
            font-size: 13px;
            font-weight: bold;
            text-transform: uppercase;
            text-decoration: none;
            color: white;

            &:hover {
                background-color: transparent;
                border: 2px solid $secondary;

            }
        }
    }
}
</style>