---
layout: page
permalink: /research/
title: research
nav: true
nav_order: 2
description: How social relationships shape health and well-being in later life—and how later-life transitions reshape those relationships in return.
---

<style>
  .post-header {
    position: relative;
    overflow: hidden;
    margin-bottom: 2.5rem;
    padding: clamp(2rem, 6vw, 4rem);
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 18%, transparent);
    border-radius: 1.25rem;
    background:
      radial-gradient(
        circle at 92% 8%,
        color-mix(in srgb, var(--global-theme-color) 15%, transparent) 0,
        transparent 34%
      ),
      linear-gradient(
        145deg,
        color-mix(in srgb, var(--global-theme-color) 8%, var(--global-bg-color)),
        var(--global-bg-color) 72%
      );
  }

  .post-header::before {
    position: absolute;
    top: 1.25rem;
    left: 1.25rem;
    width: 2.5rem;
    height: 0.2rem;
    border-radius: 999px;
    background: var(--global-theme-color);
    content: '';
  }

  .post-header .post-title {
    max-width: 720px;
    margin: 0 0 0.85rem;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(2.5rem, 7vw, 4.6rem);
    font-weight: 500;
    letter-spacing: -0.045em;
    line-height: 1;
  }

  .post-header .post-description {
    max-width: 700px;
    margin: 0;
    color: color-mix(in srgb, var(--global-text-color) 74%, transparent);
    font-size: clamp(1.02rem, 2vw, 1.18rem);
    line-height: 1.65;
  }

  .research-page {
    --research-muted: color-mix(in srgb, var(--global-text-color) 68%, transparent);
    --research-border: color-mix(in srgb, var(--global-text-color) 13%, transparent);
    --research-soft: color-mix(in srgb, var(--global-theme-color) 6%, var(--global-bg-color));
    --research-card: color-mix(in srgb, var(--global-text-color) 2.5%, var(--global-bg-color));
  }

  .research-lead {
    display: grid;
    grid-template-columns: minmax(0, 1.5fr) minmax(220px, 0.8fr);
    gap: 2rem;
    align-items: start;
    margin-bottom: 4rem;
  }

  .research-lead > p {
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(1.25rem, 2.6vw, 1.62rem);
    line-height: 1.55;
  }

  .research-jump {
    display: flex;
    flex-direction: column;
    gap: 0.55rem;
    padding-left: 1.25rem;
    border-left: 1px solid var(--research-border);
  }

  .research-jump span {
    margin-bottom: 0.15rem;
    color: var(--research-muted);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .research-jump a {
    width: fit-content;
    color: var(--global-text-color);
    font-size: 0.92rem;
    font-weight: 500;
    text-decoration: none;
  }

  .research-jump a::after {
    margin-left: 0.35rem;
    color: var(--global-theme-color);
    content: '↓';
  }

  .research-jump a:hover {
    color: var(--global-theme-color);
    text-decoration: none;
  }

  .research-section {
    margin-top: 4rem;
    scroll-margin-top: 6rem;
  }

  .research-section:first-of-type {
    margin-top: 0;
  }

  .section-heading {
    display: grid;
    grid-template-columns: 8rem minmax(0, 1fr);
    gap: 1.5rem;
    align-items: baseline;
    margin-bottom: 1.5rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--research-border);
  }

  .section-kicker {
    color: var(--global-theme-color);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .section-heading h2 {
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(1.7rem, 4vw, 2.35rem);
    font-weight: 500;
    letter-spacing: -0.025em;
    line-height: 1.15;
  }

  .section-copy {
    max-width: 730px;
    margin: 0 0 1.75rem 9.5rem;
    color: var(--research-muted);
    line-height: 1.75;
  }

  .research-facts {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1px;
    overflow: hidden;
    margin-bottom: 1.25rem;
    border: 1px solid var(--research-border);
    border-radius: 0.9rem;
    background: var(--research-border);
  }

  .research-fact {
    padding: 1rem 1.1rem;
    background: var(--global-bg-color);
  }

  .research-fact span {
    display: block;
    margin-bottom: 0.25rem;
    color: var(--research-muted);
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.09em;
    text-transform: uppercase;
  }

  .research-fact strong {
    font-family: Georgia, 'Times New Roman', serif;
    font-size: 0.98rem;
    font-weight: 500;
    line-height: 1.35;
  }

  .question-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }

  .question-card,
  .foundation-card {
    border: 1px solid var(--research-border);
    border-radius: 0.9rem;
    background: var(--research-card);
    box-shadow: 0 10px 30px color-mix(in srgb, var(--global-text-color) 4%, transparent);
  }

  .question-card {
    display: grid;
    grid-template-columns: 2.25rem minmax(0, 1fr);
    gap: 0.8rem;
    padding: 1.25rem;
  }

  .question-card:last-child {
    grid-column: 1 / -1;
  }

  .question-number {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 2.1rem;
    height: 2.1rem;
    border-radius: 50%;
    background: var(--research-soft);
    color: var(--global-theme-color);
    font-family: Georgia, 'Times New Roman', serif;
    font-size: 0.84rem;
  }

  .question-card h3,
  .foundation-card h3 {
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-weight: 600;
    line-height: 1.3;
  }

  .question-card h3 {
    font-size: 1.08rem;
  }

  .question-card p {
    margin: 0.45rem 0 0;
    color: var(--research-muted);
    font-size: 0.92rem;
    line-height: 1.65;
  }

  .foundation-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }

  .foundation-card {
    display: flex;
    flex-direction: column;
    padding: clamp(1.25rem, 3vw, 1.6rem);
  }

  .foundation-label {
    margin-bottom: 0.65rem;
    color: var(--global-theme-color);
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .foundation-card h3 {
    font-size: 1.25rem;
  }

  .foundation-summary {
    margin: 0.75rem 0 1.25rem;
    color: var(--research-muted);
    font-size: 0.92rem;
    line-height: 1.65;
  }

  .publication-list {
    margin: auto 0 0;
    padding: 1rem 0 0;
    border-top: 1px solid var(--research-border);
    list-style: none;
  }

  .publication-list li + li {
    margin-top: 0.8rem;
  }

  .publication-list a {
    display: inline;
    color: var(--global-text-color);
    font-size: 0.88rem;
    font-weight: 600;
    line-height: 1.45;
    text-decoration-color: color-mix(in srgb, var(--global-theme-color) 35%, transparent);
    text-underline-offset: 0.2em;
  }

  .publication-list a:hover {
    color: var(--global-theme-color);
  }

  .publication-meta {
    display: block;
    margin-top: 0.15rem;
    color: var(--research-muted);
    font-size: 0.78rem;
    line-height: 1.4;
  }

  .research-cta {
    display: flex;
    gap: 1.5rem;
    align-items: center;
    justify-content: space-between;
    margin-top: 4rem;
    padding: clamp(1.4rem, 4vw, 2rem);
    border-radius: 0.9rem;
    background: var(--research-soft);
  }

  .research-cta p {
    max-width: 570px;
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(1.08rem, 2.5vw, 1.3rem);
    line-height: 1.5;
  }

  .research-actions {
    display: flex;
    flex-shrink: 0;
    gap: 0.55rem;
  }

  .research-button {
    display: inline-flex;
    align-items: center;
    min-height: 2.65rem;
    padding: 0.55rem 0.9rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 999px;
    color: var(--global-theme-color);
    font-size: 0.84rem;
    font-weight: 600;
    text-decoration: none;
    transition:
      background-color 160ms ease,
      color 160ms ease,
      transform 160ms ease;
  }

  .research-button:first-child {
    background: var(--global-theme-color);
    color: var(--global-bg-color);
  }

  .research-button:hover {
    background: var(--global-theme-color);
    color: var(--global-bg-color);
    text-decoration: none;
    transform: translateY(-1px);
  }

  @media (max-width: 760px) {
    .research-lead,
    .section-heading {
      grid-template-columns: 1fr;
      gap: 0.75rem;
    }

    .research-jump {
      flex-flow: row wrap;
      gap: 0.5rem 1rem;
      padding: 1rem 0 0;
      border-top: 1px solid var(--research-border);
      border-left: 0;
    }

    .research-jump span {
      flex-basis: 100%;
    }

    .section-copy {
      margin-left: 0;
    }

    .foundation-grid {
      grid-template-columns: 1fr;
    }

    .research-cta {
      align-items: flex-start;
      flex-direction: column;
    }
  }

  @media (max-width: 560px) {
    .post-header {
      border-radius: 0.9rem;
    }

    .research-lead {
      margin-bottom: 3rem;
    }

    .research-facts,
    .question-grid {
      grid-template-columns: 1fr;
    }

    .research-fact + .research-fact {
      border-top: 1px solid var(--research-border);
    }

    .question-card:last-child {
      grid-column: auto;
    }

    .research-actions {
      flex-wrap: wrap;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .research-button {
      transition: none;
    }
  }
</style>

<div class="research-page">
  <div class="research-lead">
    <p>
      I study social relationships as both a source and an outcome of health in later life. My work centers on older adults in South Korea and
      Singapore and combines social network measures with latent class and transition models, dyadic designs, and longitudinal analysis.
    </p>
    <nav class="research-jump" aria-label="Research page sections">
      <span>On this page</span>
      <a href="#current-program">Current program</a>
      <a href="#published-foundations">Published foundations</a>
    </nav>
  </div>

  <section id="current-program" class="research-section" aria-labelledby="current-program-title">
    <div class="section-heading">
      <span class="section-kicker">Current program</span>
      <h2 id="current-program-title">Sociocentric network analysis</h2>
    </div>
    <p class="section-copy">
      My current projects use complete community network data that repeatedly record who names whom among older residents of rural Korean townships.
      Observing everyone in the community makes it possible to distinguish the ties people report from the nominations they receive—something
      egocentric surveys cannot do.
    </p>

    <div class="research-facts" aria-label="Current research at a glance">
      <div class="research-fact">
        <span>Setting</span>
        <strong>Rural Korean townships</strong>
      </div>
      <div class="research-fact">
        <span>Design</span>
        <strong>Whole-community panels</strong>
      </div>
      <div class="research-fact">
        <span>Key distinction</span>
        <strong>Sent and received ties</strong>
      </div>
    </div>

    <div class="question-grid">
      <article class="question-card">
        <span class="question-number" aria-hidden="true">01</span>
        <div>
          <h3>Being chosen and loneliness</h3>
          <p>
            Do nominations older adults receive—especially from non-kin—protect against later loneliness beyond the ties they name themselves, and
            does that differ in advanced old age?
          </p>
        </div>
      </article>

      <article class="question-card">
        <span class="question-number" aria-hidden="true">02</span>
        <div>
          <h3>Selection or influence</h3>
          <p>
            When does similarity between connected villagers reflect choosing similar others, and when does it reflect influence as networks and
            behavior co-evolve?
          </p>
        </div>
      </article>

      <article class="question-card">
        <span class="question-number" aria-hidden="true">03</span>
        <div>
          <h3>From teeth to ties</h3>
          <p>How does tooth loss change the discussion nominations older adults receive, and what does that mean for later cognitive function?</p>
        </div>
      </article>

      <article class="question-card">
        <span class="question-number" aria-hidden="true">04</span>
        <div>
          <h3>Network trajectories</h3>
          <p>How do received and sent ties change across survey waves, and how are those long-run trajectories linked to cognitive aging?</p>
        </div>
      </article>

      <article class="question-card">
        <span class="question-number" aria-hidden="true">05</span>
        <div>
          <h3>Cultural holes</h3>
          <p>
            What does it mean for well-being when older adults bridge culturally dissimilar people who are not otherwise connected? This project
            develops culturally weighted measures of brokerage to find out.
          </p>
        </div>
      </article>
    </div>
  </section>

  <section id="published-foundations" class="research-section" aria-labelledby="published-foundations-title">
    <div class="section-heading">
      <span class="section-kicker">Published work</span>
      <h2 id="published-foundations-title">Four foundations</h2>
    </div>
    <p class="section-copy">The current program grows from four connected lines of research on networks, health, caregiving, and social capital.</p>

    <div class="foundation-grid">
      <article class="foundation-card">
        <span class="foundation-label">Networks over time</span>
        <h3>Social network typology</h3>
        <p class="foundation-summary">
          I use latent class and transition analysis to identify older adults' network types and trace movement between them—after widowhood, during
          the pandemic, and over ordinary time—with consequences from depressive symptoms to mortality.
        </p>
        <ul class="publication-list" aria-label="Selected work on social network typology">
          <li>
            <a href="https://doi.org/10.1016/j.socnet.2025.12.005">Getting Lonely and Isolated?</a>
            <span class="publication-meta">Social Networks · 2026</span>
          </li>
          <li>
            <a href="https://doi.org/10.1002/psp.70231">Stability and Changes in Social Network Profiles After Widowhood</a>
            <span class="publication-meta">Population, Space and Place · 2026</span>
          </li>
          <li>
            <a href="https://doi.org/10.1016/j.socscimed.2021.114617">Transitions between Social Network Profiles and All-cause Mortality</a>
            <span class="publication-meta">Social Science &amp; Medicine · 2022</span>
          </li>
        </ul>
      </article>

      <article class="foundation-card">
        <span class="foundation-label">Reciprocal processes</span>
        <h3>Social engagement and health</h3>
        <p class="foundation-summary">
          This work treats engagement and health as processes that continually shape each other, spanning cognitive function, depressive symptoms,
          handgrip strength, oral health, multimorbidity, and healthcare needs.
        </p>
        <ul class="publication-list" aria-label="Selected work on social engagement and health">
          <li>
            <a href="https://doi.org/10.1111/ggi.70663">Multimorbidity Patterns, Healthcare Utilization, and Unmet Needs</a>
            <span class="publication-meta">Geriatrics &amp; Gerontology International · 2026</span>
          </li>
          <li>
            <a href="https://doi.org/10.1177/00220345261438375">Oral Health-Related Quality of Life and Social Engagement</a>
            <span class="publication-meta">Journal of Dental Research · 2026</span>
          </li>
          <li>
            <a href="https://doi.org/10.1002/gps.70085">Formal Social Engagement, Oral Health, and Depressive Symptoms</a>
            <span class="publication-meta">International Journal of Geriatric Psychiatry · 2025</span>
          </li>
          <li>
            <a href="https://doi.org/10.1159/000540344">Social Engagement and Handgrip Strength</a>
            <span class="publication-meta">Gerontology · 2024</span>
          </li>
        </ul>
      </article>

      <article class="foundation-card">
        <span class="foundation-label">Care in context</span>
        <h3>Family caregiving</h3>
        <p class="foundation-summary">
          Studies of families caring for older adults with cognitive impairment show that well-being depends on more than the amount of care:
          loneliness, task-sharing, mastery, and resilience all shape the caregiving experience.
        </p>
        <ul class="publication-list" aria-label="Selected work on family caregiving">
          <li>
            <a href="https://doi.org/10.1111/ggi.70499">Loneliness in Family Caregiver–Care Recipient Dyads</a>
            <span class="publication-meta">Geriatrics &amp; Gerontology International · 2026</span>
          </li>
          <li>
            <a href="https://doi.org/10.1093/geronb/gbae186">Sharing in Caring</a>
            <span class="publication-meta">The Journals of Gerontology, Series B · 2025</span>
          </li>
          <li>
            <a href="https://doi.org/10.1177/08982643241262374">Stress and Loneliness among Family Caregivers</a>
            <span class="publication-meta">Journal of Aging and Health · 2025</span>
          </li>
        </ul>
      </article>

      <article class="foundation-card">
        <span class="foundation-label">Comparative perspective</span>
        <h3>Trust and social capital</h3>
        <p class="foundation-summary">
          Cross-national research examines how generalized trust relates to social networks—especially weak ties—and the resources they carry,
          alongside comparative work on in-group trust and health in East Asia.
        </p>
        <ul class="publication-list" aria-label="Selected work on trust and social capital">
          <li>
            <a href="https://doi.org/10.1177/02685809241251770">Generalized Trust, Social Networks, and Social Resources across 30 Countries</a>
            <span class="publication-meta">International Sociology · 2024</span>
          </li>
          <li>
            <a href="https://doi.org/10.1177/0020715220937752">In-Group Trust and Self-Rated Health in East Asia</a>
            <span class="publication-meta">International Journal of Comparative Sociology · 2020</span>
          </li>
        </ul>
      </article>
    </div>
  </section>

  <aside class="research-cta" aria-label="Publications and collaboration">
    <p>Explore the full publication record, or get in touch about shared questions, data, and collaboration.</p>
    <div class="research-actions">
      <a class="research-button" href="{{ '/publications/' | relative_url }}">All publications</a>
      <a class="research-button" href="mailto:pildoosung@hanyang.ac.kr">Get in touch</a>
    </div>
  </aside>
</div>
