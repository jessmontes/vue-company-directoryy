<script setup>
import { ref } from 'vue';
const brand = ref(' J.M Company') 
</script>



<template>
  <nav>
    <div class="wrapper">
      <div class="brand">
        <span class="brand-title">{{ brand }}</span>
      </div>
      <div class="menu">
        <a href="#" class="menu-item">Departments</a>
        <a href="#" class="menu-item">Settings</a>
        <a href="#" class="menu-login">Logout</a>
      </div>
    </div>
  </nav>
</template>



<style scoped lang="postcss">
nav {
  @apply bg-stone-800 text-blue-300 h-20 flex;
  .wrapper {
    @apply container mx-auto flex w-full items-center justify-between;
    .brand {
      &-title {
        @apply text-2xl font-bold text-blue-400;
      }
    }
    .menu { 
      @apply flex gap-2;
      &-item {
        @apply rounded-md px-4 py-2 hover:bg-blue-400 hover:text-slate-900;
      }
      &-login {
        @apply rounded-md bg-red-500 px-4 py-2 hover:bg-red-700 text-red-100;
      }
    }
  }
}
</style>

