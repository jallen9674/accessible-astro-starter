<template>
  <form>
    <div class="mb-4">
        <label for="Name" class="block mb-1 text-sm text-gray-600">Your Name</label>
        <input type="text" name="name"
            class="w-full px-4 py-2 text-base border border-gray-300 rounded outline-none focus:ring-blue-500 focus:border-blue-500 focus:ring-1"
            placeholder="Enter Your Name" />
        <span class="inline-flex text-sm text-green-700">Username available!
            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24"
                stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
            </svg></span>
    </div>
    <div class="mb-4">
        <label for="password" class="block mb-1 text-sm text-gray-600">Password</label>
        <input type="password" name="password"
            class="w-full px-4 py-2 text-base border border-gray-300 rounded outline-none focus:ring-blue-500 focus:border-blue-500 focus:ring-1"
            placeholder="Password" />
        <span class="inline-flex text-sm text-red-700">Password must be 8 characters
            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="none" viewBox="0 0 24 24"
                stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg></span>
    </div>
</form>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const isMenuOpen = ref<boolean>(false)

const openMenu = (action: boolean) => {
  isMenuOpen.value = action;
}
</script>