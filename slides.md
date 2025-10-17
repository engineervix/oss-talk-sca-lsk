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

<div class="absolute bottom-6 right-32 flex items-end">
  <img src="/images/qr-code.png" class="w-40 h-40" />
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
layout: image
image: /images/tachina-lee--wjk_SSqCE4-unsplash.jpg
transition: slide-left
class: text-center
---

<style scoped>
.gradient-title {
  font-size: 6rem;
  font-weight: 900;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899, #f59e0b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 25px 25px rgb(0 0 0 / 0.5));
  line-height: 1.2;
}

.overlay {
  background: rgba(0, 0, 0, 0.4);
}
</style>

<div class="absolute inset-0 overlay"></div>

<div class="absolute inset-0 flex items-center justify-center">
  <h1 class="gradient-title">
    What is Open Source?
  </h1>
</div>

---
layout: default
transition: slide-left
---

<style scoped>
.definition-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  padding: 4rem;
}

.definition-box {
  position: relative;
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 50%, rgba(236, 72, 153, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 3rem 4rem;
  box-shadow: 12px 12px 0 rgba(139, 92, 246, 0.3);
  backdrop-filter: blur(10px);
  max-width: 1000px;
}

.definition-text {
  font-size: 2.5rem;
  line-height: 1.6;
  font-weight: 500;
  text-align: center;
  color: #e5e7eb;
  font-style: italic;
  margin-bottom: 2rem;
}

.definition-highlight {
  color: #a78bfa;
  font-weight: 700;
}

.definition-source {
  text-align: center;
  font-size: 1rem;
  opacity: 0.7;
  margin-top: 1.5rem;
}

.definition-source a {
  color: #8b5cf6;
  text-decoration: none;
  border-bottom: 1px solid rgba(139, 92, 246, 0.3);
  transition: all 0.3s;
}

.definition-source a:hover {
  color: #a78bfa;
  border-bottom-color: #a78bfa;
}

.quote-mark {
  position: absolute;
  font-size: 8rem;
  line-height: 1;
  color: rgba(139, 92, 246, 0.25);
  font-family: Georgia, serif;
}

.quote-start {
  top: -2.0rem;
  left: 1rem;
}
</style>

<div class="definition-container">
  <div class="definition-box">
    <span class="quote-mark quote-start">“</span>
    <div class="definition-text">
      Something people can <span class="definition-highlight">modify</span> and <span class="definition-highlight">share</span> because its design is <span class="definition-highlight">publicly accessible</span>.
    </div>
    <div class="definition-source">
      Source: <a href="https://opensource.com/resources/what-open-source" target="_blank">opensource.com/resources/what-open-source</a>
    </div>
  </div>
</div>

<!-- 
next, we discuss the broad nature of the term and the underlying principles / values.
-->


---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 3rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 2.5rem;
  line-height: 1.3;
  padding-bottom: 0.25rem;
}

.principles-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.25rem;
  padding: 0 3rem;
}

.principle-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1.25rem 1.5rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
  display: flex;
  align-items: flex-start;
  gap: 1rem;
  transition: all 0.3s ease;
}

.principle-card:hover {
  transform: translateY(-2px);
  border-color: rgba(139, 92, 246, 0.5);
  box-shadow: 6px 6px 0 rgba(139, 92, 246, 0.3);
}

.principle-icon {
  font-size: 2.25rem;
  flex-shrink: 0;
  color: #a78bfa;
}

.principle-content {
  flex: 1;
}

.principle-title {
  font-size: 1.2rem;
  font-weight: 600;
  color: #a78bfa;
  margin-bottom: 0.4rem;
}

.principle-description {
  font-size: 0.875rem;
  line-height: 1.4;
  opacity: 0.85;
}
</style>

# Core Values & Principles

<div class="principles-grid">
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-data-share />
    </div>
    <div class="principle-content">
      <div class="principle-title">Open Exchange</div>
      <div class="principle-description">Free sharing of ideas, designs, and information accessible to all</div>
    </div>
  </div>
  
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-partnership />
    </div>
    <div class="principle-content">
      <div class="principle-title">Collaborative Participation</div>
      <div class="principle-description">Working together across boundaries to achieve common goals</div>
    </div>
  </div>
  
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-data-vis-4 />
    </div>
    <div class="principle-content">
      <div class="principle-title">Transparency</div>
      <div class="principle-description">Open processes and decision-making visible to everyone</div>
    </div>
  </div>
  
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-rocket />
    </div>
    <div class="principle-content">
      <div class="principle-title">Rapid Prototyping</div>
      <div class="principle-description">Fast iteration and experimentation to drive innovation</div>
    </div>
  </div>
  
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-trophy />
    </div>
    <div class="principle-content">
      <div class="principle-title">Meritocracy</div>
      <div class="principle-description">Recognition and influence based on the quality of contributions</div>
    </div>
  </div>
  
  <div class="principle-card">
    <div class="principle-icon">
      <carbon-group />
    </div>
    <div class="principle-content">
      <div class="principle-title">Community-Oriented</div>
      <div class="principle-description">Development driven by and for diverse communities</div>
    </div>
  </div>
