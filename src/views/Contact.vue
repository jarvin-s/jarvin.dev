<template>
    <div class="target" v-motion-pop-visible-once>
        <section class="bg-zinc-100 dark:bg-zinc-800 contact pt-20 pb-20">
            <form
                class="box bg-zinc-300 space-y-8 py-8 lg:py-16 mx-auto max-w-screen-sm dark:bg-black shadow-lg px-8 pt-6 mb-4">
                <div>
                    <h1 class="mb-4 text-4xl text-black text-center dark:text-white font-bold">Interested in <span
                            class="text-transparent bg-clip-text bg-gradient-to-r from-purple-600 to-pink-500">working</span>
                        together?
                    </h1>
                    <h4 class="text-black flex dark:text-white text-left justify-center sm:text-center opacity-80">Don't
                        hesitate and reach out today!
                        <Icon class="flex ml-1" icon="twemoji:rocket" width="26" />
                    </h4>
                </div>
                <div>
                    <label for="name" class="block mb-2 text-sm font-bold text-black dark:text-white">Name</label>
                    <input type="name" id="name"
                        class="shadow-sm bg-gray-50 border border-gray-300 text-black text-sm rounded-lg block w-full p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
                        placeholder="Your full name" required>
                </div>
                <div>
                    <label for="email" class="block mb-2 text-sm font-bold text-black dark:text-white">Email</label>
                    <input type="text" id="email"
                        class="block p-3 w-full text-sm text-black bg-gray-50 rounded-lg border border-gray-300 shadow-sm dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light"
                        placeholder="name@example.com" required>
                </div>
                <div class="sm:col-span-2">
                    <label for="message" class="block mb-2 text-sm font-bold text-black dark:text-white">Message</label>
                    <textarea id="message" rows="6"
                        class="block p-2.5 w-full text-sm text-black bg-gray-50 rounded-lg shadow-sm border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500"
                        placeholder="Your message"></textarea>
                </div>
                <button @click="sendMessage()"
                    class="btn-send-light dark:btn-send-dark flex dark:text-white font-bold py-2 px-4 rounded-lg focus:outline-none focus:shadow-outline"
                    type="button">
                    <Icon class="mr-2 mt-0.5" icon="ion:md-send" width="24" />
                    Send message
                </button>
            </form>
        </section>
    </div>
</template>

<script>
import { Icon } from '@iconify/vue'

export default {
    components: {
        Icon,
    },
    methods: {
        sendMessage() {
            alert("Contact does not work as of currently.");
        }
    }
}
</script>

<style scoped>
.box {
    position: relative;
    transform-style: preserve-3d;
}

.box::before {
    content: '';
    position: absolute;
    inset: 0px;
    background: conic-gradient(from 60deg at 40% -25%, #ee6907, #e6390a, #de0d0d, #d61039, #cf1261, #c71585, #cf1261, #d61039, #de0d0d, #ee6907, #f79d03, #ffd700, #ffd700, #ffd700);
    filter: blur(10px);
    transform: translate3d(0px, 0px, -1px);
    clip-path: polygon(-100vmax -100vmax, 100vmax -100vmax, 100vmax 100vmax, -100vmax 100vmax, -100vmax -100vmax, 0 0, 0 100%, 100% 100%, 100% 0, 0 0);
}

@tailwind utilities;

@layer utilities {
    .btn-send-dark {
        box-shadow: 0 0 6px 0 rgba(157, 96, 212, 2);
        border: solid 3px transparent;
        background-image: linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0)), linear-gradient(60deg, #a80195, #e72656e0);
        background-origin: border-box;
        box-shadow: 2px 1000px 1px black inset;
        color: white;
        transition: 300ms;
    }

    .btn-send-dark:hover {
        box-shadow: none;
    }
}

.btn-send-light {
    box-shadow: 0 0 6px 0 rgba(157, 96, 212, 2);
    border: solid 3px transparent;
    background-image: linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0)), linear-gradient(60deg, #a80195, #e72656e0);
    background-origin: border-box;
    box-shadow: 2px 1000px 1px black inset;
    color: white;
    transition: 300ms;
}

.btn-send-light:hover {
    box-shadow: none;
}
</style>