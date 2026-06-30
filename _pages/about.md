---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+SC:wght@400;500;600&family=Noto+Sans+SC:wght@300;400;500&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>
/* =========================================================
   S. Chow — home
   Tokens:  ink #23262e · frost #3a6ea5 · mist #6b7280
            paper rgba overlays · seal (vermilion) #bb3b2e
   ========================================================= */
.s-home{
  --ink:#23262e;
  --frost:#3a6ea5;
  --frost-soft:rgba(58,110,165,.14);
  --mist:#6b7280;
  --seal:#bb3b2e;
  --line:rgba(35,38,46,.10);
  --pane:rgba(255,255,255,.55);
  --radius:18px;
  --maxw:860px;
  max-width:var(--maxw);
  margin:0 auto;
  font-family:"Inter","Noto Sans SC",system-ui,-apple-system,sans-serif;
  color:var(--ink);
}
.s-home *{box-sizing:border-box;}

/* ---------- entrance ---------- */
@keyframes sFadeUp{from{opacity:0;transform:translateY(14px);}to{opacity:1;transform:none;}}
@keyframes sDrift{0%{transform:translate(-6%,-4%);}50%{transform:translate(6%,4%);}100%{transform:translate(-6%,-4%);}}
.s-home > *{animation:sFadeUp .6s cubic-bezier(.2,.7,.2,1) both;}
.s-home > *:nth-child(2){animation-delay:.08s;}
.s-home > *:nth-child(3){animation-delay:.16s;}
.s-home > *:nth-child(4){animation-delay:.24s;}
.s-home > *:nth-child(5){animation-delay:.32s;}

/* ---------- hero ---------- */
.s-hero{
  position:relative;
  overflow:hidden;
  margin:0 0 1.4rem;
  padding:2.4rem 1.8rem 2.1rem;
  border-radius:var(--radius);
  border:1px solid var(--line);
  background:
    radial-gradient(120% 120% at 0% 0%, var(--frost-soft), transparent 55%),
    linear-gradient(160deg, rgba(35,38,46,.045), rgba(35,38,46,.012));
}
.s-hero::before{
  content:"";
  position:absolute;
  inset:-40%;
  z-index:0;
  background:radial-gradient(closest-side, var(--frost-soft), transparent 70%);
  animation:sDrift 22s ease-in-out infinite;
  pointer-events:none;
}
.s-hero > *{position:relative;z-index:1;}
.s-eyebrow{
  margin:0 0 .7rem;
  font-size:.72rem;
  font-weight:600;
  letter-spacing:.22em;
  text-transform:uppercase;
  color:var(--frost);
}
.s-hero h1{
  margin:0 0 .55rem;
  font-family:"Noto Serif SC",serif;
  font-weight:600;
  font-size:clamp(1.9rem,5vw,2.6rem);
  line-height:1.15;
  letter-spacing:.5px;
  background:linear-gradient(115deg,var(--ink) 30%,var(--frost) 100%);
  -webkit-background-clip:text;background-clip:text;
  -webkit-text-fill-color:transparent;color:var(--ink);
}
.s-hero p{
  margin:0;
  max-width:46ch;
  line-height:1.85;
  font-weight:400;
  color:var(--ink);
  opacity:.86;
}
.s-hero p .en{font-family:"Inter",sans-serif;font-size:.94rem;opacity:.7;}