</div>

<!--
While the term originated in software development, open source designates a broader set of values that extend far beyond code. These principles guide how open source projects operate and why they're successful.
-->

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.25rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.35rem;
  line-height: 1.3;
  padding-bottom: 0.25rem;
}

.subtitle {
  text-align: center;
  font-size: 0.95rem;
  opacity: 0.7;
  margin-bottom: 1.25rem;
}

.timeline-container {
  display: flex;
  gap: 1.25rem;
  padding: 0 3rem;
}

.timeline-line {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-top: 0.4rem;
}

.timeline-dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  margin-bottom: 0.4rem;
  flex-shrink: 0;
}

.timeline-connector {
  width: 2px;
  flex: 1;
  min-height: 45px;
}

.dot-blue { background: #3b82f6; }
.dot-purple { background: #8b5cf6; }
.dot-pink { background: #ec4899; }
.dot-orange { background: #f59e0b; }

.connector-blue { background: linear-gradient(to bottom, #3b82f6, #8b5cf6); }
.connector-purple { background: linear-gradient(to bottom, #8b5cf6, #ec4899); }
.connector-pink { background: linear-gradient(to bottom, #ec4899, #f59e0b); }

.timeline-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 0.6rem;
}

.timeline-era {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.05) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 0.7rem 1rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
}

.era-header {
  display: flex;
  align-items: baseline;
  gap: 0.6rem;
  margin-bottom: 0.35rem;
}

.era-decade {
  font-size: 0.75rem;
  font-weight: 700;
  color: #a78bfa;
  letter-spacing: 0.05em;
  white-space: nowrap;
}

.era-title {
  font-size: 0.95rem;
  font-weight: 600;
  color: #e5e7eb;
}

.era-content {
  font-size: 0.7rem;
  line-height: 1.45;
  opacity: 0.85;
}

.era-highlight {
  color: #a78bfa;
  font-weight: 600;
}
</style>

# A Brief History

<div class="subtitle">From Shared Code to a Global Movement</div>

<div class="timeline-container">
<div class="timeline-line">
<div class="timeline-dot dot-blue"></div>
<div class="timeline-connector connector-blue"></div>
<div class="timeline-dot dot-purple"></div>
<div class="timeline-connector connector-purple"></div>
<div class="timeline-dot dot-pink"></div>
<div class="timeline-connector connector-pink"></div>
<div class="timeline-dot dot-orange"></div>
</div>

<div class="timeline-content">
<div class="timeline-era">
<div class="era-header">
<span class="era-decade">1960s-70s</span>
<span class="era-title">The Hacker Ethic</span>
</div>
<div class="era-content">
Software freely shared in academic labs (MIT).<br>
Focus on collaborative improvement and learning, not profit.
</div>
</div>

<div class="timeline-era">
<div class="era-header">
<span class="era-decade">1980s</span>
<span class="era-title">Software Becomes Property</span>
</div>
<div class="era-content">
Companies sell software under restrictive licenses.<br>
<span class="era-highlight">1985:</span> Richard Stallman launches the <span class="era-highlight">GNU Project</span> championing "Free Software".
</div>
</div>

<div class="timeline-era">
<div class="era-header">
<span class="era-decade">1990s</span>
<span class="era-title">Key Projects Emerge</span>
</div>
<div class="era-content">
<span class="era-highlight">1991:</span> Linus Torvalds starts the <span class="era-highlight">Linux kernel</span>.<br>
<span class="era-highlight">1995:</span> Apache HTTP Server launched.<br>
<span class="era-highlight">1998:</span> "Open Source" coined by Christine Peterson.
</div>
</div>

<div class="timeline-era">
<div class="era-header">
<span class="era-decade">2000s-Today</span>
<span class="era-title">Mainstream & Platforms</span>
</div>
<div class="era-content">
<span class="era-highlight">2005:</span> Linus creates <span class="era-highlight">git</span>.<br>
<span class="era-highlight">2008:</span> <span class="era-highlight">GitHub launched</span>.<br>
Open source now powers the modern internet, from Android to the cloud.
</div>
</div>
</div>
</div>

<!--
ref: https://www.freecodecamp.org/news/brief-history-of-open-source/

-   **The Early Days (1960s-70s): The Hacker Ethic**
    -   In academic and research labs (like MIT), software and its source code were freely shared.
    -   The focus was on collaborative improvement and learning, not profit.
-   **The Shift (1980s): Software Becomes Property**
    -   Companies began selling software under restrictive licenses. You could *use* it, but not see or change the code.
    -   **1985:** Richard Stallman launches the **GNU Project** to create a completely free and open operating system, championing "Free Software" (free as in freedom).
-   **The Foundation (1990s): Key Projects Emerge**
    -   **1991:** A student named Linus Torvalds starts a "hobby" project: the **Linux kernel**. He shares it online.
    -   **1995:** The Apache HTTP Server is launched, which would go on to power a huge portion of the web.
    -   **1998:** The term **"Open Source" is coined** by Christine Peterson to be more business-friendly. Netscape releases its browser's source code, a huge move for a major tech company.
-   **The Explosion (2000s-Today): Mainstream & Collaborative Platforms**
    -   **2005**: Linus Torvalds (yes, the Linux guy!) creates `git` to manage Linux kernel development. It revolutionizes how devs track changes and collaborate.
    -   Companies like Red Hat prove that you can build a successful business model around open-source software (selling support).
    -   **2008:** **GitHub is launched**, built on top of `git`, revolutionizing how devs collaborate on code, making it easier than ever to contribute..
    -   Today, open source is the backbone of the internet and modern technology. From Android to the cloud, it's everywhere!
-->

---
layout: center
class: text-center
transition: slide-left
---

<style scoped>
.xkcd-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  height: 100%;
  padding: 2rem 0;
}

.xkcd-title {
  font-size: 1.75rem;
  font-weight: 600;
  opacity: 0.9;
}

.xkcd-image {
  max-width: 75%;
  max-height: 75vh;
  width: auto;
  height: auto;
  object-fit: contain;
}
</style>

<div class="xkcd-container">
  <div class="xkcd-title">Open Source Today</div>
  <img src="/images/xkcd_2347_dependency_2x.png" class="xkcd-image" alt="XKCD: Dependency - A random person in Nebraska has been maintaining a critical piece of internet infrastructure" />
</div>

<!--
This famous XKCD comic illustrates how critical open source has become - a huge portion of modern digital infrastructure often depends on projects maintained by ordinary people like you and me.
-->
---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 1.75rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 1rem;
  line-height: 1.2;
}

.subtitle {
  text-align: center;
  font-size: 1rem;
  opacity: 0.7;
  margin-bottom: 1.5rem;
  font-style: italic;
}

.myths-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0.6rem;
  padding: 0 2.5rem;
}

.myth-card {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.7rem;
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.05) 0%, rgba(139, 92, 246, 0.05) 100%);
  border: 2px solid rgba(139, 92, 246, 0.2);
  padding: 0.6rem 0.9rem;
  transition: all 0.3s ease;
}

.myth-card:hover {
  border-color: rgba(139, 92, 246, 0.4);
  box-shadow: 0 4px 12px rgba(139, 92, 246, 0.15);
}

.myth-side, .reality-side {
  display: flex;
  gap: 0.65rem;
  align-items: flex-start;
}

.myth-icon, .reality-icon {
  font-size: 1.5rem;
  flex-shrink: 0;
  margin-top: 0.1rem;
}

.myth-icon {
  color: #ef4444;
}

.reality-icon {
  color: #10b981;
}

.myth-content, .reality-content {
  flex: 1;
}

.myth-label, .reality-label {
  font-size: 0.7rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 0.3rem;
}

.myth-label {
  color: #ef4444;
}

.reality-label {
  color: #10b981;
}

.myth-text, .reality-text {
  font-size: 0.8rem;
  line-height: 1.45;
  opacity: 0.9;
}

.myth-text {
  font-style: italic;
}

.reality-highlight {
  color: #a78bfa;
  font-weight: 600;
}
</style>

# Common Misconceptions

<div class="myths-container">
  <div class="myth-card">
    <div class="myth-side">
      <div class="myth-icon">✗</div>
      <div class="myth-content">
        <div class="myth-label">Myth</div>
        <div class="myth-text">"Free" (ZMW 0) means it's low quality or not good enough for serious projects.</div>
      </div>
    </div>
    <div class="reality-side" v-click="1">
      <div class="reality-icon">✓</div>
      <div class="reality-content">
        <div class="reality-label">Reality</div>
        <div class="reality-text">Open source powers mission-critical systems at <span class="reality-highlight">NASA, Google, Microsoft</span>, and the world's stock exchanges. Its quality comes from thousands of expert contributors.</div>
      </div>
    </div>
  </div>

  <div class="myth-card">
    <div class="myth-side">
      <div class="myth-icon">✗</div>
      <div class="myth-content">
        <div class="myth-label">Myth</div>
        <div class="myth-text">It's only for elite developers who write complex algorithms.</div>
      </div>
    </div>
    <div class="reality-side" v-click="2">
      <div class="reality-icon">✓</div>
      <div class="reality-content">
        <div class="reality-label">Reality</div>
        <div class="reality-text"><span class="reality-highlight">Contributions are diverse!</span> Improving documentation, designing a better UI, testing for bugs, managing the community, or translating text are all vital contributions. If you can write, design, or organize, there's a place for you.</div>
      </div>
    </div>
  </div>

  <div class="myth-card">
    <div class="myth-side">
      <div class="myth-icon">✗</div>
      <div class="myth-content">
        <div class="myth-label">Myth</div>
        <div class="myth-text">You can't make money with open source.</div>
      </div>
    </div>
    <div class="reality-side" v-click="3">
      <div class="reality-icon">✓</div>
      <div class="reality-content">
        <div class="reality-label">Reality</div>
        <div class="reality-text">It's a <span class="reality-highlight">massive industry!</span> Companies build profitable businesses by providing services, support, and hosting for open-source software (e.g., <span class="reality-highlight">Red Hat, papermark.com</span>).</div>
      </div>
    </div>
  </div>

  <div class="myth-card">
    <div class="myth-side">
      <div class="myth-icon">✗</div>
      <div class="myth-content">
        <div class="myth-label">Myth</div>
        <div class="myth-text">Open source projects don't have proper support or documentation.</div>
      </div>
    </div>
    <div class="reality-side" v-click="4">
      <div class="reality-icon">✓</div>
      <div class="reality-content">
        <div class="reality-label">Reality</div>
        <div class="reality-text">Major projects have <span class="reality-highlight">extensive documentation</span>, active communities, and professional support options. Many companies offer <span class="reality-highlight">enterprise support</span> for open-source tools.</div>
      </div>
    </div>
  </div>
</div>

<!--
These misconceptions often prevent people from getting started with open source.
By addressing them head-on, we can help remove these mental barriers and encourage more people to contribute.
-->

---
layout: default
transition: fade
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.5rem;
  line-height: 1.2;
}

.subtitle {
  text-align: center;
  font-size: 1.1rem;
  opacity: 0.8;
  margin-bottom: 1.75rem;
  font-weight: 500;
}

.benefits-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.25rem;
  padding: 0 2.5rem;
}

.benefit-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1.25rem 1.5rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
  transition: all 0.3s ease;
}

