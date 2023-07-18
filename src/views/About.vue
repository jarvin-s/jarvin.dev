<template>
    <div class="target" v-motion-slide-visible-once-left>
        <section class="about bg-zinc-100 dark:bg-zinc-800">
            <div class="hero-main flex flex-col mr-40 pb-80">
                <div class="flex flex-col md:flex-row justify-end">
                    <!-- <div class="absolute z-0 w-[90%] h-[35%] top-0 gradient-1"></div>
                        <div class="absolute z-0 w-[80%] h-[80%] rounded-full bottom-40 gradient-2"></div>
                        <div class="absolute z-0 w-[80%] h-[50%] right-20 bottom-20 gradient-3"></div> -->
                    <div class="gradient-one"></div>
                    <h1 class="w-1/3 font-bold dark:text-white text-6xl text-center sm:text-right">
                        About me</h1>
                    <p class="flex flex-col md:flex-row justify-end">test</p>
                </div>
                <div class="scroll-parent flex flex-col md:flex-row">
                    <div class="scroll-element primary justify-end">
                        <img class="w-10" src="/languages/HTML.svg" />
                        <img class="w-10" src="/languages/CSS.svg" />
                        <img class="w-10" src="/languages/JavaScript.svg" />
                        <img class="w-10" src="/languages/Vue.svg" />
                        <img class="w-10" src="/languages/tailwind.svg" />
                        <img class="w-10" src="/languages/git.svg" />
                        <img class="w-10" src="/languages/mysql.svg" />
                    </div>
                    <div class="scroll-element secondary">
                        <img class="w-10" src="/languages/HTML.svg" />
                        <img class="w-10" src="/languages/CSS.svg" />
                        <img class="w-10" src="/languages/JavaScript.svg" />
                        <img class="w-10" src="/languages/Vue.svg" />
                        <img class="w-10" src="/languages/tailwind.svg" />
                        <img class="w-10" src="/languages/git.svg" />
                        <img class="w-10" src="/languages/mysql.svg" />
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>

</script>

<style scoped>
.scroll-container {
    display: flex;
    flex-direction: row;
    align-items: center;
    overflow: hidden;
    margin-top: 2rem;
}

.scroll-parent {
    position: absolute;
    width: 28.3vw;
    height: 20rem;
    padding: 2rem 0;
    overflow-x: hidden;
}

.scroll-element {
    width: inherit;
    height: inherit;
    position: absolute;
    right: 0%;
    top: 0%;
    animation: primary 12s linear infinite;
    display: flex;
    align-items: center;
    justify-content: space-around;
}

.scroll-element img {
    width: 6%;
}

.primary {
    animation: primary 12s linear infinite;
}

.secondary {
    animation: secondary 12s linear infinite;
}

@keyframes primary {
    from {
        right: 0%;
    }

    to {
        right: -100%;
    }
}

@keyframes secondary {
    from {
        right: 100%;
    }

    to {
        right: 0%;
    }
}

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
