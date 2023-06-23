<script>
export default {
    name: "AppSubpages",
    data() {
        return {
            subpage: [
                {
                    text: "Digital Comics",
                    url: "#",
                    img: 'buy-comics-digital-comics.png'
                },
                {
                    text: "DC Merchandise",
                    url: "#",
                    img: 'buy-comics-merchandise.png'
                },
                {
                    text: "Subscription",
                    url: "#",
                    img: 'buy-comics-subscriptions.png'
                },
                {
                    text: "Comic Shop Locator",
                    url: "#",
                    img: 'buy-comics-shop-locator.png'
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                    img: 'buy-dc-power-visa.svg'
                }
            ]
        }
    },
    methods: {
        getImagePath(img) {
            return new URL(`../assets/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section class="subpages">
        <div class="container">
            <ul>
                <li v-for="element in subpage">
                    <a :href="getImagePath(element.img)">
                        <img :src="getImagePath(element.img)" alt="">
                        <p>{{ element.text }}</p>
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
$subpage-background: #0282F9;

.subpages {
    position: relative;
    z-index: 1;
    height: 120px;
    width: 100%;
    padding: 0 1rem;
    background-color: $subpage-background;
    color: white;

    .container {
        max-width: 800px;
        height: 100%;
        display: flex;
        align-items: center;

        ul {
            width: 100%;
            display: flex;
            margin: 0;
            padding: 0;

            li {
                width: 20%;
                list-style: none;

                a {
                    height: 100%;
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    gap: 0.7rem;
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: 400;
                    font-size: 0.65rem;
                    color: inherit;

                    img {
                        margin: unset;
                        max-width: 40px;
                        max-height: 40px;
                    }

                    p {
                        margin: unset;
                    }
                }
            }
        }
    }
}
</style>