<script setup lang="ts">
  import SkipNavigation from '../../../src/vue3/skip-navigation/SkipNavigation.vue'
</script>

<template>
  <SkipNavigation />

  <h1>Demo Page</h1>
  <p>Some demo content</p>
  <button>Have fun!</button>
  <h2>Navigation:</h2>
  <ul>
    <li><a href="#">Make stuff</a></li>
    <li><a href="#">Do stuff</a></li>
    <li><a href="#">Do more stuff</a></li>
  </ul>
  <hr>
  <main id="main">
    <h2>Content</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo nesciunt rerum tempore distinctio. Alias autem dolorem non fuga consectetur eius dolore suscipit consequatur aut iste! Eos reiciendis delectus eum ab!</p>
    <a href="#">Go there &rarr;</a>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex facilis, tempore inventore tempora dolor omnis magni saepe beatae, veritatis obcaecati dolores soluta earum reiciendis repellat. Voluptate quam rerum iusto explicabo?</p>
    <button>Went here</button>
  </main>
</template>