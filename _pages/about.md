---
layout: default
title: about
permalink: /
selected_papers: true
---


<script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Person",
    "@id": "{{ site.url }}/#person",
    "name": "Pildoo Sung",
    "url": "{{ site.url }}/",
    "jobTitle": "Associate Professor of Sociology",
    "affiliation": {
      "@type": "CollegeOrUniversity",
      "name": "Hanyang University",
      "url": "https://socio.hanyang.ac.kr/home"
    },
    "sameAs": [
      "https://github.com/Pildoo",
      "https://orcid.org/0000-0002-5730-6241",
      "https://scholar.google.com/citations?user=zJTtOhYAAAAJ",
      "https://socio.hanyang.ac.kr/home"
    ]
  }
</script>


<style>
  .pildoo-home {
    --pildoo-muted: color-mix(in srgb, var(--global-text-color) 68%, transparent);
    --pildoo-border: color-mix(in srgb, var(--global-text-color) 14%, transparent);
  }


  .pildoo-hero {
    max-width: 860px;
    margin: 0 auto;
    padding: 2.5rem 1rem 2.75rem;
    text-align: center;
  }


  .pildoo-avatar {
    display: block;
    width: 188px;
    height: 188px;
    margin: 0 auto 1.4rem;
    border: 4px solid var(--global-bg-color);
    border-radius: 50%;
    box-shadow:
      0 0 0 2px var(--global-theme-color),
      0 10px 30px rgba(0, 0, 0, 0.13);
    object-fit: cover;
  }


  .pildoo-hero h1 {
    margin: 0;
    font-family: Georgia, 'Times New Roman', serif;
    font-size: clamp(2.25rem, 5vw, 3.5rem);
    letter-spacing: -0.03em;
  }


  .pildoo-subtitle {
    margin: 0.65rem 0 0;
    color: var(--pildoo-muted);
    font-size: 1.05rem;
  }


  .pildoo-actions,
  .pildoo-nav,
  .pildoo-keywords {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.55rem;
  }


  .pildoo-actions {
    margin: 1.6rem 0 1.4rem;
  }


  .pildoo-social-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 2.9rem;
    height: 2.9rem;
    border-radius: 50%;
    color: var(--global-theme-color);
    font-size: 1.5rem;
    text-decoration: none;
    transition:
      background-color 160ms ease,
      color 160ms ease,
      transform 160ms ease;
  }


  .pildoo-social-link:hover {
    background: color-mix(in srgb, var(--global-theme-color) 10%, var(--global-bg-color));
    color: var(--global-theme-color);
    text-decoration: none;
    transform: translateY(-1px);
  }


  .pildoo-nav a,
  .pildoo-keyword {
    display: inline-flex;
    align-items: center;
    min-height: 2.35rem;
    padding: 0.42rem 0.85rem;
    border: 1px solid var(--pildoo-border);
    border-radius: 0.35rem;
    background: color-mix(in srgb, var(--global-theme-color) 5%, var(--global-bg-color));
    color: var(--global-text-color);
    font-size: 0.92rem;
    text-decoration: none;
    transition:
      border-color 160ms ease,
      color 160ms ease,
      transform 160ms ease;
