<template>
    <div class="about">

        <Head>
            <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
        </Head>
        <article class="about_title">
            <h1>About Me</h1>
            <p>My introduction</p>
        </article>
        <article class="about_body">
            <section class='about_img'>
                <img src="/pic.jpg" alt="">
            </section>
            <section class="about_desc">
                <article class="btn_head">
                    <div class="little-card">
                        <span class="material-icons">
                            workspace_premium
                        </span>
                        <h2>Experience</h2>
                        <p>1 + Years</p>
                    </div>
                    <div class="little-card">
                        <span class="material-icons">
                            cases
                        </span>
                        <h2>Completed</h2>
                        <p>10 + Projects</p>
                    </div>
                    <div class="little-card">
                        <span class="material-icons">
                            support_agent
                        </span>
                        <h2>Support</h2>
                        <p>Online 24/7</p>
                    </div>
                </article>
                <article class="about_text">
                    <p>Frontend developer, I create web pages with UI / UX user interface, I have years of experience and
                        many clients are happy with the projects carried out.</p>
                </article>
                <button class="btn_cv">download CV</button>
            </section>
        </article>


    </div>
</template>

<script setup>

</script>

<style scoped>
.about {
    height: auto;
}

.about_title {
    margin-top: 20rem;
    text-align: center;
    font-size: 1.5rem;
}

.about_title h1 {
    font-size: 4rem;
    font-weight: bold;
}

.about_body {
    margin-top: 2rem;
}

.about_img {
    display: grid;
    justify-items: center;
}

.about_img img {
    width: 400px;
    height: 400px;
    margin: 2rem auto;
    border-radius: 2rem;
}

.about_desc {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;

}

.btn_head {
    margin-top: 2rem;
    display: grid;
    width: 40rem;
    grid-template-columns: repeat(3, 1fr);
    justify-items: center;
}

.little-card {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    padding: 2rem;
    box-shadow: -1px 15px 38px -12px rgba(0, 0, 0, 0.45);
    border-radius: 20px;
    gap: 1rem;
}

.little-card:hover {
    box-shadow: -1px 15px 38px -4px rgba(0, 0, 0, 0.67);
}

.about_text {
    margin-top: 3rem;
    font-size: 1.25rem;
    width: 37rem;
    padding-left: 2rem;
}

.btn_cv {
    background: black;
    color: white;
    margin-top: 3rem;
    border-radius: 3rem;
    width: 17rem;
    padding: 2rem 3rem;
}

@media (min-width: 768px) {


    .about_body {
        display: grid;
        grid-template-columns: 1fr 1fr;
        place-items: center;
    }

    .about_title {
        margin-top: 2rem;
        text-align: center;
        font-size: 1.5rem;
    }
}
</style>