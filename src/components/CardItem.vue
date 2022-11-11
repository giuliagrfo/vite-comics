<script>
export default {
    name: 'Card',
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="col gy-5">
        <img :src="image" :alt="title">
        <div class="title">
            <span>{{ title }}</span>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as*;

.title {
    text-transform: uppercase;
    margin-top: 1rem;
}
</style>