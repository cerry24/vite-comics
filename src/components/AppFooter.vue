<script>
export default {
    data() {
        return {
            dcComicsList: [
                {
                    text: "Characters",
                    url: "#"
                },
                {
                    text: "Comics",
                    url: "#"
                },
                {
                    text: "Movies",
                    url: "#"
                },
                {
                    text: "Tv",
                    url: "#"
                },
                {
                    text: "Games",
                    url: "#"
                },
                {
                    text: "Videos",
                    url: "#"
                },
                {
                    text: "News",
                    url: "#"
                }
            ],

            shopList: [
                {
                    text: "Shop DC",
                    url: "#"
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#"
                }
            ],

            dcList: [
                {
                    text: "Terms Of Use",
                    url: "#"
                },
                {
                    text: "Privacy policy (New)",
                    url: "#"
                },
                {
                    text: "Ad Choices",
                    url: "#"
                },
                {
                    text: "Advertising",
                    url: "#"
                },
                {
                    text: "Jobs",
                    url: "#"
                },
                {
                    text: "Subscriptions",
                    url: "#"
                },
                {
                    text: "Talent Workshops",
                    url: "#"
                },
                {
                    text: "CPSC Certificates",
                    url: "#"
                },
                {
                    text: "Ratings",
                    url: "#"
                },
                {
                    text: "Shop Help",
                    url: "#"
                },
                {
                    text: "Contact Us",
                    url: "#"
                }
            ],

            sitesList: [
                {
                    text: "DC",
                    url: "#"
                },
                {
                    text: "MAD Magazine",
                    url: "#"
                },
                {
                    text: "DC Kids",
                    url: "#"
                },
                {
                    text: "DC Universe",
                    url: "#"
                },
                {
                    text: "DC Power Visa",
                    url: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <section id="upper-footer">
        <div class="footer-container">
            <div class="footer-nav">
                <div class="queueing-lists">
                    <ul>
                        <li>
                            <h4>dc comics</h4>
                        </li>
                        <li v-for="dcComicsListItem in dcComicsList">
                            <a :href="dcComicsListItem.url">{{ dcComicsListItem.text }}</a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <h4>shop</h4>
                        </li>
                        <li v-for="shopListItem in shopList">
                            <a :href="shopListItem.url">{{ shopListItem.text }}</a>
                        </li>
                    </ul>
                </div>

                <ul>
                    <li>
                        <h4>dc</h4>
                    </li>
                    <li v-for="dcListItem in dcList">
                        <a :href="dcListItem.url">{{ dcListItem.text }}</a>
                    </li>
                </ul>

                <ul>
                    <li>
                        <h4>sites</h4>
                    </li>
                    <li v-for="sitesListItem in sitesList">
                        <a :href="sitesListItem.url">{{ sitesListItem.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="logo-big">
                <img src="../assets/img/dc-logo-bg.png" alt="Big logo Dc">
            </div>
        </div>
    </section>

    <section id="lower-footer">
        <div class="footer-container">
            <div class="sign-up-btn">
                <h4>Sign-up Now!</h4>
            </div>
            <div class="social-icons">
                <h3>Follow Us</h3>
                <ul class="icons">
                    <li>
                        <img src="../assets/img/footer-facebook.png" alt="Facebook logo">
                    </li>
                    <li>
                        <img src="../assets/img/footer-twitter.png" alt="Twitter logo">
                    </li>
                    <li>
                        <img src="../assets/img/footer-youtube.png" alt="Youtube logo">
                    </li>
                    <li>
                        <img src="../assets/img/footer-pinterest.png" alt="Pinterest logo">
                    </li>
                    <li>
                        <img src="../assets/img/footer-periscope.png" alt="Periscope logo">
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;

#upper-footer {
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    justify-content: space-between;
    overflow: hidden;
}

.footer-container {
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
}

.footer-nav {
    display: flex;
    margin: 3rem 0;

    ul {
        list-style-type: none;
        margin-right: 2rem;
        margin-bottom: 1rem;

        li {
            font-size: 0.9rem;
            line-height: 1.4rem;

            a {
                color: gray;
            }
        }
    }
}


h4 {
    text-transform: uppercase;
    margin-bottom: 0.8rem;
    font-size: 1rem;
    color: $white-color;
}

.logo-big {
    position: relative;

    img {
        position: absolute;
        right: 0;
        top: -100px;
    }
}

#lower-footer {
    background-color: $dark-gray-bg-color;
    padding: 1.5rem 0;

    .sign-up-btn {
        border: 2px solid $main-color;
        padding: 1rem;

        h4 {
            margin: 0;
        }
    }

    .social-icons {
        display: flex;
        align-items: center;

        h3 {
            color: $main-color;
            text-transform: uppercase;
        }

        ul {
            list-style-type: none;
            margin-left: 1.5rem;

            li {
                display: inline-block;
                padding-right: 1.5rem;
            }
        }
    }
}
</style>