.benefit-card:hover {
  transform: translateY(-2px);
  border-color: rgba(139, 92, 246, 0.5);
  box-shadow: 6px 6px 0 rgba(139, 92, 246, 0.3);
}

.benefit-header {
  display: flex;
  align-items: center;
  gap: 0.85rem;
  margin-bottom: 0.7rem;
}

.benefit-icon {
  font-size: 2.25rem;
  flex-shrink: 0;
  color: #a78bfa;
}

.benefit-title {
  font-size: 1.25rem;
  font-weight: 700;
  color: #a78bfa;
}

.benefit-description {
  font-size: 0.875rem;
  line-height: 1.45;
  opacity: 0.9;
  margin-bottom: 0.65rem;
}

.benefit-examples {
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
  font-size: 0.8rem;
  opacity: 0.85;
  margin-top: 0.6rem;
  padding-left: 0.65rem;
  border-left: 2px solid rgba(167, 139, 250, 0.3);
}

.example-item {
  display: flex;
  align-items: baseline;
  gap: 0.45rem;
}

.example-role {
  color: #ec4899;
  font-weight: 600;
  min-width: 4rem;
}

.example-text {
  flex: 1;
  line-height: 1.4;
}

.highlight {
  color: #a78bfa;
  font-weight: 600;
}
</style>

