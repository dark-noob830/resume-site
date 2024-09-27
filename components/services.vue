<template>
    <div>

        <Head>
            <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
        </Head>
        <article class="services_title">
            <h1>Services</h1>
            <p>what i offer</p>
        </article>
        <article class="services-body">
            <section class="services-card">
                <i class="material-icons " style="font-size: 2rem;">
                    space_dashboard
                </i>
                <h1>web Designer</h1>
            </section>
            <section class="services-card">
                <i class="material-icons " style="font-size: 2rem;">
                    code
                </i>
                <h1>coding project</h1>
            </section>

        </article>
    </div>
</template>

<script setup>

</script>

<style  scoped>
.services_title {
    text-align: center;
    margin-top: 5rem;
    font-size: 1.25rem;
}

.services_title h1 {
    font-size: 3rem;
    font-weight: bold;
}

.services-body {
    width: 70vw;
    margin: 0 auto;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(384px, 1fr));
    place-items: center;
}

.services-card {
    margin-top: 2rem;
    padding: 2rem;
    padding-top: 5rem;
    border: 1px solid black;
    border-radius: 3rem;
    font-size: 2rem;
}
</style>