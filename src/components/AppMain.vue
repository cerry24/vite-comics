<script>
import MainJumbotron from './AppMain_components/MainJumbotron.vue';

export default {
    components: {
        MainJumbotron
    }
}
</script>

<template>
    <MainJumbotron />

    <section id="current-series">
        <div class="content-container">
            <h3>--> Content goes here</h3>
        </div>
    </section>

    <section id="dc-universe">
        <ul>
            <li>oggetto</li>
            <li>oggetto</li>
            <li>oggetto</li>
            <li>oggetto</li>
            <li>oggetto</li>
        </ul>
    </section>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;

#current-series {
    background-color: $black-bg-color;
    padding: 3rem 0;

    .content-container {
        width: 70%;
        color: $white-color;
        margin: 0 auto;
    }
}

#dc-universe {
    background-color: $main-color;
    padding: 4rem 0;

    ul {
        display: flex;
        justify-content: space-between;
        width: 70%;
        list-style-type: none;
        color: $white-color;
        margin: 0 auto;

        li {
            margin: 1rem;
        }
    }
}
</style>