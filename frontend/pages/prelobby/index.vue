<template>
    <div class="absolute inset-0 -z-10 h-full w-full">
        <!-- dotted background from: https://bg.ibelick.com/ -->
        <!-- Punkte im Hintergrund: bg-[radial-gradient(#e5e7eb_1px,transparent_1px)] [background-size:16px_16px] -->
        <div
            class="flex flex-col justify-between h-screen overflow-hidden sm:mx-0 mx-4"
        >
            <Navbar class="z-30" />
            <Lobbyname class="z-30" />

            <div
                class="flex sm:flex-row flex-col justify-center items-center w-full lg:gap-32 md:gap-24 sm:gap-16 gap-4"
            >
                <UserDisplay />
                <div>
                    <InviteInfo />
                    <StartGame />
                </div>
            </div>
            <div></div>
        </div>
    </div>
</template>

<script setup>
import Navbar from "~/components/prelobby/Navbar.vue";
import Lobbyname from "~/components/prelobby/Lobbyname.vue";
import StartGame from "~/components/prelobby/StartGame.vue";
import UserDisplay from "~/components/prelobby/UserDisplay.vue";
import InviteInfo from "~/components/prelobby/InviteInfo.vue";
</script>

<style lang="scss" scoped></style>
