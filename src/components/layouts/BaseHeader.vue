<script lang="ts" setup>
import { toggleDark } from "~/composables";
</script>

<template>
  <el-menu class="el-menu-demo" mode="horizontal">
    <el-menu-item index="1">Dashboard</el-menu-item>
    <el-sub-menu index="2">
      <template #title>Menu 1</template>
      <el-menu-item index="2-1">List Data</el-menu-item>
      <el-menu-item index="2-2">Tambah Data</el-menu-item>
    </el-sub-menu>
    <el-sub-menu index="3">
      <template #title>Menu 2</template>
      <el-menu-item index="3-1">List Data</el-menu-item>
      <el-menu-item index="3-2">Tambah Data</el-menu-item>
    </el-sub-menu>
    <el-menu-item h="full" @click="toggleDark()">
      <button
        class="border-none w-full bg-transparent cursor-pointer"
        style="height: var(--ep-menu-item-height)"
      >
        <i inline-flex i="dark:ep-moon ep-sunny" />
      </button>
    </el-menu-item>
  </el-menu>
</template>

<style scoped>

</style>
