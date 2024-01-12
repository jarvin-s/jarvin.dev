<template>
    <div class="target" ref="targetEl" v-motion-roll-bottom>
        <section id="home" class="hero bg-zinc-100 dark:bg-zinc-800">
            <div class="content py-6 items-center gap-x-12 pb-40">
                <div class="hero-main w-1/3 m-40 h-80 flex justify-center items-center flex-col md:flex-row relative">
                    <div class="absolute z-0 w-[90%] h-[35%] top-0 gradient-1"></div>
                    <div class="absolute z-0 w-[80%] h-[80%] rounded-full bottom-40 gradient-2"></div>
                    <div class="hero-text absolute flex flex-col text-center md:text-left">
                        <h1 class="text-2xl font-bold text-pink-700">Hi, my name
                            is
                        </h1>
                        <h1 class="text-6xl font-bold dark:text-slate-100 text-center md:text-left">Jarvin
                            Siegers</h1>
                        <h1 class="text-3xl text-center md:text-left dark:text-white opacity-60">Software
                            Developer
                        </h1>
                        <div class="flex flex-row justify-center md:justify-start items-center mt-6">
                            <button
                                class="btn-send cursor-pointer flex py-2 px-4 font-bold rounded-lg focus:outline-none focus:shadow-outline">
                                <RouterLink to="#home" v-scroll-to="'#contact'">
                                    Get in touch
                                </RouterLink>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
import { RouterLink } from 'vue-router'
import { useMotion } from '@vueuse/motion'
import { ref } from 'vue'
const targetEl = ref()

useMotion(targetEl, {
    enter: {
        transition: {
            duration: 2000,
        }
    }
});
</script>

<style scoped>
@tailwind utilities;

@layer utilities {
    .btn-send {
        border: solid 3px transparent;
        background-image: linear-gradient(60deg, rgb(172, 9, 109), rgb(179, 23, 12));
        background-origin: border-box;
        color: white;
        transition: 300ms;
        box-shadow: none;
        transition: all 800ms;
    }

    .btn-send:hover {
        -webkit-box-shadow: 0px 0px 54px 0px rgba(189, 32, 189, 1);
        -moz-box-shadow: 0px 0px 54px 0px rgba(189, 32, 189, 1);
        box-shadow: 0px 0px 54px 0px rgb(172, 9, 109), rgb(179, 23, 12) 0px 0px 32px 0px;
    }
}

/* .hero-img {
    -webkit-animation: morph 6s ease-in-out infinite;
    animation: morph 6s ease-in-out infinite;
    transition: all 1s ease-in-out;
    width: 20rem;
    height: 20rem;
    background-position: 50%;
    background-size: contain;
    background-repeat: no-repeat;
    background-image: url("/jarvin.png");
    max-width: 300px;
}

.hero-text {
    display: flex;
    flex-direction: column;
    max-width: 50rem;
    position: relative;
} */

@keyframes morph {
    0% {
        border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
    }

    50% {
        border-radius: 30% 70% 60% 40%/70% 60% 40% 30%;
    }

    100% {
        border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
    }

}

/* Gradients */
.gradient-1 {
    background: linear-gradient(180deg, rgba(188, 165, 255, 0) 0%, #d60baa 100%);
    filter: blur(123px);
}

.gradient-2 {
    background: linear-gradient(90deg, #500b88 0%, #580970 100%);
    filter: blur(500px);
}

.wave {
    animation-name: wave-animation;
    animation-duration: 2.5s;
    animation-iteration-count: infinite;
    transform-origin: 70% 70%;
    display: inline-block;
}

@keyframes wave-animation {
    0% {
        transform: rotate(0.0deg)
    }

    10% {
        transform: rotate(14.0deg)
    }

    20% {
        transform: rotate(-8.0deg)
    }

    30% {
        transform: rotate(14.0deg)
    }

    40% {
        transform: rotate(-4.0deg)
    }

    50% {
        transform: rotate(10.0deg)
    }

    60% {
        transform: rotate(0.0deg)
    }

    100% {
        transform: rotate(0.0deg)
    }
}
</style>