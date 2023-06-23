<script>
export default {
    name: "AppSocialFooter"
}
</script>

<template>
    <div class="appSocialFooter">
        <div class="container">
                <div class="signup-button">
                    <a href="">SIGN-UP NOW!</a>
                </div>
                <div class="social-links">
                    <ul>
                        <li>
                            <a href="">
                                <p>FOLLOW US</p>
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/footer-facebook.png" alt="Facebook">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/footer-twitter.png" alt="Twitter">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/footer-youtube.png" alt="Youtube">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/footer-pinterest.png" alt="Pinterest">
                            </a>
                        </li>
                        <li>
                            <a href="">
                                <img src="../assets/footer-periscope.png" alt="Periscope">
                            </a>
                        </li>
                    </ul>
                </div>
        </div>
    </div>
</template>

<style scoped lang="scss">
.appSocialFooter {
    position: relative;
    display: flex;
    background-color: rgb(48, 48, 48);
    height: 80px;
    .container {
        display: flex;
        width: 800px;
        height: 100%;
        margin: 0 auto;
        .signup-button {
            display: flex;
            width: 50%;
            height: 100%;
            align-items: center;
            a {
                padding: 10px;
                border: 2px solid rgb(2, 130, 249);
                text-decoration: none;
                background: none;
                color: white;
                margin: 0;
            }
        }
        .social-links {
            display: flex;
            flex-wrap: nowrap;
            align-items: center;
            justify-content: end;
            width: 50%;
            height: 100%;
            ul {
                display: flex;
                gap: 3px;
                align-items: center;
                margin: 0;
                li {
                    list-style: none;
                    a {
                        text-decoration: none;
                        p {
                            color: rgb(2, 130, 249);
                            font-weight: bold;
                            padding-right: 1rem;
                        }
                        img {
                            width: 70%;
                        }
                    }
                }
            }
        }
    }
}
</style>