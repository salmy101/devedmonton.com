<template>
    <footer class="bg-grey-000">
        <div
            class="max-w-7xl mx-auto py-12 px-4 overflow-hidden sm:px-6 lg:px-8"
        >
            <nav
                class="-mx-5 -my-2 flex flex-wrap justify-center"
                aria-label="Footer"
            >
                <div class="px-5 py-2">
                    <NuxtLink
                        to="/board"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Board
                    </NuxtLink>
                </div>

                <div class="px-5 py-2">
                    <NuxtLink
                        to="/become_a_member"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Become a member
                    </NuxtLink>
                </div>

                <div class="px-5 py-2">
                    <a
                        href="https://docs.google.com/document/d/1i6oXabir-628csa2bQacHpc17Kmhec9EfkyHij9yQGM/edit#heading=h.sns5qzyi4gru"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Bylaws
                    </a>
                </div>

                <div class="px-5 py-2">
                    <NuxtLink
                        to="/code_of_conduct"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Code of Conduct
                    </NuxtLink>
                </div>

                <div class="px-5 py-2">
                    <NuxtLink
                        to="/sponsors"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Sponsors
                    </NuxtLink>
                </div>

                <div class="px-5 py-2">
                    <NuxtLink
                        to="/contact"
                        class="text-base text-gray-600 hover:text-black"
                    >
                        Contact
                    </NuxtLink>
                </div>
            </nav>
            <p class="mt-8 text-center text-base text-gray-500">
                Dev Edmonton Society
            </p>
        </div>
    </footer>
</template>

<script>
export default {};
</script>
