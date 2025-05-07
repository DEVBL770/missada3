<template>
    <div class="flex items-center gap-4 mb-6 bg-white/10 rounded-xl p-4 shadow-md hover:scale-[1.02] transition">
      <img
        :src="item.image"
        :alt="item.name"
        class="w-24 h-24 rounded-md object-cover border border-white"
      />
      <div class="flex-1">
        <h3 class="text-xl text-white font-semibold">{{ item.name }}</h3>
        <p class="text-sm text-gray-300 italic">{{ item.description }}</p>
      </div>
      <div class="text-white font-bold text-lg whitespace-nowrap">
        {{ item.price.toFixed(2) }} €
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    item: Object
  })
  </script>
  