# What's in it for you?

<div class="subtitle">Contributing to open source is an investment in your <span class="highlight">skills</span>, <span class="highlight">network</span>, and <span class="highlight">career</span></div>

<div class="benefits-grid">
  <div class="benefit-card">
    <div class="benefit-header">
      <div class="benefit-icon">
        <carbon-portfolio />
      </div>
      <div class="benefit-title">Your Public Portfolio</div>
    </div>
    <div class="benefit-description">
      Instead of just <em>saying</em> you have skills, <strong>show</strong> your work to the world. Your contributions are proof of what you can do.
    </div>
    <div class="benefit-examples">
      <div class="example-item">
        <span class="example-role">Writers:</span>
        <span class="example-text">Clear documentation proves communication skills</span>
      </div>
      <div class="example-item">
        <span class="example-role">Designers:</span>
        <span class="example-text">UI mockups showcase design thinking</span>
      </div>
      <div class="example-item">
        <span class="example-role">PMs:</span>
        <span class="example-text">Organized issues demonstrate leadership</span>
      </div>
      <div class="example-item">
        <span class="example-role">Testers:</span>
        <span class="example-text">Bug reports show attention to detail</span>
      </div>
      <div class="example-item">
        <span class="example-role">Coders:</span>
        <span class="example-text">Merged PRs are real projects on your resume</span>
      </div>
    </div>
  </div>

  <div class="benefit-card">
    <div class="benefit-header">
      <div class="benefit-icon">
        <carbon-education />
      </div>
      <div class="benefit-title">Your Global Classroom</div>
    </div>
    <div class="benefit-description">
      Learn from the best, regardless of where you are in the world. Get real experience that universities can't teach.
    </div>
    <div class="benefit-examples">
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text"><strong>Mentorship</strong> from experienced professionals worldwide</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text"><strong>Code reviews</strong> teach industry best practices</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text"><strong>Real-world team experience</strong> sets you apart</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Learn tools & workflows used by top companies</span>
      </div>
    </div>
  </div>
