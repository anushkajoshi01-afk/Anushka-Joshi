<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Anushka Joshi</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #0A0A0A;
    --text: #F0EDE8;
    --muted: #6A6560;
    --accent: #C8B8A2;
    --rule: #1E1C1A;
    --max: 760px;
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    font-weight: 300;
    font-size: 16px;
    line-height: 1.8;
    -webkit-font-smoothing: antialiased;
  }

  /* NAV */
  nav {
    position: fixed;
    top: 0; left: 0; right: 0;
    z-index: 100;
    padding: 28px 48px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: linear-gradient(to bottom, rgba(10,10,10,0.95) 60%, transparent);
  }

  .nav-name {
    font-family: 'DM Sans', sans-serif;
    font-weight: 400;
    font-size: 13px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--text);
    text-decoration: none;
  }

  .nav-links {
    display: flex;
    gap: 36px;
    list-style: none;
  }

  .nav-links a {
    font-size: 12px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--muted);
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .nav-links a:hover { color: var(--accent); }

  /* SECTIONS */
  section {
    max-width: var(--max);
    margin: 0 auto;
    padding: 140px 32px;
  }

  section + section {
    border-top: 1px solid var(--rule);
  }

  /* HERO */
  #hero {
    padding-top: 220px;
    padding-bottom: 160px;
  }

  .hero-label {
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 32px;
    opacity: 0;
    animation: fadeUp 0.8s ease 0.2s forwards;
  }

  .hero-headline {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(42px, 6vw, 68px);
    line-height: 1.1;
    letter-spacing: -0.01em;
    color: var(--text);
    margin-bottom: 28px;
    opacity: 0;
    animation: fadeUp 0.9s ease 0.4s forwards;
  }

  .hero-sub {
    font-size: 16px;
    color: var(--muted);
    max-width: 460px;
    line-height: 1.7;
    opacity: 0;
    animation: fadeUp 0.9s ease 0.6s forwards;
  }

  .hero-tags {
    margin-top: 48px;
    display: flex;
    gap: 24px;
    flex-wrap: wrap;
    opacity: 0;
    animation: fadeUp 0.9s ease 0.8s forwards;
  }

  .tag {
    font-size: 11px;
    letter-spacing: 0.16em;
    text-transform: uppercase;
    color: var(--accent);
  }

  .tag-sep { color: var(--rule); }

  /* ABOUT */
  .section-label {
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 40px;
  }

  .about-text {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(22px, 3vw, 28px);
    line-height: 1.65;
    color: var(--text);
  }

  /* CAPABILITIES */
  .cap-intro {
    font-size: 14px;
    color: var(--muted);
    margin-bottom: 64px;
    letter-spacing: 0.02em;
  }

  .cap-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 56px 64px;
  }

  .cap-item-title {
    font-family: 'DM Sans', sans-serif;
    font-weight: 500;
    font-size: 15px;
    color: var(--text);
    margin-bottom: 10px;
    letter-spacing: 0.01em;
  }

  .cap-item-desc {
    font-size: 14px;
    color: var(--muted);
    line-height: 1.75;
  }

  /* CASE STUDIES */
  .cs-section-label {
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 80px;
  }

  .case-study {
    margin-bottom: 96px;
    padding-bottom: 96px;
    border-bottom: 1px solid var(--rule);
  }

  .case-study:last-child {
    border-bottom: none;
    margin-bottom: 0;
    padding-bottom: 0;
  }

  .cs-meta {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    margin-bottom: 28px;
    flex-wrap: wrap;
    gap: 8px;
  }

  .cs-number {
    font-size: 11px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--muted);
  }

  .cs-tag {
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--accent);
  }

  .cs-title {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(28px, 4vw, 40px);
    line-height: 1.2;
    color: var(--text);
    margin-bottom: 12px;
  }

  .cs-collab {
    font-size: 13px;
    color: var(--muted);
    font-style: italic;
    margin-bottom: 48px;
  }

  .cs-block {
    margin-bottom: 36px;
  }

  .cs-block-label {
    font-size: 11px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 14px;
  }

  .cs-block-text {
    font-size: 15px;
    color: #A8A39D;
    line-height: 1.85;
  }

  .cs-gap-text {
    font-size: 15px;
    color: var(--text);
    line-height: 1.85;
  }

  /* CONTACT */
  .contact-headline {
    font-family: 'Cormorant Garamond', serif;
    font-weight: 300;
    font-size: clamp(28px, 4vw, 38px);
    line-height: 1.3;
    color: var(--text);
    margin-bottom: 48px;
  }

  .contact-links {
    display: flex;
    flex-direction: column;
    gap: 16px;
  }

  .contact-link {
    font-size: 14px;
    color: var(--muted);
    text-decoration: none;
    letter-spacing: 0.02em;
    transition: color 0.3s ease;
  }

  .contact-link:hover { color: var(--accent); }

  .contact-link span {
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--muted);
    margin-right: 16px;
    opacity: 0.5;
  }

  /* FOOTER */
  footer {
    max-width: var(--max);
    margin: 0 auto;
    padding: 40px 32px 64px;
    border-top: 1px solid var(--rule);
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 12px;
  }

  .footer-name {
    font-size: 12px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
  }

  .footer-year {
    font-size: 12px;
    color: var(--rule);
    color: #2E2C2A;
  }

  /* ANIMATIONS */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(18px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .fade-in {
    opacity: 1;
    transform: translateY(0);
    transition: opacity 0.7s ease, transform 0.7s ease;
  }

  .js-loaded .fade-in {
    opacity: 0;
    transform: translateY(16px);
  }

  .js-loaded .fade-in.visible {
    opacity: 1;
    transform: translateY(0);
  }

  /* RESPONSIVE */
  @media (max-width: 640px) {
    nav { padding: 24px 24px; }
    section { padding: 100px 24px; }
    #hero { padding-top: 160px; }
    .cap-grid { grid-template-columns: 1fr; gap: 40px; }
    .cs-meta { flex-direction: column; gap: 4px; }
    footer { padding: 32px 24px 48px; }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#hero" class="nav-name">Anushka Joshi</a>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#capabilities">Capabilities</a></li>
    <li><a href="#work">Work</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO -->
<section id="hero">
  <p class="hero-label">Strategy &amp; Research</p>
  <h1 class="hero-headline">Strategy focused on<br>complex systems.</h1>
  <p class="hero-sub">I turn structural gaps into clear direction and execution.</p>
  <div class="hero-tags">
    <span class="tag">AI</span>
    <span class="tag-sep">/</span>
    <span class="tag">Healthcare</span>
    <span class="tag-sep">/</span>
    <span class="tag">National Security</span>
    <span class="tag-sep">/</span>
    <span class="tag">Neurotechnology</span>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <p class="section-label fade-in">About</p>
  <p class="about-text fade-in">I work on complex systems that influence real decisions. I identify structural gaps and turn them into clear, executable direction.</p>
</section>

<!-- CAPABILITIES -->
<section id="capabilities">
  <p class="section-label fade-in">What I bring to the table</p>
  <p class="cap-intro fade-in">The way I approach complex systems.</p>
  <div class="cap-grid">
    <div class="cap-item fade-in">
      <p class="cap-item-title">Systems Framing</p>
      <p class="cap-item-desc">I identify structural gaps across data, workflow, and incentives. I define what is actually breaking before proposing solutions.</p>
    </div>
    <div class="cap-item fade-in">
      <p class="cap-item-title">Standards &amp; Infrastructure</p>
      <p class="cap-item-desc">I understand how interoperability, semantic structure, and governance shape what is possible in real-world systems.</p>
    </div>
    <div class="cap-item fade-in">
      <p class="cap-item-title">Strategic Positioning</p>
      <p class="cap-item-desc">I translate technical complexity into clear narratives, tradeoffs, and long-term direction.</p>
    </div>
    <div class="cap-item fade-in">
      <p class="cap-item-title">Execution Discipline</p>
      <p class="cap-item-desc">I turn thinking into artifacts teams can use immediately. Frameworks, roadmaps, and decision briefs.</p>
    </div>
  </div>
</section>

<!-- CASE STUDIES -->
<section id="work">
  <p class="cs-section-label fade-in">Selected Work</p>

  <!-- CS 1 -->
  <div class="case-study fade-in">
    <div class="cs-meta">
      <span class="cs-number">01</span>
      <span class="cs-tag">Healthcare AI &middot; Interoperability</span>
    </div>
    <h2 class="cs-title">Interoperability for Intelligent Health Systems</h2>
    <p class="cs-collab">In collaboration with Dr. David Rhew, Chief Medical Officer at Microsoft</p>

    <div class="cs-block">
      <p class="cs-block-label">Problem</p>
      <p class="cs-block-text">Healthcare systems can exchange data, but they struggle to use it in ways that support real clinical and operational decisions. Standards exist, yet workflows remain fragmented.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">What Was Missing</p>
      <p class="cs-block-text">Data could move between systems, but it was not consistently interpreted in context. There was little clarity on how technical standards, semantic reasoning, and workflow integration should work together. Consumer tools and enterprise systems operated with different assumptions, without a shared framework.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">How I Filled the Gap</p>
      <p class="cs-gap-text">Working alongside Dr. David Rhew, I structured interoperability across three layers: data exchange, semantic understanding, and workflow execution. I clarified the difference between information that is transferable and information that is actionable. I analyzed how standards like FHIR enable structured exchange but require contextual reasoning to support real decisions. I then mapped contrasting architectural approaches and outlined how a hybrid model could better support both patients and institutions. The result was a clear framework that translated technical complexity into strategic direction.</p>
    </div>
  </div>

  <!-- CS 2 -->
  <div class="case-study fade-in">
    <div class="cs-meta">
      <span class="cs-number">02</span>
      <span class="cs-tag">National Security &middot; AI Intelligence</span>
    </div>
    <h2 class="cs-title">AI Visibility in National Security Intelligence</h2>
    <p class="cs-collab">See resume for role and organizational details</p>

    <div class="cs-block">
      <p class="cs-block-label">Problem</p>
      <p class="cs-block-text">Emerging AI systems changed how research, coordination, and influence activity take place. Traditional intelligence workflows were not designed to detect these new signals.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">What Was Missing</p>
      <p class="cs-block-text">Monitoring efforts focused on outputs, not the underlying infrastructure and behavior patterns. There was no clear framework connecting AI-driven activity to policy-relevant intelligence. The shift was recognized, but not structured.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">How I Filled the Gap</p>
      <p class="cs-gap-text">I reframed the issue as a visibility gap. I organized product capabilities into a policy-to-intelligence pipeline that clarified how signals are collected, analyzed, assessed, and translated into action. I simplified complex monitoring concepts into a structured narrative that stakeholders could understand and apply. This provided a clearer foundation for institutional decision-making in a rapidly shifting environment.</p>
    </div>
  </div>

  <!-- CS 3 -->
  <div class="case-study fade-in">
    <div class="cs-meta">
      <span class="cs-number">03</span>
      <span class="cs-tag">Neurotechnology &middot; Strategic Framing</span>
    </div>
    <h2 class="cs-title">UploadedMind: Strategic Framing for a Brain-Computer Interface</h2>
    <p class="cs-collab">Advisor: Gopi Kallayil, Chief Business Strategist, Google</p>

    <div class="cs-block">
      <p class="cs-block-label">Problem</p>
      <p class="cs-block-text">The BCI field is driven by bold scientific ideas, but many concepts lack clear positioning and staged feasibility. Ambition often outpaced structure.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">What Was Missing</p>
      <p class="cs-block-text">Clear differentiation from electrode-based competitors. A phased roadmap grounded in practical milestones. A narrative that connected technical feasibility to investor confidence.</p>
    </div>

    <div class="cs-block">
      <p class="cs-block-label">How I Filled the Gap</p>
      <p class="cs-gap-text">With guidance from Gopi Kallayil, I structured the concept into a phased roadmap beginning with medical applications and expanding over time. I clarified tradeoffs in resolution, invasiveness, and scalability. I refined the positioning so the long-term vision was supported by credible near-term milestones. I strengthened the rationale by grounding it in advances in imaging, gene therapy, and computation. The outcome was a focused, investor-ready narrative that aligned scientific ambition with strategic direction.</p>
    </div>
  </div>

</section>

<!-- CONTACT -->
<section id="contact">
  <p class="section-label fade-in">Contact</p>
  <p class="contact-headline fade-in">If you are working on something that does not have a framework yet.</p>
  <div class="contact-links fade-in">
    <a href="/cdn-cgi/l/email-protection#bcddd2c9cfd4d7dd92d6d3cfd4d58c8dfccfd6cfc992d9d8c9" class="contact-link">
      <span>Email</span><span class="__cf_email__" data-cfemail="b8d9d6cdcbd0d3d996d2d7cbd0d18889f8cbd2cbcd96dddccd">[email&#160;protected]</span>
    </a>
    <a href="https://www.linkedin.com/in/anushka-joshi01/" target="_blank" rel="noopener" class="contact-link">
      <span>LinkedIn</span>anushka-joshi01
    </a>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <span class="footer-name">Anushka Joshi</span>
  <span class="footer-year">2026</span>
</footer>

<script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>
  // Scroll-triggered fade-ins
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry, i) => {
      if (entry.isIntersecting) {
        setTimeout(() => {
 
