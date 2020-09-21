# Vue Click Away

Vue 3.0 Compatible Click Away Directive

## Overview

Detect if a click event happened outside of an element. Compatible with Vue 3.x.

## Requirements

- Vue 3.x

## Installation

```
npm i vue-click-away
```

<p></p>

```
yarn add vue-click-away
```

## Usage

:::tip
By default the module exports a directive, you can also use this as a mixin which is documented below.
:::

```html
<template>
  <div v-click-away="onClickAway">
    ...
  </div>
</template>
```

<p></p>

```js
import VueClickAway from "vue3-click-away";
export default {
  directives: {
    ClickAway: VueClickAway,
  },
  methods: {
    onClickAway(event) {
      console.log(event);
    }
  }
}
```

### Mixin

```html
<template>
  <div v-click-away="onClickAway">
    ...
  </div>
</template>
```

<p></p>

```js
import { mixin as VueClickAway } from "vue3-click-away";
export default {
  mixins: [VueClickAway],
  methods: {
    onClickAway(event) {
      console.log(event);
    }
  }
}
```