</div>

<!--
personal development through portfolio building and learning opportunities. 
These are tangible, immediate benefits that students and early career professionals can take advantage of.
-->

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.5rem;
  line-height: 1.2;
}

.subtitle {
  text-align: center;
  font-size: 1.1rem;
  opacity: 0.8;
  margin-bottom: 1.75rem;
  font-weight: 500;
}

.benefits-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.25rem;
  padding: 0 2.5rem;
  margin-bottom: 1.5rem;
}

.benefit-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1.25rem 1.5rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
  transition: all 0.3s ease;
}

.benefit-card:hover {
  transform: translateY(-2px);
  border-color: rgba(139, 92, 246, 0.5);
  box-shadow: 6px 6px 0 rgba(139, 92, 246, 0.3);
}

.benefit-header {
  display: flex;
  align-items: center;
  gap: 0.85rem;
  margin-bottom: 0.7rem;
}

.benefit-icon {
  font-size: 2.25rem;
  flex-shrink: 0;
  color: #a78bfa;
}

.benefit-title {
  font-size: 1.25rem;
  font-weight: 700;
  color: #a78bfa;
}

.benefit-description {
  font-size: 0.875rem;
  line-height: 1.45;
  opacity: 0.9;
  margin-bottom: 0.65rem;
}

.benefit-examples {
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
  font-size: 0.8rem;
  opacity: 0.85;
  margin-top: 0.6rem;
  padding-left: 0.65rem;
  border-left: 2px solid rgba(167, 139, 250, 0.3);
}

.example-item {
  display: flex;
  align-items: baseline;
  gap: 0.45rem;
}

.example-text {
  flex: 1;
  line-height: 1.4;
}

.bottom-note {
  text-align: center;
  font-size: 1.05rem;
  opacity: 0.8;
  margin-top: 0.5rem;
  font-style: italic;
  padding: 0 2.5rem;
}

.highlight {
  color: #a78bfa;
  font-weight: 600;
}
</style>

# What's in it for you?

<div class="subtitle">Contributing to open source is an investment in your <span class="highlight">skills</span>, <span class="highlight">network</span>, and <span class="highlight">career</span></div>

<div class="benefits-grid">
  <div class="benefit-card">
    <div class="benefit-header">
      <div class="benefit-icon">
        <carbon-cloud-satellite-link />
      </div>
      <div class="benefit-title">Your Professional Network</div>
    </div>
    <div class="benefit-description">
      Build genuine connections with people who can help shape your career. Your work speaks louder than any introduction.
    </div>
    <div class="benefit-examples">
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Connect with <strong>peers & mentors</strong> globally</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text"><strong>Future employers</strong> see your passion & work ethic</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Join a supportive <strong>global community</strong></span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Recommendations from maintainers carry weight</span>
      </div>
    </div>
  </div>

  <div class="benefit-card">
    <div class="benefit-header">
      <div class="benefit-icon">
        <carbon-chart-line-smooth />
      </div>
      <div class="benefit-title">Your Career Accelerator</div>
    </div>
    <div class="benefit-description">
      Open source opens doors. From internships to full-time roles, it's a proven path to opportunity.
    </div>
    <div class="benefit-examples">
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text"><strong>Stand out</strong> in job applications with real experience</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Access to <strong>paid programs</strong> (GSoC, Outreachy)</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Companies <strong>actively recruit</strong> from open source</span>
      </div>
      <div class="example-item">
        <span style="color: #a78bfa; margin-right: 0.3rem;">✓</span>
        <span class="example-text">Build <strong>confidence</strong> in your abilities</span>
      </div>
    </div>
  </div>