.s-actions{display:flex;flex-wrap:wrap;gap:.6rem;margin-top:1.3rem;}
.s-actions a{
  display:inline-flex;align-items:center;gap:.4rem;
  padding:.55rem 1.05rem;
  border-radius:999px;
  border:1px solid var(--line);
  background:rgba(255,255,255,.4);
  font-size:.9rem;font-weight:500;
  color:var(--ink);text-decoration:none;
  transition:transform .18s ease, border-color .18s ease, background .18s ease, box-shadow .18s ease;
}
.s-actions a:hover{
  transform:translateY(-2px);
  border-color:var(--frost);
  background:rgba(58,110,165,.08);
  box-shadow:0 8px 22px -14px rgba(58,110,165,.7);
}
.s-actions a.primary{
  border-color:transparent;
  background:linear-gradient(120deg,var(--frost),#2f5d8c);
  color:#fff;
}
.s-actions a.primary:hover{box-shadow:0 10px 26px -12px rgba(47,93,140,.85);}

/* ---------- poem (signature card) ---------- */
.s-poem{
  position:relative;
  margin:0 0 1.7rem;
  padding:1.8rem 1.8rem 1.5rem;
  border-radius:var(--radius);
  border:1px solid var(--line);
  background:linear-gradient(180deg, rgba(35,38,46,.035), rgba(35,38,46,.015));
}
.s-poem blockquote{
  margin:0;padding:0 0 0 1.3rem;
  border-left:3px solid var(--frost);
  font-family:"Noto Serif SC",serif;
  font-weight:400;
  font-size:1.18rem;
  line-height:2.25;
  letter-spacing:.04em;
  color:var(--ink);
}
.s-poem .s-date{
  margin-top:1rem;
  text-align:right;
  font-family:"Noto Serif SC",serif;
  font-size:.92rem;
  letter-spacing:.06em;
  color:var(--mist);
}
/* --- decorative seal (delete this span + block to remove) --- */
.s-seal{
  position:absolute;top:1.5rem;right:1.6rem;
  display:grid;place-items:center;
  width:52px;height:52px;
  border-radius:8px;
  background:var(--seal);
  color:#fff;
  font-family:"Noto Serif SC",serif;
  font-size:1.55rem;font-weight:600;
  transform:rotate(-4deg);
  box-shadow:inset 0 0 0 2px rgba(255,255,255,.35), 0 6px 18px -10px rgba(187,59,46,.8);
  opacity:.92;user-select:none;
}

/* ---------- section heading ---------- */
.s-kicker{
  margin:0 0 .9rem;
  font-family:"Noto Sans SC",sans-serif;
  font-size:1.05rem;font-weight:500;
  letter-spacing:.04em;
  color:var(--ink);
}
.s-kicker::before{
  content:"";display:inline-block;
  width:18px;height:2px;margin:0 .55rem .28rem 0;
  background:var(--frost);vertical-align:middle;
}

/* ---------- nav cards ---------- */
.s-grid{
  display:grid;gap:.9rem;margin:0 0 1.7rem;
  grid-template-columns:repeat(3,minmax(0,1fr));
}
.s-card{
  display:flex;flex-direction:column;gap:.35rem;
  padding:1.15rem 1.2rem;
  border-radius:14px;
  border:1px solid var(--line);
  background:var(--pane);
  text-decoration:none;color:var(--ink);
  transition:transform .18s ease, border-color .18s ease, box-shadow .18s ease;
}
.s-card:hover{
  transform:translateY(-3px);
  border-color:var(--frost);
  box-shadow:0 14px 30px -20px rgba(35,38,46,.6);
}
.s-card .ico{font-size:1.2rem;line-height:1;}
.s-card .t{font-family:"Noto Sans SC",sans-serif;font-weight:500;}
.s-card .s{font-size:.82rem;color:var(--mist);}
.s-card .go{margin-top:.2rem;font-size:.84rem;color:var(--frost);font-weight:500;}

/* ---------- contact ---------- */
.s-contact{
  margin:0 0 1rem;padding:1.3rem 1.4rem;
  border-radius:var(--radius);
  border:1px solid var(--line);
  background:linear-gradient(160deg, var(--frost-soft), rgba(255,255,255,.35));
}
.s-contact h3{
  margin:0 0 .8rem;
  font-family:"Noto Sans SC",sans-serif;font-size:1.05rem;font-weight:500;
}
.s-rows{display:flex;flex-wrap:wrap;gap:.6rem 2rem;}
.s-row{display:flex;align-items:center;gap:.55rem;font-size:.95rem;}
.s-row .lab{color:var(--mist);font-size:.84rem;min-width:3.2em;}
.s-row a, .s-row code{
  font-family:"Inter",ui-monospace,monospace;
  color:var(--ink);text-decoration:none;
  background:rgba(35,38,46,.05);
  padding:.18rem .5rem;border-radius:6px;font-size:.9rem;
}
.s-row a:hover{color:var(--frost);}

/* ---------- responsive ---------- */
@media (max-width:720px){
  .s-grid{grid-template-columns:1fr;}
  .s-hero{padding:2rem 1.3rem;}
  .s-seal{width:46px;height:46px;font-size:1.35rem;top:1.2rem;right:1.2rem;}
}

/* ---------- accessibility ---------- */
.s-home a:focus-visible{outline:2px solid var(--frost);outline-offset:3px;border-radius:6px;}
@media (prefers-reduced-motion:reduce){
  .s-home > *{animation:none;}
  .s-hero::before{animation:none;}
  .s-actions a,.s-card{transition:none;}
}
</style>

<div class="s-home" markdown="0">

  <header class="s-hero">
    <p class="s-eyebrow">papers · essays · records · projects</p>
    <h1>Hi, This is S. Chow</h1>
    <p>
      写一点代码，也写一点诗。<br>
      这里放我的文章、项目和一些长期记录。
    </p>
    <nav class="s-actions">
      <a class="primary" href="{{ '/cv/' | relative_url }}">个人简介</a>
      <a href="{{ '/portfolio/' | relative_url }}">往期回顾</a>
      <a href="/physicscources/">物理资源</a>
    </nav>
  </header>

  <section class="s-poem">
    <span class="s-seal">石</span>
    <blockquote>
      你在瓦尔登湖的水面上泛舟<br>
      我在寒冷窗花的木屋里写诗<br>
      冬天把梭罗摆在荷马的面前<br>
      冻碎了一地的象形文字
    </blockquote>
    <div class="s-date">— 令和七年十二月</div>
  </section>

  <p class="s-kicker">你可以从这里开始逛</p>
  <div class="s-grid">
    <a class="s-card" href="{{ '/cv/' | relative_url }}">
      <span class="ico">👤</span>
      <span class="t">个人简介</span>
      <span class="s">about / cv</span>
      <span class="go">前往 →</span>
    </a>
    <a class="s-card" href="{{ '/portfolio/' | relative_url }}">
      <span class="ico">🗂️</span>
      <span class="t">往期回顾</span>
      <span class="s">portfolio</span>
      <span class="go">前往 →</span>
    </a>
    <a class="s-card" href="/physicscources/">
      <span class="ico">⚛️</span>
      <span class="t">物理资源</span>
      <span class="s">physics notes</span>
      <span class="go">前往 →</span>
    </a>
  </div>

  <section class="s-contact">
    <h3>✉️ 联系我</h3>
    <div class="s-rows">
      <div class="s-row">
        <span class="lab">微信</span>
        <code>Shssip22233315779</code>
      </div>
      <div class="s-row">
        <span class="lab">邮箱</span>
        <a href="mailto:sunnystone2007@gmail.com">sunnystone2007@gmail.com</a>
      </div>
    </div>
  </section>

</div>
