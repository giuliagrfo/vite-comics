<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            menu: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'Tv',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                }
            ]
        }
    }
}


</script>

<template>
    <div class="container">
        <header id="site_header">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav class="navbar">
                <a :href="item.href" v-for="item in menu" :class="item.text === 'Comics' ? 'active' : ''">
                    {{ item.text }}
                </a>

            </nav>


        </header>
    </div>

</template>