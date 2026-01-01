---
permalink: /
title: "S.Chow's Webpage"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
/* ===== Home Hero ===== */
.home-hero{
  max-width: 860px;
  margin: 0 auto 1.6rem auto;
  padding: 1.6rem 1.4rem;
  border-radius: 16px;
  background: linear-gradient(135deg, rgba(40,40,40,.06), rgba(40,40,40,.02));
  border: 1px solid rgba(0,0,0,.08);
}
.home-hero h1{
  margin: 0 0 .4rem 0;
  font-size: 2rem;
  letter-spacing: .2px;
}
.home-hero p{
  margin: .2rem 0 1rem 0;
  opacity: .85;
  line-height: 1.7;
}
.home-actions{
  display: flex;
  flex-wrap: wrap;
  gap: .6rem;
  margin-top: .8rem;
}
.home-actions a{
  display: inline-block;
  padding: .55rem .9rem;
  border-radius: 999px;
  border: 1px solid rgba(0,0,0,.16);
  text-decoration: none;
}
.home-actions a.primary{
  border-color: rgba(0,0,0,.12);
  background: rgba(0,0,0,.06);
}
.home-grid{
  max-width: 860px;
  margin: 0 auto 1.6rem auto;
  display: grid;
  grid-template-columns: repeat(2, minmax(0,1fr));
  gap: .9rem;
}
@media (max-width: 720px){
  .home-grid{ grid-template-columns: 1fr; }
}
/* ===== Poem Card ===== */
.poem-card{
  max-width: 860px;
  margin: 0 auto 1.2rem auto;
  padding: 1.2rem 1.3rem;
  border-radius: 16px;
  background: rgba(0,0,0,.03);
  border: 1px solid rgba(0,0,0,.08);
}
.poem{
  margin: 0;
  padding-left: 1rem;
  border-left: 4px solid rgba(0,0,0,.18);
  line-height: 2.0;
  font-size: 1.05rem;
}
.poem-footer{
  margin-top: .8rem;
  opacity: .7;
  font-size: .95rem;
  text-align: right;
}
.card{
  padding: 1rem 1.1rem;
  border-radius: 14px;
  border: 1px solid rgba(0,0,0,.08);
  background: rgba(255,255,255,.55);
}
.card h3{ margin: 0 0 .4rem 0; }
.card p{ margin: 0; line-height: 1.7; opacity: .85; }
</style>

<div class="home-hero" align="center">

<h1>你好，我是 S. Chow</h1>

<p>
写一点代码，也写一点诗。<br>
这里放我的文章、项目和一些长期记录。
</p>



</div>

<div class="poem-card">

<blockquote class="poem">
你在瓦尔登湖的水面上泛舟<br>
我在寒冷窗花的木屋里写诗<br>
冬天把梭罗摆在荷马的面前<br>
冻碎了一地的象形文字
</blockquote>
<div class="poem-footer">— 令和七年十二月</div>
</div>

<div class="home-grid">

<div class="card">

### ✉️ 联系我

- 微信：Shssip22233315779
  
- 邮箱：sunnystone2007@gmail.com
  

</div>

</div>

---

#### 你可以从这里开始逛
- 👉 [个人简介]({{ '/cv/' | relative_url }})
- 👉 [往期回顾]({{ '/portfolio/' | relative_url }})
- 👉 [物理资源](/physicscources/)
