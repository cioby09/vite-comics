<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "Character",
                    url: "#",
                    current: false
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "Games",
                    url: "#",
                    current: false
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false
                },
                {
                    text: "News",
                    url: "#",
                    current: false
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <a href="/">
                    <img src="../assets/dc-logo.png" alt="">
                </a>
            </div>
            <nav class="nav-bar">
                <ul>
                    <li v-for="link in links" :class="link.current ? 'active' : ''">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
$header-text: #464646;

header {
    height: 100px;
    width: 100%;
    padding: 0 1rem;
    background-color: white;

    .container {
        height: 100%;
        max-width: 800px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
            margin: 0;

            img {
                height: 60px;
            }
        }

        .nav-bar {
            margin: 0;
            line-height: 100px;

            ul {
                display: flex;
                gap: 1rem;

                li {
                    display: flex;
                    list-style: none;

                    &.active,
                    &:hover {
                        border-bottom: 3px solid #0282F9;
                        height: 100px;
                    }

                    a {
                        text-decoration: none;
                        font-weight: 700;
                        font-size: 0.6rem;
                        text-transform: uppercase;
                        color: $header-text;
                    }
                }
            }
        }
    }
}
</style>