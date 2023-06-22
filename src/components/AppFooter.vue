<script>
export default {
    name: "AppFooter",
    data() {
        return {
            ComicLink: ["Character", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            ShopLink: ["Shod DC", "Shop DC Collectilbles"],
            DCLink: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            SitesLink:["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]

        }
    }
}
</script>

<template>
    <section class="appFooter">
        <div class="container">
            <div class="footer-links">
                <div class="list">
                    <h4 class="list-title">DC COMICS</h4>
                    <ul v-for="(element, index) in ComicLink">
                        <li>{{ element }}</li>
                    </ul>
                    <h4 class="list-title">SHOP</h4>
                    <ul v-for="(element, index) in ShopLink">
                        <li>{{ element }}</li>
                    </ul>
                </div>
                <div class="list">
                    <h4 class="list-title">DC</h4>
                    <ul v-for="(element, index) in DCLink">
                        <li>{{ element }}</li>
                    </ul>
                </div>
                <div class="list">
                    <h4 class="list-title">SITES</h4>
                    <ul v-for="(element, index) in SitesLink">
                        <li>{{ element }}</li>
                    </ul>
                </div>
            </div>
            <div class="footer-logo-container flex">
                <img class="footer-logo" src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.appFooter {
    background-image: url(../assets/footer-bg.jpg);
    .container {
        max-width: 800px;
        margin: 0 auto;
        display: flex;
        .footer-links {
            display: flex;
            width: 50%;
            margin: 0;
            .list {
                margin-right: 1.5rem;
                margin-left: 0;
                margin-top: 1.5rem;
                margin-bottom: 2rem;
                .list-title {
                    padding: 0.5rem 0;
                    color: white;
                }
                ul {
                    padding-left: 0;
                    li {
                        font-size: 0.6rem;
                        color: rgba(164, 164, 164, 0.658);
                        list-style: none;
                        padding: 0.1rem 0;
                    }
                }
            }
        }
    }
    .footer-logo-container {
        width: 50%;
        justify-content: center;
        position: relative;
        .footer-logo {
            top: -75px;
            position: absolute;
            transform: scale(0.9);
        }

    }
}
</style>