</div>

<div class="bottom-note">
  The best part? You can start today, right where you are. No special permission needed. 🚀
</div>

<!--
networking and career advancement
-->

---
layout: image
image: /images/nubelson-fernandes-Y376h7VN27c-unsplash.jpg
transition: slide-left
class: text-center
---

<style scoped>
.gradient-title {
  font-size: 6rem;
  font-weight: 900;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899, #f59e0b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 25px 25px rgb(0 0 0 / 0.5));
  line-height: 1.2;
}

.overlay {
  background: rgba(0, 0, 0, 0.4);
}
</style>

<div class="absolute inset-0 overlay"></div>

<div class="absolute inset-0 flex items-center justify-center">
  <h1 class="gradient-title">
    Real World<br>Example
  </h1>
</div>

<!-- Share your story / experience, and encourage folks to get started today -->

<!-- then we transition to talking about git and github -->

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 2rem;
  line-height: 1.2;
}

.scenarios-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
  padding: 0 3rem;
  margin-bottom: 2rem;
}

.scenario-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1.5rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
}

.scenario-title {
  font-size: 1.25rem;
  font-weight: 700;
  color: #a78bfa;
  margin-bottom: 1.25rem;
  text-align: center;
}

.file-list {
  background: rgba(0, 0, 0, 0.3);
  padding: 1rem 1.25rem;
  border-radius: 0.5rem;
  font-family: 'Monaco', 'Courier New', monospace;
  font-size: 0.85rem;
  line-height: 1.8;
  margin-bottom: 1rem;
}

.file-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  opacity: 0.9;
}

.file-icon {
  color: #60a5fa;
}

.team-chaos {
  background: rgba(0, 0, 0, 0.3);
  padding: 1rem 1.25rem;
  border-radius: 0.5rem;
  font-family: 'Monaco', 'Courier New', monospace;
  font-size: 0.85rem;
  line-height: 1.8;
  margin-bottom: 1rem;
}

.speech-bubble {
  opacity: 0.9;
}

.caption {
  text-align: center;
  font-size: 1.1rem;
  font-weight: 600;
  color: #ec4899;
  margin-top: 0.5rem;
}

.punchline {
  text-align: center;
  font-size: 1.75rem;
  font-weight: 700;
  color: #a78bfa;
  margin-top: 1rem;
}
</style>

# The Problem Git Solves

<div class="scenarios-container">
  <div class="scenario-card" v-click="1">
    <div class="scenario-title">Individual</div>
    <div class="file-list">
      <div class="file-item">
        <span class="file-icon">📄</span>
        <span>final_project.zip</span>
      </div>
      <div class="file-item">
        <span class="file-icon">📄</span>
        <span>final_project_v2.zip</span>
      </div>
      <div class="file-item">
        <span class="file-icon">📄</span>
        <span>final_project_FIXED.zip</span>
      </div>
      <div class="file-item">
        <span class="file-icon">📄</span>
        <span>final_project_ACTUAL_FINAL.zip</span>
      </div>
      <div class="file-item">
        <span class="file-icon">📄</span>
        <span>final_project_USE_THIS_ONE.zip</span>
      </div>
    </div>
    <div class="caption">Which one actually works? 🤷‍♀️</div>
  </div>

  <div class="scenario-card" v-click="2">
    <div class="scenario-title">Team</div>
    <div class="team-chaos">
      <div class="speech-bubble">"I updated the homepage yesterday..."</div>
      <div class="speech-bubble">"Wait, who changed the CSS?"</div>
      <div class="speech-bubble">"My version doesn't have those changes!"</div>
      <div class="speech-bubble">"Can we go back to Friday's version?"</div>
    </div>
    <div class="caption">Sound familiar? 😅</div>
  </div>
</div>

<div class="punchline" v-click="3">
  Git solves this. Here's how. →
</div>

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.25rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 0.4rem;
  line-height: 1.2;
}

