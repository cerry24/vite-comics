<script>
export default {

}
</script>
<template>
    <section id="content">
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
#content {
    background-color: black;
    padding: 3rem 0;

    .content-container {
        width: 70%;
        color: white;
        margin: 0 auto;
    }
}

#dc-universe {
    background-color: #0282f9;
    padding: 4rem 0;

    ul {
        display: flex;
        justify-content: space-between;
        width: 70%;
        list-style-type: none;
        color: white;
        margin: 0 auto;

        li {
            margin: 1rem;
        }
    }
}
</style>