<template>
    <footer class="absolute w-full bottom overflow-hidden">
        <div class="w-full relative bg-stone-50 text-black dark:bg-zinc-900 dark:text-white">
            <div
                class="container mx-auto max-w-4xl h-full flex  flex-wrap justify-between items-center text-sm py-6 pl-6 pr-4">
                <div class="mt-4">{{ creator }}</div>
                <div class="flex pt-4 md:p-0 text-left text-xs">
                    <div class="ml-4 cursor-pointer"><a class=" dark:hover:text-white text-zinc-400 hover:text-slate-600 duration-300"
                            target="_blank" href="https://github.com/jarvin-s">
                            <Icon icon="mdi:github" width="28" />
                        </a></div>
                    <div class="ml-4 cursor-pointer"><a class=" dark:hover:text-white text-zinc-400 hover:text-slate-600 duration-300"
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