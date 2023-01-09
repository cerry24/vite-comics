<script>
export default {

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
                        <li>oggetto</li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                    </ul>
                    <ul>
                        <li>
                            <h4>shop</h4>
                        </li>
                        <li>oggetto</li>
                        <li>oggetto</li>
                    </ul>
                </div>

                <ul>
                    <li>
                        <h4>dc</h4>
                    </li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                </ul>

                <ul>
                    <li>
                        <h4>sites</h4>
                    </li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                    <li>oggetto</li>
                </ul>
            </div>

            <div class="logo-big">
                <img src="../assets/img/dc-logo-bg.png" alt="Big logo Dc">
            </div>
        </div>
    </section>
</template>

<style lang="scss">
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
            color: gray;
        }
    }
}


h4 {
    text-transform: uppercase;
    margin-bottom: 0.8rem;
    font-size: 1rem;
    color: white;
}

.logo-big {
    position: relative;

    img {
        position: absolute;
        right: 0;
        top: -100px;
    }
}
</style>