.subtitle {
  text-align: center;
  font-size: 1rem;
  opacity: 0.8;
  margin-bottom: 1.5rem;
  font-weight: 500;
}

.concepts-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
  padding: 0 2.5rem;
}

.concept-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1rem 1.25rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
  transition: all 0.3s ease;
}

.concept-card:hover {
  transform: translateY(-2px);
  border-color: rgba(139, 92, 246, 0.5);
  box-shadow: 6px 6px 0 rgba(139, 92, 246, 0.3);
}

.concept-header {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  margin-bottom: 0.6rem;
}

.concept-icon {
  font-size: 2rem;
  flex-shrink: 0;
  color: #a78bfa;
}

.concept-title {
  font-size: 1.1rem;
  font-weight: 700;
  color: #a78bfa;
}

.concept-description {
  font-size: 0.8rem;
  line-height: 1.4;
  opacity: 0.9;
  margin-bottom: 0.6rem;
}

.concept-analogy {
  background: rgba(139, 92, 246, 0.15);
  padding: 0.5rem 0.75rem;
  border-radius: 0.5rem;
  font-size: 0.75rem;
  line-height: 1.3;
  font-style: italic;
}

.analogy-label {
  font-weight: 600;
  color: #ec4899;
  font-style: normal;
  margin-right: 0.3rem;
}

.highlight {
  color: #a78bfa;
  font-weight: 600;
}
</style>

# Git: Key Concepts

<div class="subtitle">Four essential ideas to understand version control</div>

<div class="concepts-grid">
  <div class="concept-card">
    <div class="concept-header">
      <div class="concept-icon">
        <carbon-folder />
      </div>
      <div class="concept-title">Repository (Repo)</div>
    </div>
    <div class="concept-description">
      Your project folder that Git watches. It tracks every change made to your files over time.
    </div>
    <div class="concept-analogy">
      <span class="analogy-label">Think:</span> A project with superpowers
    </div>
  </div>

  <div class="concept-card">
    <div class="concept-header">
      <div class="concept-icon">
        <carbon-save />
      </div>
      <div class="concept-title">Commit</div>
    </div>
    <div class="concept-description">
      A snapshot of your work at a specific moment. Includes <span class="highlight">what</span> changed, <span class="highlight">who</span> changed it, <span class="highlight">when</span>, and <span class="highlight">why</span>.
    </div>
    <div class="concept-analogy">
      <span class="analogy-label">Think:</span> Save points in a video game
    </div>
  </div>

  <div class="concept-card">
    <div class="concept-header">
      <div class="concept-icon">
        <carbon-branch />
      </div>
      <div class="concept-title">Branch</div>
    </div>
    <div class="concept-description">
      A separate copy to try new ideas without breaking what works. Everyone can work on different features at the same time.
    </div>
    <div class="concept-analogy">
      <span class="analogy-label">Think:</span> Working on a draft while keeping the original safe
    </div>
  </div>

  <div class="concept-card">
    <div class="concept-header">
      <div class="concept-icon">
        <carbon-cloud-upload />
      </div>
      <div class="concept-title">Remote (GitHub)</div>
    </div>
    <div class="concept-description">
      Where your code lives online so your team can access it from anywhere. Makes collaboration seamless.
    </div>
    <div class="concept-analogy">
      <span class="analogy-label">Think:</span> Google Drive, but for code
    </div>
  </div>
</div>

<!--
Four fundamental Git concepts that beginners need to understand. 
-->

---
layout: center
class: text-center
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.25rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 1.5rem;
  line-height: 1.2;
}

.video-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
}

.video-wrapper {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
  border: 3px solid rgba(139, 92, 246, 0.4);
  border-radius: 0.5rem;
  overflow: hidden;
  box-shadow: 0 10px 40px rgba(139, 92, 246, 0.3);
}

.video-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>

# A brief introduction to Git for beginners

<div class="video-container">
  <div class="video-wrapper">
    <iframe 
      src="https://www.youtube.com/embed/r8jQ9hVA2qs" 
      title="A brief introduction to Git for beginners | GitHub"
      frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
      allowfullscreen>
    </iframe>
  </div>
</div>

<!--
Watch in your own time -- it's less than 10 min
-->

---
layout: image
image: /images/rubaitul-azad-HLQDfaJUTVI-unsplash.jpg
transition: slide-left
---

<!--
key points for getting started:
1. Find a Welcoming Project - Look for projects with `good first issue` or `help wanted` labels
2. Start with What You Know - Improving documentation is a great first contribution
3. Read the CONTRIBUTING.md File - Understand the project's process and Code of Conduct
4. Don't Be Afraid to Ask - Use community channels (Discord, Slack, GitHub Discussions)
-->

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 2rem;
  line-height: 1.2;
}

