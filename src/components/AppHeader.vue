<script>
export default {
    data() {
        return {
            mainNav: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <div class="header-container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="Dc small logo">
        </div>
        <nav>
            <ul>
                <li v-for="navItem in mainNav">
                    <a :href="navItem.url" :class="(navItem.current) ? 'active' : ''">{{ navItem.text }}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;

.header-container {
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    padding: 0.8rem 0;

    img {
        width: 75%;
    }
}

nav ul {
    list-style-type: none;

    li {
        display: inline-block;
        text-transform: uppercase;
        font-weight: 700;
        font-size: 0.9rem;
        padding: 0 0.8rem;
    }
}

a {
    text-decoration: none;
    color: black;

    &.active {
        color: $main-color;
    }
}
</style>