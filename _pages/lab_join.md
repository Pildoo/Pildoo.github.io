---
layout: page
permalink: /lab/join/
title: join the lab
nav: false
nav_order: 7
description: How to join the Social Connections & Health Lab at Hanyang University as a doctoral, master's, or undergraduate research student.
---

<style>
  .post-header {
    display: none;
  }

  .lab-page {
    --lab-muted: color-mix(in srgb, var(--global-text-color) 68%, transparent);
    --lab-border: color-mix(in srgb, var(--global-text-color) 13%, transparent);
    --lab-soft: color-mix(in srgb, var(--global-theme-color) 6%, var(--global-bg-color));
    --lab-card: color-mix(in srgb, var(--global-text-color) 2.5%, var(--global-bg-color));
  }

  .lab-hero {
    position: relative;
    overflow: hidden;
    margin-bottom: 3rem;
    padding: clamp(2rem, 6vw, 3.5rem);
    border: 1px solid color-mix(in srgb, var(--global-theme-color) 18%, transparent);
    border-radius: 1.25rem;
    background:
      radial-gradient(circle at 92% 8%, color-mix(in srgb, var(--global-theme-color) 15%, transparent) 0, transparent 34%),
      linear-gradient(145deg, color-mix(in srgb, var(--global-theme-color) 8%, var(--global-bg-color)), var(--global-bg-color) 72%);
  }

  .lab-hero::before {
    position: absolute;
    top: 1.25rem;
    left: 1.25rem;
    width: 2.5rem;
    height: 0.2rem;
    border-radius: 999px;
    background: var(--global-theme-color);
    content: '';
  }

  .lab-eyebrow {
    display: block;
    margin-bottom: 0.9rem;
    color: var(--global-theme-color);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .lab-eyebrow a {
    color: inherit;
    text-decoration: none;
  }

  .lab-eyebrow a:hover {
    color: var(--global-theme-color);
    text-decoration: underline;
  }

  .lab-hero h1 {
    max-width: 780px;
    margin: 0 0 0.5rem;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(2.2rem, 6.4vw, 4rem);
    font-weight: 500;
    letter-spacing: -0.045em;
    line-height: 1.02;
  }

  .lab-hero-ko {
    margin: 0 0 1.4rem;
    color: var(--lab-muted);
    font-size: clamp(1rem, 2.4vw, 1.15rem);
    letter-spacing: -0.01em;
  }

  .lab-hero-lead {
    max-width: 660px;
    margin: 0;
    font-size: clamp(1.02rem, 2vw, 1.16rem);
    line-height: 1.7;
  }

  .lab-ko {
    display: block;
    color: var(--lab-muted);
    font-size: 0.88rem;
    line-height: 1.7;
    word-break: keep-all;
  }

  .lab-hero-lead .lab-ko {
    margin-top: 0.6rem;
  }

  .lab-actions {
    display: flex;
    flex-wrap: wrap;
    gap: 0.55rem;
    margin-top: 1.8rem;
  }

  .lab-button {
    display: inline-flex;
    align-items: center;
    min-height: 2.65rem;
    padding: 0.55rem 1rem;
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

  .lab-button--primary {
    background: var(--global-theme-color);
    color: var(--global-bg-color);
  }

  .lab-button:hover {
    background: var(--global-theme-color);
    color: var(--global-bg-color);
    text-decoration: none;
    transform: translateY(-1px);
  }

  .lab-section {
    margin-top: 3.75rem;
    scroll-margin-top: 6rem;
  }

  .lab-section-heading {
    display: grid;
    grid-template-columns: 8rem minmax(0, 1fr);
    gap: 1.5rem;
    align-items: baseline;
    margin-bottom: 1.5rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid var(--lab-border);
  }

  .lab-kicker {
    color: var(--global-theme-color);
    font-size: 0.72rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .lab-section-heading h2 {
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(1.6rem, 3.6vw, 2.15rem);
    font-weight: 500;
    letter-spacing: -0.025em;
    line-height: 1.15;
  }

  .lab-section-heading .lab-ko {
    margin-top: 0.35rem;
    font-size: 0.92rem;
  }

  .lab-copy {
    max-width: 730px;
    margin: 0 0 1.75rem 9.5rem;
    color: var(--lab-muted);
    line-height: 1.75;
  }

  .lab-copy .lab-ko {
    margin-top: 0.7rem;
    padding-top: 0.7rem;
    border-top: 1px solid var(--lab-border);
    font-size: 0.86rem;
  }

  .lab-track-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  }

  .lab-track,
  .lab-panel {
    padding: clamp(1.25rem, 3vw, 1.5rem);
    border: 1px solid var(--lab-border);
    border-radius: 0.9rem;
    background: var(--lab-card);
    box-shadow: 0 10px 30px color-mix(in srgb, var(--global-text-color) 4%, transparent);
  }

  .lab-track-label {
    display: block;
    margin-bottom: 0.6rem;
    color: var(--global-theme-color);
    font-size: 0.68rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
  }

  .lab-track h3,
  .lab-panel h3 {
    margin: 0 0 0.55rem;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: 1.08rem;
    font-weight: 600;
  }

  .lab-track h3 .lab-ko {
    margin-top: 0.1rem;
    font-family: inherit;
    font-size: 0.82rem;
    font-weight: 400;
  }

  .lab-track p {
    margin: 0 0 0.9rem;
    color: var(--lab-muted);
    font-size: 0.9rem;
    line-height: 1.65;
  }

  .lab-track p:last-child {
    margin-bottom: 0;
  }

  .lab-track-note {
    margin: 0;
    padding-top: 0.85rem;
    border-top: 1px solid var(--lab-border);
    color: var(--lab-muted);
    font-size: 0.82rem;
    line-height: 1.6;
  }

  .lab-panel-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
  }

  .lab-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .lab-list li + li {
    margin-top: 0.75rem;
    padding-top: 0.75rem;
    border-top: 1px solid var(--lab-border);
  }

  .lab-list strong {
    display: block;
    font-size: 0.9rem;
    font-weight: 600;
  }

  .lab-list span {
    display: block;
    margin-top: 0.15rem;
    color: var(--lab-muted);
    font-size: 0.82rem;
    line-height: 1.55;
  }

  .lab-steps {
    counter-reset: lab-step;
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .lab-steps > li {
    position: relative;
    padding: 0 0 1.4rem 3.25rem;
  }

  .lab-steps > li::before {
    position: absolute;
    top: 0;
    left: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 2.1rem;
    height: 2.1rem;
    border-radius: 50%;
    background: var(--lab-soft);
    color: var(--global-theme-color);
    font-family: Georgia, 'Times New Roman', serif;
    font-size: 0.84rem;
    counter-increment: lab-step;
    content: counter(lab-step, decimal-leading-zero);
  }

  .lab-steps > li:not(:last-child)::after {
    position: absolute;
    top: 2.4rem;
    bottom: 0.4rem;
    left: 1.05rem;
    width: 1px;
    background: var(--lab-border);
    content: '';
  }

  .lab-steps h3 {
    margin: 0.25rem 0 0.4rem;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: 1.05rem;
    font-weight: 600;
  }

  .lab-steps p {
    margin: 0;
    color: var(--lab-muted);
    font-size: 0.92rem;
    line-height: 1.7;
  }

  .lab-steps ul {
    margin: 0.6rem 0 0;
    padding-left: 1.1rem;
    color: var(--lab-muted);
    font-size: 0.9rem;
    line-height: 1.7;
  }

  .lab-note {
    margin-top: 1.5rem;
    padding: 1.1rem 1.25rem;
    border-left: 3px solid var(--global-theme-color);
    border-radius: 0 0.6rem 0.6rem 0;
    background: var(--lab-soft);
  }

  .lab-note p {
    margin: 0;
    font-size: 0.92rem;
    line-height: 1.7;
  }

  .lab-note p + p {
    margin-top: 0.6rem;
  }

  .lab-cta {
    display: flex;
    gap: 1.5rem;
    align-items: center;
    justify-content: space-between;
    margin-top: 3.75rem;
    padding: clamp(1.4rem, 4vw, 2rem);
    border-radius: 0.9rem;
    background: var(--lab-soft);
  }

  .lab-cta p {
    max-width: 570px;
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(1.08rem, 2.5vw, 1.3rem);
    line-height: 1.5;
  }

  .lab-cta-actions {
    display: flex;
    flex-shrink: 0;
    gap: 0.55rem;
  }

  @media (max-width: 860px) {
    .lab-track-grid,
    .lab-panel-grid {
      grid-template-columns: 1fr;
    }
  }

  @media (max-width: 760px) {
    .lab-section-heading {
      grid-template-columns: 1fr;
      gap: 0.5rem;
    }

    .lab-copy {
      margin-left: 0;
    }

    .lab-cta {
      align-items: flex-start;
      flex-direction: column;
    }
  }

  @media (max-width: 560px) {
    .lab-hero {
      border-radius: 0.9rem;
    }

    .lab-cta-actions {
      flex-wrap: wrap;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    .lab-button {
      transition: none;
    }
  }
</style>

<div class="lab-page">
  <header class="lab-hero">
    <span class="lab-eyebrow"><a href="{{ '/lab/' | relative_url }}">Social Connections &amp; Health Lab</a></span>
    <h1>Join the lab</h1>
    <p class="lab-hero-ko" lang="ko">대학원생·학부연구생 모집 안내</p>
    <p class="lab-hero-lead">
      The lab studies aging, health, and social relationships with Korean panel and whole-community network data. We are looking for students who want
      to learn how to turn a real question about later life into evidence.
      <span class="lab-ko" lang="ko"
        >본 연구실은 국내 패널자료와 완전연결망 자료로 노화·건강·사회적 관계를 연구합니다. 노년기에 대한 실제 질문을 근거 있는 분석으로 바꾸는 법을
        배우고자 하는 학생을 찾습니다.</span
      >
    </p>
    <div class="lab-actions">
      <a class="lab-button lab-button--primary" href="#apply">How to apply · 지원 방법</a>
      <a class="lab-button" href="{{ '/lab/' | relative_url }}">About the lab</a>
    </div>
  </header>

  <section id="who" class="lab-section" aria-labelledby="lab-who-title">
    <div class="lab-section-heading">
      <span class="lab-kicker">Who we look for</span>
      <div>
        <h2 id="lab-who-title">Three ways to join</h2>
        <span class="lab-ko" lang="ko">지원 경로</span>
      </div>
    </div>
    <p class="lab-copy">
      Students come to the lab from sociology, but also from public health, social welfare, gerontology, and statistics. What matters is a real
      question you care about and the willingness to learn the methods it takes to answer it.
      <span class="lab-ko" lang="ko"
        >사회학뿐 아니라 보건학, 사회복지학, 노년학, 통계학 배경의 학생도 함께합니다. 중요한 것은 스스로 관심 있는 질문과, 그 질문에 답하기 위한 방법을
        배우려는 자세입니다.</span
      >
    </p>

    <div class="lab-track-grid">
      <article class="lab-track">
        <span class="lab-track-label">Doctoral</span>
        <h3 lang="ko">박사과정</h3>
        <p>
          Doctoral members develop an independent line of work inside the lab's program—framing a question, designing the analysis, and carrying it
          through to publication—while contributing to ongoing projects.
        </p>
        <p class="lab-track-note" lang="ko">
          연구실의 연구 프로그램 안에서 독립적인 연구 주제를 발전시키고, 진행 중인 과제에도 함께 참여합니다.
        </p>
      </article>

      <article class="lab-track">
        <span class="lab-track-label">Master's</span>
        <h3 lang="ko">석사과정</h3>
        <p>
          Master's members build a working foundation in panel and network analysis, take part in an ongoing project, and write a thesis on a question
          of their own.
        </p>
        <p class="lab-track-note" lang="ko">패널·연결망 분석의 기초를 다지면서 진행 중인 연구에 참여하고, 자신의 주제로 학위논문을 씁니다.</p>
      </article>

      <article class="lab-track">
        <span class="lab-track-label">Undergraduate</span>
        <h3 lang="ko">학부 연구생</h3>
        <p>
          Undergraduates join for a semester or longer to learn data cleaning, measurement, and basic analysis by working alongside graduate members.
          It is a good way to find out whether research suits you before applying to graduate school.
        </p>
        <p class="lab-track-note" lang="ko">
          한 학기 이상 참여하며 자료 정리와 기초 분석을 배웁니다. 대학원 진학 전에 연구가 자신에게 맞는지 확인해 볼 수 있는 기회입니다.
        </p>
      </article>
    </div>

  </section>

  <section id="preparation" class="lab-section" aria-labelledby="lab-preparation-title">
    <div class="lab-section-heading">
      <span class="lab-kicker">Preparation</span>
      <div>
        <h2 id="lab-preparation-title">What helps before you start</h2>
        <span class="lab-ko" lang="ko">준비하면 좋은 것</span>
      </div>
    </div>
    <p class="lab-copy">
      None of this is a prerequisite—members learn most of it in the lab. It is a map of where you will end up, not a gate you have to pass first.
      <span class="lab-ko" lang="ko">아래 항목은 필수 자격 요건이 아니라 연구실에서 함께 익혀 가는 내용입니다.</span>
    </p>

    <div class="lab-panel-grid">
      <article class="lab-panel">
        <h3>Coursework<span class="lab-ko" lang="ko">수강하면 좋은 과목</span></h3>
        <ul class="lab-list">
          <li>
            <strong>Social Networks and Social Capital (SOC9115)</strong>
            <span>Graduate seminar covering the network concepts the lab's projects are built on.</span>
          </li>
          <li>
            <strong>Medical Sociology Seminar (SOC9116)</strong>
            <span>Graduate seminar on the social determinants of health and illness.</span>
          </li>
          <li>
            <strong>Intermediate Social Statistics (SOC9109)</strong>
            <span>Regression and the statistical grounding the lab's longitudinal models assume.</span>
          </li>
        </ul>
      </article>

      <article class="lab-panel">
        <h3>Skills<span class="lab-ko" lang="ko">익혀 두면 좋은 기술</span></h3>
        <ul class="lab-list">
          <li>
            <strong>One statistical package, reasonably well</strong>
            <span>Stata or R is enough to begin; the lab uses both, plus Mplus for latent variable models.</span>
          </li>
          <li>
            <strong>Reading empirical articles closely</strong>
            <span>Being able to follow how a paper moves from a question to a design to a table matters more than knowing every technique.</span>
          </li>
          <li>
            <strong>English academic reading and writing</strong>
            <span>The lab publishes in international journals, so most reading and writing is in English.</span>
          </li>
        </ul>
      </article>
    </div>

  </section>

  <section id="apply" class="lab-section" aria-labelledby="lab-apply-title">
    <div class="lab-section-heading">
      <span class="lab-kicker">How to apply</span>
      <div>
        <h2 id="lab-apply-title">Getting in touch</h2>
        <span class="lab-ko" lang="ko">지원 방법</span>
      </div>
    </div>
    <p class="lab-copy">
      Graduate admission runs through the Department of Sociology's regular admissions cycle, but the conversation should start earlier. Email before
      you apply so we can talk about whether your questions and the lab's work fit each other.
      <span class="lab-ko" lang="ko"
        >대학원 입학은 사회학과의 정규 입학 전형을 따르지만, 그 전에 먼저 이메일로 연락 주시기를 권합니다. 관심 주제와 연구실의 연구가 서로 맞는지 미리
        이야기해 보는 편이 좋습니다.</span
      >
    </p>

    <ol class="lab-steps">
      <li>
        <h3>Write to Pildoo Sung</h3>
        <p>
          Send an email to <a href="mailto:pildoosung@hanyang.ac.kr">pildoosung@hanyang.ac.kr</a> with "Lab inquiry" and your intended track (doctoral,
          master's, or undergraduate research) in the subject line.
        </p>
      </li>
      <li>
        <h3>Include four things</h3>
        <ul>
          <li>A short statement—two or three paragraphs—on what you want to study and why this lab.</li>
          <li>Your CV or résumé.</li>
          <li>A transcript, with statistics and methods courses noted.</li>
          <li>Optionally, a writing sample: a thesis, term paper, or research report.</li>
        </ul>
      </li>
      <li>
        <h3>Talk it through</h3>
        <p>
          If there is a good fit, we will meet—in person or online—to discuss possible questions, data, and what the next year or two would actually
          look like.
        </p>
      </li>
      <li>
        <h3>Apply to the department</h3>
        <p>
          Formal admission is decided by the graduate program, not the lab. Check the
          <a href="https://socio.hanyang.ac.kr/home">Department of Sociology</a> for the current cycle, required documents, and deadlines.
        </p>
      </li>
    </ol>

    <div class="lab-note">
      <p>
        <strong>On funding and research assistantships.</strong> Whether funded positions are open depends on the projects running at the time. Ask in
        your first email and you will get a straight answer.
      </p>
      <p lang="ko">
        연구비 지원과 연구보조원(RA) 자리는 그 시점에 진행 중인 과제에 따라 달라집니다. 첫 이메일에서 함께 문의해 주시면 솔직하게 답변드리겠습니다.
      </p>
    </div>

  </section>

  <aside class="lab-cta" aria-label="Contact the lab">
    <p>Not sure whether your question fits? Write anyway—that is usually the fastest way to find out.</p>
    <div class="lab-cta-actions">
      <a class="lab-button lab-button--primary" href="mailto:pildoosung@hanyang.ac.kr">Email the lab</a>
      <a class="lab-button" href="{{ '/research/' | relative_url }}">Research program</a>
    </div>
  </aside>
</div>
