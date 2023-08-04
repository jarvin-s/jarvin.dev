<template>
    <footer class="absolute w-full bottom overflow-hidden">
        <div class="w-full relative bg-stone-50 text-black dark:bg-zinc-900 dark:text-white">
            <div
                class="container mx-auto max-w-4xl h-full flex  flex-wrap justify-between items-center text-sm py-6 pl-6 pr-4">
                <div class="mt-4">{{ creator }}</div>
                <div class="flex pt-4 md:p-0 text-left text-xs">
                    <div class="ml-4 cursor-pointer"><a class=" dark:hover:text-zinc-400 hover:text-slate-600 duration-300"
                            target="_blank" href="https://github.com/jarvin-s">
                            <Icon icon="mdi:github" width="28" />
                        </a></div>
                    <div class="ml-4 cursor-pointer"><a class=" dark:hover:text-zinc-400 hover:text-slate-600 duration-300"
                            target="_blank" href="https://www.linkedin.com/in/jarvin-siegers-65bbb11bb/">
                            <Icon icon="mdi:linkedin" width="28" />
                        </a></div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
import { Icon } from '@iconify/vue'

export default {
    components: {
        Icon,
    },
    data() {
        return {
            creator: "Made with 🤓 by Jarvin. All rights reserved.",
            privacy: "Privacy Policy",
            tos: "Terms & Conditions",
            contactMe: "Contact me"
        }
    }
}
</script>

<style scoped>
/* footer {
    padding-block: 7rem;
}

.wavy {
    background: #111111;

    --mask:
        radial-gradient(132.49px at 50% 179.55px, #000 99%, #0000 101%) calc(50% - 126px) 0/252px 100%,
        radial-gradient(132.49px at 50% -116.55px, #0000 99%, #000 101%) 50% 63px/252px 100% repeat-x;
    -webkit-mask: var(--mask);
    mask: var(--mask);
} */
</style>