<template>
  <header class="w-full mt-5 p-3 bg-blue-300 flex justify-between items-center">
    <button @click="goHome" class="cursor-pointer">
      <h1 class="text-[25px] text-white font-semibold">Nuxt</h1>
    </button>
    <nav>
      <ul class="flex gap-3">
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/FAQ">FAQ</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<script setup lang="ts">
const router = useRouter();

function goHome() {
  router.push("/");
}
</script>

<style scoped></style>
