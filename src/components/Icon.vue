<script setup>
import { icons } from '../icons';

defineProps(["icon"])
</script>
<template>
<div v-html="icons[icon]"></div>
</template>