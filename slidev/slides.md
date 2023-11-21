---
theme: seriph
background: /wallpaper.webp
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
layout: default
---

# 目次
<Toc class="text-5xl text-black font-bold" maxDepth="1"></Toc>
 
---
layout: default
---

# IchigoJam で「ピアノ」を弾こう！
<div grid="~ cols-3">

  <div class="col-span-2">
    <h2 class="text-green m-2">ピアノのコード</h2>
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
  </div>

  <div class="text-black text-xl font-bold bg-green-200 px-6 py-2">
    <h2 class="text-red">コードの解説</h2><br>
    <div class="m-1">10行目　ファイルの名前</div>
    <div class="m-1">20行目　ボタンを押す設定</div>
    <div class="m-1">30行目　<span class="text-red">Z</span> ボタンに <span class="text-blue">ド</span></div>
    <div class="m-1">40行目　<span class="text-red">X</span> ボタンに <span class="text-blue">レ</span></div>
    <div class="m-1">50行目　<span class="text-red">C</span> ボタンに <span class="text-blue">ミ</span></div>
    <div class="m-1">60行目　<span class="text-red">V</span> ボタンに <span class="text-blue">ファ</span></div>
    <div class="m-1">70行目　<span class="text-red">B</span> ボタンに <span class="text-blue">ソ</span></div>
    <div class="m-1">80行目　<span class="text-red">N</span> ボタンに <span class="text-blue">ラ</span></div>
    <div class="m-1">90行目　<span class="text-red">M</span> ボタンに <span class="text-blue">シ</span></div>
    <div class="m-1">100行目　<span class="text-red">,</span> ボタンに高い <span class="text-blue">ド</span></div>
    <div class="m-1">110行目　20行目に戻る</div>
  </div>

</div>

---
layout: default
---

# 次は IchigoJam でメロディーを奏でよう！

<h2 class="text-4xl text-pink m-2">チューリップの歌</h2>
<pre>
<code class="lang-ichigojam">                                
10 'Tulip Song                   
20 PLAY "T180 CDER CDER GEDCDED"
</code>
</pre>

<h2 class="text-4xl text-yellow m-2">ジングルベル</h2>
<pre>
<code class="lang-ichigojam">                                                    
10 'Jingle Bells Song                                
20 PLAY "T360 O5 ER8ER8E2R ER8ER8E2R E.G.C2 D6E2.R8"
</code>
</pre>

<div class="text-center text-6xl text-black m-2">前奏やサビだけでなく、<br><span class="text-orange">他のところも作ってみよう！</span></div>

---
layout: cover
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# END