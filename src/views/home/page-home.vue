<template>
  <div class="container">
    <div class="text-center text-2xl font-bold">List Menu</div>
    <div class="grid grid-cols-3 mt-5 gap-3">
      <div
        class="bg-blue-200 w-64 h-full rounded-md"
        v-for="menuItem in menuData.slice(0, 6)"
        :key="menuItem.id"
      >
        <div class="py-3 px-2">
          <div class="text-center text-lg font-semibold">
            {{ menuItem.nama }}
          </div>
          <div>{{ menuItem.deskripsi }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { menuData } from "@/data/menuData.js";
</script>

<style lang="scss" scoped></style>
