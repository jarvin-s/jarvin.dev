<template>
    <div class="target" v-motion-slide-visible-once-left>
        <section class="relative overflow-hidden text-black dark:text-white bg-zinc-100 dark:bg-zinc-800">
            <div class="relative z-10 pb-60 max-w-2xl w-full sm:ml-40">
                <main class="mt-10 mx-auto px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:px-8 xl:mt-28">
                    <h2 class="my-6 text-6xl font-bold text-center sm:text-left text-transparent bg-clip-text bg-gradient-to-l from-indigo-400 to-rose-700">
                        About me
                    </h2>
                    <p class="text-lg dark:text-white text-center sm:text-left">A software development student
                        on his journey to become a Frontend Developer. Currently building <span
                            class="text-transparent bg-clip-text bg-gradient-to-l from-yellow-300 to-pink-500">accessible</span>
                        and <span class="text-transparent bg-clip-text bg-gradient-to-l from-yellow-300 to-pink-500">user-friendly</span> apps, using modern frameworks such as
                        <a target="_blank" class="hover:font-bold underline decoration-sky-500 decoration-2"
                            href="https://tailwindcss.com/">TailwindCSS</a>,
                        <a target="_blank" class="hover:font-bold underline decoration-green-600 decoration-2"
                            href="https://vuejs.org/">Vue</a>/<a target="_blank"
                            class="hover:font-bold underline decoration-green-500 decoration-2"
                            href="https://nuxt.com">Nuxt</a>
                        and in the future I will be learning
                        <a target="_blank" class="hover:font-bold underline decoration-sky-400 decoration-2"
                            href="https://react.dev/">React</a>/<a target="_blank"
                            class="hover:font-bold underline decoration-stone-950 decoration-2"
                            href="https://nextjs.org/">Next.js</a>.
                    </p>
                </main>
            </div>
        </section>
    </div>
</template>

<script>

</script>

<style scoped>
.gradient-one {
    position: absolute;
    width: 40vw;
    height: 40vw;
    background: radial-gradient(rgba(228, 7, 180, 0.0533) 0%, transparent 60%)
}

.gradient-two {
    position: absolute;
    width: 1000px;
    height: 800px;
    background: radial-gradient(rgba(255, 41, 41, 0.055) 0%, transparent 60%);
    z-index: 1;
}

.gradient-three {
    position: absolute;
    width: 900px;
    height: 700px;
    margin-left: 500px;
    background: radial-gradient(rgba(0, 195, 255, 0.057) 0%, transparent 60%);
    z-index: 1;
}

/* .gradient-1 {
    background: linear-gradient(180deg, rgba(188, 165, 255, 0) 0%, #d10b9f 100%);
    filter: blur(123px);
}

.gradient-2 {
    background: linear-gradient(90deg, #8b0d0d 0%, #c9300a 100%);
    filter: blur(500px);
}

.gradient-3 {
    background: rgba(62, 206, 231, 0.6);
    filter: blur(400px);
} */
</style>
