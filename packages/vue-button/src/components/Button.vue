<template>
  <NuButton class="nu_btn btn_bootstrap" :class="$attrs.class"><slot></slot></NuButton>
</template>

<script setup>
import NuButton from '../index.vue';
</script>

<style>
@import "@_nu/css-button";
@import "@_nu/css-button/lib/skins/bootstrap.css";

.btn_bootstrap:disabled{
  opacity: 0.8;
}
</style>
