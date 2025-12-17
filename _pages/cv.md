---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
  /* ===== CV-only styling (scoped) ===== */
  .cv-page{
    --bg: rgba(255,255,255,.60);
    --card: rgba(255,255,255,.55);
    --border: rgba(15,23,42,.12);
    --text: rgba(15,23,42,.90);
    --muted: rgba(15,23,42,.65);
    --a1: #7c3aed;
    --a2: #06b6d4;
    --a3: #f59e0b;

    max-width: 980px;
    margin: 0 auto;
    padding: 1.1rem 1rem 2.5rem;
    color: var(--text);
  }

  @media (prefers-color-scheme: dark){
    .cv-page{
      --bg: rgba(2,6,23,.55);
      --card: rgba(255,255,255,.06);
      --border: rgba(255,255,255,.14);
      --text: rgba(255,255,255,.90);
      --muted: rgba(255,255,255,.68);
    }
  }

  .cv-page::before{
    content:"";
    position: fixed;
    inset: -40vh -25vw;
    background:
      radial-gradient(closest-side, rgba(124,58,237,.18), transparent 62%),
      radial-gradient(closest-side, rgba(6,182,212,.14), transparent 62%),
      radial-gradient(closest-side, rgba(245,158,11,.10), transparent 66%);
    pointer-events: none;
    z-index: -1;
    filter: blur(2px);
  }

  /* Intro box (first paragraph) */
  .cv-page p:first-of-type{
    background: linear-gradient(90deg, rgba(124,58,237,.12), rgba(6,182,212,.10));
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: .9rem 1rem;
    box-shadow: 0 14px 36px rgba(0,0,0,.12);
  }

  /* Headings */
  .cv-page h2{
    margin-top: 1.3rem;
    margin-bottom: .55rem;
    padding-left: .85rem;
    position: relative;
    letter-spacing: .2px;
  }
  .cv-page h2::before{
    content:"";
    position:absolute;
    left:0;
    top:.25rem;
    bottom:.25rem;
    width: 4px;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--a1), var(--a2));
  }

  /* The "======" setext heading becomes h1 in many renderers */
  .cv-page h1{
    margin-top: 1.5rem;
    margin-bottom: .6rem;
    font-size: 1.7rem;
    background: linear-gradient(90deg, var(--a1), var(--a2));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    letter-spacing: .2px;
  }

  /* Links */
  .cv-page a{
    color: var(--text);
    text-decoration: none;
    border-bottom: 1px dashed rgba(125,125,125,.55);
    transition: transform .15s ease, border-color .15s ease, background .15s ease;
  }
  .cv-page a:hover{ border-color: rgba(125,125,125,.9); }

  /* Make the PDF link look like a pill */
  .cv-page a[href*="CV_FALL_2025.pdf"]{
    display: inline-block;
    padding: .45rem .8rem;
    border-radius: 999px;
    border: 1px solid var(--border);
    background: linear-gradient(90deg, rgba(124,58,237,.18), rgba(6,182,212,.14));
    box-shadow: 0 12px 28px rgba(0,0,0,.10);
    border-bottom: none;
  }
  .cv-page a[href*="CV_FALL_2025.pdf"]:hover{
    transform: translateY(-1px);
    background: linear-gradient(90deg, rgba(124,58,237,.26), rgba(6,182,212,.20));
  }

  /* Lists */
  .cv-page ul{ margin: .25rem 0 1.05rem; padding-left: 1.15rem; }
  .cv-page li{ margin: .38rem 0; }
  .cv-page li::marker{ color: var(--a2); }
  .cv-page ul ul li::marker{ color: var(--a1); }

  /* Subtle section “card” effect without wrapping */
  .cv-page h2, .cv-page h1{
    scroll-margin-top: 90px;
  }
  .cv-page h2 + ul,
  .cv-page h2 + p,
  .cv-page h1 + ul,
  .cv-page h1 + p{
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: .85rem 1rem;
    box-shadow: 0 14px 34px rgba(0,0,0,.10);
  }

  /* Teaching quote */
  .cv-page .cv-quote{
    background: linear-gradient(90deg, rgba(245,158,11,.14), rgba(124,58,237,.10));
    border: 1px solid var(--border);
    border-left: 4px solid rgba(245,158,11,.85);
    border-radius: 18px;
    padding: .85rem 1rem;
    box-shadow: 0 14px 34px rgba(0,0,0,.10);
    color: var(--text);
  }
</style>

<div class="cv-page" markdown="1">

Here is a much more detailed CV updated till Dec 2025:

- [research CV]({{ '/files/CV_FALL_2025.pdf' | relative_url }})


Education
-----

* B.S. in Stony Brook, Stony Brook University, 2024-2027
* B.S. in Xi'an, China. Xi'an Jiaotong University, 2023-2024
* High School in Suzhou, China. Suzhou High School, 2022-2023

Research experience
-----
* Fall 2025: Atmospheric Neutrino Reconstruction in Time Projection Chamber
  * Stony Brook University
  * Supervisor: Changkee Jung and Ciro Riccio

* Fall 2024: DUNE FD3 Photon Detector Upgrade
  * Stony Brook University
  * Supervisor: Ciro Riccio

* Fall 2025: Quantum Many-Body Theory and Random Matrix Theory
  * Stony Brook University
  * Supervisor: Jacobus Verbaarschot

* Summer 2025:Cryogenic Test of Front-End Motherboards (FEMBs) for DUNE
  * Brookhaven National Laboratory
  * Shanshan Gao,Vladimir Tishchenko
  
Skills
-----
* Programming Skills: Mathematica, C++, Fortran, Python, LaTeX, Linux.

* Soccer (Physics department Chairman nominated best player in the physics department)
  
* Argentina Tengo(Vice President of Tengo Club in Stony Brook University)

*table tennis

Publications
-----

  
Talks
-----

  
Teaching
-----
<p class="cv-quote">Mr. Chow doesn't teach. Mr. Chow regards not teaching a perfection.</p>

  
Service and leadership
======
* Currently NNgroup member in Stony Brook University

</div>
