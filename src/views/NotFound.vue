<template>
    <div class="wrapper">
        <div class="wrapper-overlay">
            <div class="content-container">
                <div class="text">
                    <h1>404</h1>
                    <h3>Die angegebene Seite wurde leider nicht gefunden D:</h3>
                    <h3>Hier sind ein paar Vorschläge!</h3>
                    <div class="pt-3 row">
                        <a class="col center social-icon" href="mailto:hcgoper@carossa-gymnasium.de"><i class="fa fa-envelope"></i></a>
                            <button class="col center home-btn btn enter-button-outline" type="button" id="newsletter-enter" @click="returnToHome">
                                <span class="btn-text">Startseite</span>
                            </button>
                        <a class="col center social-icon" href="#"><i class="fa-brands fa-instagram"></i></a>      
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PageNotFound',
    methods: {
        returnToHome() {
            window.location.href = "/";
        }
    }
}
</script>

<style scoped>
.wrapper {
    position: relative;
    overflow: hidden;
    position: absolute;
    height: 100vh;
    width: 100%;
    background-image: linear-gradient(to right bottom, #0744ef, #0075ff, #0094f1, #00aad4, #2bbcbc);
    background-position: left;
    background-repeat: no-repeat;
    background-size: cover;
    top: 0;
    padding: auto;
}

.row {
    margin-bottom: 20px;
}
.text {
    display: inline-block;
    font-family: "Oswald",sans-serif;
    color: white;
}

.text > div > a {
    color: white;
    font-size: 50px;
    text-decoration: none;
}

.text > h1 {
    font-weight: 700;
    font-size: 200px;
    text-shadow: 0px 10px 0px rgba(150, 150, 150, 1);
}
.content-container {
    padding: 7%;
    text-align: center;
}

.rocket-img {
    width: 200px;
    float: right;
}

.btn-text {
    z-index: 1;
}

.btn:hover {
    color: #00a1e0;
}

.btn {
    position: relative;
    border-radius: 0% !important;
    width: 175px;
    height: 50px;
    border-width: 3px;
    border-color: white;
    color: white;

    font-family: 'Oswald', sans-serif;
    font-size: 1.5rem;
}

.btn:after {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #ffffff;
    transition: all 0.40s;
}

.btn:hover:after {
    width: 100%;
}
</style>