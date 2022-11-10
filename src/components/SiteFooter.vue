<script>
export default {
    name: 'SiteFooter',
    data() {
        return {
            dc_comics: [
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
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                }

            ],
            shop: [
                {
                    text: 'Shop DC',
                    href: '#',
                },
                {
                    text: 'Shop DC Collectibles',
                    href: '#',
                }
            ],
            dc: [
                {
                    text: 'Terms Of Use',
                    href: '#'
                },
                {
                    text: 'Privacy Policy',
                    href: '#'
                },
                {
                    text: 'Ad Choices',
                    href: '#'
                },
                {
                    text: 'Advertising',
                    href: '#'
                },
                {
                    text: 'Jobs',
                    href: '#'
                },
                {
                    text: 'Subscriptions',
                    href: '#'
                },
                {
                    text: 'Talent Workshops',
                    href: '#'
                },
                {
                    text: 'CPSC Certificates',
                    href: '#'
                },
                {
                    text: 'Ratings',
                    href: '#'
                },
                {
                    text: 'Shop Help',
                    href: '#'
                },
                {
                    text: 'Contact Us',
                    href: '#'
                }
            ],
            sites: [
                {
                    text: 'DC',
                    href: '#'
                },
                {
                    text: 'MAD Magazine',
                    href: '#'
                },
                {
                    text: 'DC Kids',
                    href: '#'
                },
                {
                    text: 'DC Universe',
                    href: '#'
                },
                {
                    text: 'DC Power Visa',
                    href: '#'
                }
            ]
        }
    }

}


</script>

<template>
    <footer id="site_footer">

        <div class="container">
            <div class="row">
                <div class="col links">
                    <div class="row">
                        <div class="col dc_comics gy-5">
                            <h3>Dc Comics</h3>
                            <ul>
                                <li v-for="item in dc_comics">
                                    <a :href="item.href">
                                        {{ item.text }}
                                    </a>
                                </li>
                            </ul>
                            <div class="row">
                                <div class="col shop">
                                    <h3>Shop</h3>
                                    <ul>
                                        <li v-for="item in shop">
                                            <a :href="item.href">{{ item.text }}</a>
                                        </li>
                                    </ul>
                                </div>
                            </div>
                        </div>
                        <div class="col dc gy-5">
                            <h3>Dc</h3>
                            <ul>
                                <li v-for="item in dc">
                                    <a :href="item.href">
                                        {{ item.text }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="col sites gy-5">
                            <h3>Sites</h3>
                            <ul>
                                <li v-for="item in sites">
                                    <a :href="item.href">
                                        {{ item.text }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="col ft_logo">
                </div>
            </div>
        </div>


        <div class="call_to_action">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div class="sign_up">
                            <a href="#">Sign-Up Now!</a>
                        </div>
                    </div>
                    <div class="col">
                        <div class="social">
                            <h3>Follow Us</h3>
                            <img src="../assets/img/footer-facebook.png" alt="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </div>

                    </div>
                </div>

            </div>

        </div>


    </footer>
</template>