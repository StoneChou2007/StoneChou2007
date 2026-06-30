---
layout: archive
title: "portfolio"
permalink: /portfolio/
author_profile: true
---

{% include base_path %}

<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+SC:wght@400;500;600&family=Noto+Sans+SC:wght@300;400;500&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>
/* ===== S. Chow — portfolio gallery (shares home tokens) ===== */
.s-port{
  --ink:#23262e;
  --frost:#3a6ea5;
  --frost-soft:rgba(58,110,165,.12);
  --mist:#6b7280;
  --line:rgba(35,38,46,.10);
  --radius:18px;
  max-width:860px;margin:0 auto;
  font-family:"Inter","Noto Sans SC",system-ui,-apple-system,sans-serif;
  color:var(--ink);
}
.s-port *{box-sizing:border-box;}

@keyframes sFadeUp{from{opacity:0;transform:translateY(14px);}to{opacity:1;transform:none;}}

.s-port .s-eyebrow{
  margin:0 0 1.2rem;
  font-size:.72rem;font-weight:600;letter-spacing:.22em;
  text-transform:uppercase;color:var(--frost);
}

.s-gallery{
  display:grid;gap:1rem;
  grid-template-columns:repeat(2,minmax(0,1fr));
}
.s-shot{
  position:relative;display:block;
  border-radius:var(--radius);overflow:hidden;
  border:1px solid var(--line);
  background:var(--frost-soft);
  text-decoration:none;
  animation:sFadeUp .6s cubic-bezier(.2,.7,.2,1) both;
  transition:transform .2s ease, box-shadow .2s ease, border-color .2s ease;
}
.s-shot:nth-child(2){animation-delay:.08s;}
.s-shot:nth-child(3){animation-delay:.16s;}
.s-shot:hover{
  transform:translateY(-4px);
  border-color:var(--frost);
  box-shadow:0 24px 44px -28px rgba(35,38,46,.75);
}
/* feature: first item spans full width (delete this rule for a uniform grid) */
.s-shot.feature{grid-column:1 / -1;}

.s-img{position:relative;width:100%;overflow:hidden;background:var(--frost-soft);}
.s-shot.feature .s-img{aspect-ratio:16 / 9;}
.s-shot:not(.feature) .s-img{aspect-ratio:4 / 3;}
.s-img img{
  width:100%;height:100%;object-fit:cover;display:block;
  transition:transform .55s cubic-bezier(.2,.7,.2,1);
}
.s-shot:hover .s-img img{transform:scale(1.06);}

.s-cap{
  position:absolute;left:0;right:0;bottom:0;
  padding:1.1rem 1.15rem .95rem;
  display:flex;align-items:flex-end;justify-content:space-between;gap:.8rem;
  background:linear-gradient(to top, rgba(12,14,18,.82), rgba(12,14,18,.32) 55%, transparent);
}
.s-cap .t{
  font-family:"Noto Serif SC",serif;
  color:#fff;font-weight:500;font-size:1.05rem;line-height:1.4;
  text-shadow:0 1px 10px rgba(0,0,0,.45);
}
.s-cap .go{
  flex:none;color:#fff;font-size:.85rem;font-weight:500;
  opacity:0;transform:translateX(-4px);white-space:nowrap;
  transition:opacity .2s ease, transform .2s ease;
}
.s-shot:hover .s-cap .go{opacity:.95;transform:none;}

@media (max-width:680px){
  .s-gallery{grid-template-columns:1fr;}
  .s-shot.feature{grid-column:auto;}
  .s-shot:not(.feature) .s-img{aspect-ratio:16 / 10;}
}
.s-port a:focus-visible{outline:2px solid var(--frost);outline-offset:3px;}
@media (prefers-reduced-motion:reduce){
  .s-shot{animation:none;transition:none;}
  .s-img img{transition:none;}
}
</style>

<div class="s-port" markdown="0">

  <p class="s-eyebrow">images · essays · records</p>

  <div class="s-gallery">

    <a class="s-shot feature" href="{{ '/portfolio/portfolio-1' | relative_url }}">
      <div class="s-img">
        <img src="{{ '/images/goldenhour.png' | relative_url }}" alt="Golden Hour at SHSSIP">
      </div>
      <div class="s-cap">
        <span class="t">Golden Hour at SHSSIP</span>
        <span class="go">查看 →</span>
      </div>
    </a>

    <a class="s-shot" href="{{ '/portfolio/portfolio-2' | relative_url }}">
      <div class="s-img">
        <img src="{{ '/images/xiaguan.jpg' | relative_url }}" alt="Xiaguan Forum and related">
      </div>
      <div class="s-cap">
        <span class="t">Xiaguan Forum and related</span>
        <span class="go">查看 →</span>
      </div>
    </a>

    <a class="s-shot" href="{{ '/portfolio/portfolio-3' | relative_url }}">
      <div class="s-img">
        <img src="{{ '/images/kyra.jpg' | relative_url }}" alt="佩铂中士的寂寞芳心俱乐部（一部未名的词典）">
      </div>
      <div class="s-cap">
        <span class="t">佩铂中士的寂寞芳心俱乐部（一部未名的词典）</span>
        <span class="go">查看 →</span>
      </div>
    </a>

  </div>

</div>
