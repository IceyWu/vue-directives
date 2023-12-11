<h1 align="center">vue-directives-lib</h1>
<p align="center">🚀Useful custom directives for vue </p>

<p align="center">
<a href="https://www.npmjs.com/package/vue-directives-lib" target="__blank"><img src="https://img.shields.io/npm/v/vue-directives-lib?color=a1b858&label=" alt="NPM version"></a>
<a href="https://www.npmjs.com/package/vue-directives-lib" target="__blank"><img alt="NPM Downloads" src="https://img.shields.io/npm/dm/vue-directives-lib?color=50a36f&label="></a>
</p>

**Eenglish** | [中文](./README.zh-CN.md)

## 📦 Installation

```bash
npm install vue-directives-lib
or
pnpm add vue-directives-lib
or
yarn add vue-directives-lib
```

## 🦄 Usage

- Global import

```ts
// main.ts
import { createApp } from "vue";
import App from "./App.vue";
import vueDirectives from "vue-directives-lib";

const app = createApp(App);
app.use(vueDirectives);
app.mount("#app");
```

- Local import

```ts
// test.vue
<template>
  <div v-copy="copyValue">{{copyValue}}</div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
import { copy as vCopy } from "vue-directives-lib";
const copyValue = ref("我是复制的内容");
</script>
```

<!-- ## 🐳 功能列表


| 指令名       | 说明                 | 参数                    | 备注                    |
| ------------ | -------------------- | ----------------------- | ----------------------- |
| `v-copy`     | 复制文本内容         | {} |                        | v-copy="'复制的内容'" |
| `v-tooltip` | 文本溢出时在元素周围显示全部内容 | {} | v-tooltip | -->

## 🐳 Function list

| Directive name | Description                                                     | Parameter | Usage                 |
| -------------- | --------------------------------------------------------------- | --------- | --------------------- |
| `v-copy`       | Copy text content                                               | {}        | v-copy="'复制的内容'" |
| `v-tooltip`    | When the text overflows, display all content around the element | {}        | v-tooltip             |
