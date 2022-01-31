# headless-utils
My collection of headless utils and Vue.js components I use across projects.

## Installation
Install this GitHub Repo globally in your project like this:
```bash
npm i madebyfabian/headless-utils
```

# Patterns
## skip-navigation
Heavily inspired from https://github.com/vue-a11y/vue-skip-to/tree/next.

### Usage
1. Import the `SkipNavigation.vue` as component like this:
```vue
<template>
	<SkipNavigation label="Custom label" to="#main" />
</template>

<script setup>
	import SkipNavigation from 'headless-utils/src/vue3/skip-navigation'
</script>
```

## Headless Accordion/Disclosure
Use https://www.aditus.io/patterns/accordion/#vue-js 

## Headless Notifications
Use https://github.com/sansil/vt-notifications
