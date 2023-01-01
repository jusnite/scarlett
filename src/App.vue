<template>
  <div id="app" class="min-h-screen min-w-full bg-gray-900 text-gray-200">
    <router-view v-slot="{ Component }">
      <transition name="fade" mode="out-in">
        <component :is="Component" />
      </transition>
    </router-view>
  </div>
</template>