.subtitle {
  text-align: center;
  font-size: 1rem;
  opacity: 0.8;
  margin-bottom: 2rem;
  font-weight: 500;
}

.resources-list {
  padding: 0 4rem;
  line-height: 2.2;
}

.resources-list ul {
  list-style: none;
  padding: 0;
}

.resources-list li {
  font-size: 1.1rem;
  margin-bottom: 1rem;
}

.resource-name {
  font-weight: 700;
  color: #a78bfa;
}

.resource-name a {
  color: #a78bfa;
  text-decoration: none;
  transition: color 0.3s;
}

.resource-name a:hover {
  color: #c4b5fd;
  text-decoration: underline;
}

.resource-description {
  font-size: 0.9rem;
  opacity: 0.85;
  margin-left: 1.5rem;
}
</style>

# Check These Out

<div class="subtitle">Programs and communities to help you get started</div>

<div class="resources-list">

- **[GitHub Student Developer Pack](https://education.github.com/pack)** — Free access to the best developer tools
- **[Google Summer of Code (GSoC)](https://summerofcode.withgoogle.com/)** — Paid, mentored program to work on open source
- **[Outreachy](https://www.outreachy.org/)** — Paid internships for underrepresented groups in tech
- **[GoodFirstIssue.dev](https://goodfirstissue.dev/)** — Curated easy-to-tackle issues from popular projects
- **[SCA](https://shecodeafrica.org/)** — Collaborate, ask for help, find mentors right here!

</div>

<!--
Programs and communities that provide support, mentorship, and opportunities for getting started with open source.
-->

---
layout: default
transition: slide-left
---

<style scoped>
h1 {
  text-align: center;
  font-size: 2.75rem;
  font-weight: 700;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  margin-bottom: 2.5rem;
  line-height: 1.2;
}

.links-container {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  padding: 0 4rem;
}

.link-card {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(139, 92, 246, 0.1) 100%);
  border: 2px solid rgba(139, 92, 246, 0.3);
  padding: 1.75rem 2rem;
  box-shadow: 4px 4px 0 rgba(139, 92, 246, 0.2);
  transition: all 0.3s ease;
}

.link-card:hover {
  transform: translateY(-2px);
  border-color: rgba(139, 92, 246, 0.5);
  box-shadow: 6px 6px 0 rgba(139, 92, 246, 0.3);
}

.link-title {
  font-size: 1.1rem;
  font-weight: 600;
  color: #a78bfa;
  margin-bottom: 0.75rem;
}

.link-url {
  font-size: 0.9rem;
  font-family: 'Monaco', 'Courier New', monospace;
  color: #60a5fa;
  word-break: break-all;
}

.link-url a {
  color: #60a5fa;
  text-decoration: none;
  transition: color 0.3s;
}

.link-url a:hover {
  color: #93c5fd;
  text-decoration: underline;
}
</style>

# Additional Resources

<div class="links-container">
  <div class="link-card">
    <div class="link-title">This article goes hand-in-hand with the video I shared earlier</div>
    <div class="link-url">
      <a href="https://github.blog/developer-skills/programming-languages-and-frameworks/what-is-git-our-beginners-guide-to-version-control/" target="_blank">
        github.blog/developer-skills/programming-languages-and-frameworks/what-is-git-our-beginners-guide-to-version-control/
      </a>
    </div>
  </div>

  <div class="link-card">
    <div class="link-title">Essential Git commands you should know</div>
    <div class="link-url">
      <a href="https://github.blog/developer-skills/github/top-12-git-commands-every-developer-must-know/" target="_blank">
        github.blog/developer-skills/github/top-12-git-commands-every-developer-must-know/
      </a>
    </div>
  </div>
</div>

<!--
Links to helpful articles for continuing the learning journey.
-->

---
layout: image
image: /images/elissa-garcia-ckVjMurwKIs-unsplash.jpg
transition: slide-left
class: text-center
---

<style scoped>
.gradient-title {
  font-size: 6rem;
  font-weight: 900;
  background: linear-gradient(to right, #3b82f6, #8b5cf6, #ec4899, #f59e0b);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 25px 25px rgb(0 0 0 / 0.5));
  line-height: 1.2;
}

.overlay {
  background: rgba(0, 0, 0, 0.4);
}
</style>

<div class="absolute inset-0 overlay"></div>

<div class="absolute inset-0 flex items-center justify-center">
  <h1 class="gradient-title">
    Questions?
  </h1>
</div>

<!--
Q&A
-->
