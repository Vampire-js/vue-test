<script setup>
defineProps(["name", "msg", "time"])
</script>
<template>
<div class="p-3 pb-4 border-b-2 border-b-slate-800">
  <div class="header flex items-center text-white"><div class="name font-extrabold text-lg ">{{ name }}</div><span class="text-sm ml-2 font-bold text-slate-500">{{time}}</span></div>
  <div class="msg text-slate-400">{{ msg }}</div>
</div>
</template>