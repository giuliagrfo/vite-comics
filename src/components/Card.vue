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
        <h4>{{ title }}</h4>
    </div>
</template>