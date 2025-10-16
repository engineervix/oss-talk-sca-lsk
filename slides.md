---
theme: seriph
background: /images/title-image.svg
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# force color schema for the slides, can be 'auto', 'light', or 'dark'
colorSchema: dark
---

<div class="mb-90">
  <h1>Getting Started With<br><span class="bg-gradient-to-r from-blue-400 via-purple-500 to-pink-500 bg-clip-text text-transparent">Open Source</span></h1>
</div>

<div class="abs-bl m-6 text-left">
  <div class="text-base opacity-75">
    <div class="font-semibold">Victor Miti</div>
    <div>2025-10-17</div>
    <div>Contributhon Extended, Day 1</div>
    <div>SCA Lusaka</div>
  </div>
</div>

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/engineervix/oss-talk-sca-lsk" target="_blank" alt="GitHub" title="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: default
transition: fade-out
---

<style scoped>
.code-wrapper {
  transform: scale(1.4);
  transform-origin: top left;
  margin-bottom: 2rem;
}
</style>

<div class="code-wrapper">

```json
{
  "name": "Victor Miti",
  "likes": [
    "🛠️ building and fixing things",
    "🏃 running",
    "🍲 experimenting with food",
    "🎵 making music",
    "🐶 dogs"
  ],
  "work": {
    "org": "Torchbox",
    "url": "torchbox.com",
    "role": "engineer"
  },
  "links": {
    "home": "victor.co.zm",
    "github": "@engineervix",
  }
}
```

</div>

<img src="/images/victor.jpg" class="rounded-full w-60 h-60 object-cover shadow-2xl absolute top-20 right-20" />

---
layout: default
transition: slide-left
---

# What is Open Source ?


---
layout: default
transition: slide-left
---

# Some Title



---
layout: default
transition: slide-left
---

# Another Title
