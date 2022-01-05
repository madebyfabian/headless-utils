# headless-utils
My collection of headless utils and Vue.js components I use across projects.

## skip-navigation
Heavily inspired from https://github.com/vue-a11y/vue-skip-to/tree/next.

### Usage
1. Import the `SkipNavigation.vue` as component like this:
```vue
<template>
	<SkipNavigation label="Custom label" to="#main" />
</template>

<script setup>
	import SkipNavigation from 'github:madebyfabian/headless-utils/src/vue3/skip-navigation'
</script>
```