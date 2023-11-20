---
theme: seriph
background: /cover.webp
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## Robosava mini corner
  Presentation slides for Hiroshima robosava.

  Learn more at [ロボサバ](https://robosava.jp/)
drawings:
  persist: false
transition: slide-left
title: 響け、メロディー♪
mdc: true
---

# 響け、メロディー♪

<div class="text-2xl">IchigoJam から愛を込めて</div>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="text-4xl px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Space で進む <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="absolute bottom-8">
  by Akio Muto 2023
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/Marukome0743/IchigoJam" target="_blank" alt="GitHub" title="Open in GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
layout: image
image: /head.webp
class: 
---

# 目次
<Toc class="text-5xl text-black font-bold" maxDepth="1"></Toc>
 
---
layout: image
image: /content.webp
---

# IchigoJam で「ピアノ」を弾こう！

<br>

<pre>
<code class="lang-ichigojam">                           
10 'PIANO                   
20 K=INKEY()                
30 IF K=ASC("Z") PLAY "O4C" 
40 IF K=ASC("X") PLAY "O4D" 
50 IF K=ASC("C") PLAY "O4E" 
60 IF K=ASC("V") PLAY "O4F" 
70 IF K=ASC("B") PLAY "O4G" 
80 IF K=ASC("N") PLAY "O4A" 
90 IF K=ASC("M") PLAY "O4B" 
100 IF K=ASC(",") PLAY "O5C"
110 GOTO 20                
</code>
</pre>

---
layout: image
image: /content.webp
---

# 次は IchigoJam でメロディーを奏でよう！

<br>
<div class="text-4xl text-pink m-2">
  チューリップの歌
</div>
<pre>
<code class="lang-ichigojam">                                
10 'Tulip Song                   
20 PLAY "T180 CDER CDER GEDCDED"
</code>
</pre>

---
layout: image
image: /spine.webp
---

# END