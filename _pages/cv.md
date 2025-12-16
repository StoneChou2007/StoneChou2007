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
  /* ===== Fancy CV styling (purely visual; content unchanged) ===== */
  :root{
    --cv-bg: #0b1020;
    --cv-card: rgba(255,255,255,.06);
    --cv-border: rgba(255,255,255,.12);
    --cv-text: rgba(255,255,255,.88);
    --cv-muted: rgba(255,255,255,.68);
    --cv-accent: #7c3aed;
    --cv-accent-2:#06b6d4;
    --cv-accent-3:#f59e0b;
    --cv-radius: 18px;
  }

  /* Page container */
  .cv-page{
    max-width: 980px;
    margin: 0 auto;
    padding: 1.25rem 1rem 2.5rem;
    color: var(--cv-text);
  }

  /* Soft background glow without touching theme */
  .cv-page::before{
    content:"";
    position: fixed;
    inset: -40vh -20vw;
    background:
      radial-gradient(closest-side, rgba(124,58,237,.20), transparent 60%),
      radial-gradient(closest-side, rgba(6,182,212,.16), transparent 62%),
      radial-gradient(closest-side, rgba(245,158,11,.10), transparent 64%);
    z-index: -1;
    pointer-events: none;
    filter: blur(2px);
  }

  /* Hero line (first paragraph) */
  .cv-page p:first-of-type{
    background: linear-gradient(90deg, rgba(124,58,237,.18), rgba(6,182,212,.14));
    border: 1px solid var(--cv-border);
    border-radius: var(--cv-radius);
    padding: .9rem 1rem;
    margin-top: .75rem;
    box-shadow: 0 10px 30px rgba(0,0,0,.18);
  }

  /* Headings */
  .cv-page h1, .cv-page h2{
    letter-spacing: .2px;
    margin-top: 1.35rem;
    margin-bottom: .65rem;
    line-height: 1.15;
  }

  .cv-page h1{
    font-size: 2rem;
    background: linear-gradient(90deg, var(--cv-accent), var(--cv-accent-2));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
  }

  .cv-page h2{
    font-size: 1.35rem;
    position: relative;
    padding-left: .85rem;
  }

  .cv-page h2::before{
    content:"";
    position:absolute;
    left: 0;
    top: .25rem;
    bottom: .25rem;
    width: 4px;
    border-radius: 999px;
    background: linear-gradient(180deg, var(--cv-accent), var(--cv-accent-2));
  }

  /* Section separators (uses existing markdown hr-like lines naturally) */
  .cv-page hr{
    border: none;
    height: 1px;
    background: linear-gradient(90deg, transparent, var(--cv-border), transparent);
    margin: 1rem 0;
  }

  /* Lists */
  .cv-page ul{
    padding-left: 1.15rem;
    margin: .25rem 0 1rem;
  }
  .cv-page li{
    margin: .35rem 0;
  }
  .cv-page li::marker{
    color: var(--cv-accent-2);
  }

  /* Make the CV link look like a pill button */
  .cv-page a{
    color: rgba(255,255,255,.92);
    text-decoration: none;
    border-bottom: 1px dashed rgba(255,255,255,.35);
    transition: transform .15s ease, background .15s ease, border-color .15s ease;
  }
  .cv-page a:hover{
    border-color: rgba(255,255,255,.75);
  }
  .cv-page a[href*="CV_FALL_2025.pdf"]{
    display: inline-block;
    padding: .45rem .75rem;
    border-radius: 999px;
    border: 1px solid rgba(255,255,255,.18);
    background: linear-gradient(90deg, rgba(124,58,237,.22), rgba(6,182,212,.18));
    box-shadow: 0 10px 24px rgba(0,0,0,.16);
    border-bottom: none;
  }
  .cv-page a[href*="CV_FALL_2025.pdf"]:hover{
    transform: translateY(-1px);
    background: linear-gradient(90deg, rgba(124,58,237,.30), rgba(6,182,212,.24));
  }

  /* Card-like blocks for each H2 section content */
  .cv-section{
    background: var(--cv-card);
    border: 1px solid var(--cv-border);
    border-radius: var(--cv-radius);
    padding: .95rem 1rem;
    box-shadow: 0 16px 40px rgba(0,0,0,.18);
    margin: .8rem 0 1.15rem;
  }

  /* Research items: make the first line pop a bit (still same text) */
  .cv-section strong{
    color: rgba(255,255,255,.95);
  }

  /* Quote styling for Teaching line */
  .cv-quote{
    margin: .25rem 0 0;
    padding: .75rem .9rem;
    border-left: 4px solid rgba(245,158,11,.75);
    background: rgba(245,158,11,.08);
    border-radius: 12px;
    color: rgba(255,255,255,.86);
  }

  /* Small polish on muted lines */
  .cv-muted{
    color: var(--cv-muted);
  }
</style>

<div class="cv-page">

Here is a much more detailed CV updated till Dec 2025:

- [research CV]({{ '/files/CV_FALL_2025.pdf' | relative_url }})

<div class="cv-section">

Education
-----

* B.S. in Stony Brook, Stony Brook University, 2024-2027
* B.S. in Xi'an, China. Xi'an Jiaotong University, 2023-2024
* High School in Suzhou, China. Suzhou High School, 2022-2023

</div>

<div class="cv-section">

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

</div>

<div class="cv-section">

Skills
-----
* Programming Skills: Mathematica, C++, Fortran, Python, LaTeX, Linux.

* Soccer (Physics department Chairman nominated best player in the physics department)

* Argentina Tengo(Vice President of Tengo Club in Stony Brook University)

*table tennis

</div>

<div class="cv-section">

Publications
-----

</div>

<div class="cv-section">

Talks
-----

</div>

<div class="cv-section">

Teaching
-----
<div class="cv-quote">Mr. Chow doesn't teach. Mr. Chow regards not teaching a perfection.</div>

</div>

<div class="cv-section">

Service and leadership
======
* Currently NNgroup member in Stony Brook University
<!-- this is my webpage using md, can you revise it in a much more fancy way? do not change the content at all . for example, change the color of words -->

</div>

</div>
