<script>
export default {

}
</script>
<template>
    <div class="header-container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="Dc small logo">
        </div>
        <nav>
            <ul>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
                <li><a href="#">oggetto</a></li>
            </ul>
        </nav>
    </div>
</template>

<style lang="scss">
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
}
</style>