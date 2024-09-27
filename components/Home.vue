<template>
    <div>

        <Head>
            <link rel="stylesheet"
                href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
            <link rel="stylesheet" href="../magic-master/dist/magic.css">
        </Head>

        <article class="grid mt-8 h-[100vh] grid-cols-1 place-items-center md:grid-cols-2  home-div " dir="rtl">


            <section class="section ">
                <section class="w-96 h-72 rounded-full section__title">

                    <img class="rounded-full" src="/pic.jpg" />
                </section>


            </section>
            <section class=" w-96 text-center mt-14 leading-7  " dir="ltr">
                <section class=" mb-4 font-bold  text-4xl tracking-wide ">

                    <h1>mahdi amrollahi 👋</h1>

                </section>
                <section class=" mb-12 ">

                    <h1 class="home-h3-section text-3xl mb-4 text-center">visual designer</h1>
                    <p class="text-xl text-gray-500">i'm creative designer based in tehran and i'm
                        very passianate and dedicated to
                        my work...</p>
                </section>
                <p
                    class="border-2  cursor-pointer rounded-full mx-10  text-xl flex justify-center 	bg-slate-950 text-neutral-400 px-10 py-6  hover:text-black hover:bg-white hover:text-3xl transition-all ease-linear duration-150">
                    Hello
                </p>


            </section>
            <section class="hidden lg:flex text-2xl text-black flex-col align-middle gap-6  ">

                <i class="fa fa-instagram"></i>
                <i class="fa fa-github"></i>
                <i class="fa fa-twitter"></i>


            </section>

        </article>
    </div>
</template>

<script  setup>

</script>
<style scoped>
img {
    object-fit: contain;
}

@media (min-width: 1024px) {
    .home-div {
        grid-template-columns: 1fr 3fr auto;
        margin: 0 10rem;
    }
}



/* h1 {
    font-size: 30px;
    margin: 0;
    background-image: url(../img/about.jpg);
    background-size: cover;
    background-clip: text;
    color: transparent;
} */
</style>