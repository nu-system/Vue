<template>
  <h1>{{ msg }}</h1>
  <div>
    count is: {{ state.count }}
  </div>
  <p>
    <Button class="_fill _primary" @click="state.count++">Hello World</Button>
    <Button class="_fill _secondary" @click="state.count++">Hello World</Button>
    <Button class="_fill _warning" @click="state.count++">Hello World</Button>
    <Button class="_fill _success" @click="state.count++">Hello World</Button>
    <Button class="_fill _danger" @click="state.count++">Hello World</Button>
  </p>
  <p>
    <Button class="_ghost _primary" @click="state.count++">Hello World</Button>
    <Button class="_ghost _secondary" @click="state.count++">Hello World</Button>
    <Button class="_ghost _warning" @click="state.count++">Hello World</Button>
    <Button class="_ghost _success" @click="state.count++">Hello World</Button>
    <Button class="_ghost _danger" @click="state.count++">Hello World</Button>
  </p>
  <p>
    <Button class="_link _primary" @click="state.count++">Hello World</Button>
    <Button class="_link _secondary" @click="state.count++">Hello World</Button>
    <Button class="_link _warning" @click="state.count++">Hello World</Button>
    <Button class="_link _success" @click="state.count++">Hello World</Button>
    <Button class="_link _danger" @click="state.count++">Hello World</Button>
  </p>
  <p>
    <Button class="_fill _primary _large" @click="state.count++">Hello World</Button>
    <Button class="_fill _primary" @click="state.count++">Hello World</Button>
    <Button class="_fill _primary _small" @click="state.count++">Hello World</Button>
  </p>
</template>

<script setup>
import Button from './components/Button.vue';
import { defineProps, reactive } from 'vue';

defineProps({
  msg: String,
});

const state = reactive({ count: 0 });
</script>

<style>
@import "sacss";
</style>
