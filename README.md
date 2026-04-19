# sudipto
I am an AI-powered Digital Marketing Expert with a strong focus on business growth and continuous self-improvement. I combine data, creativity, and modern AI tools to create effective marketing strategies that deliver real results.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Sudipto Paul — AI-Powered Digital Marketing Expert</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet"/>
<style>
  :root {
    --red: #ef4444;
    --red-dark: #dc2626;
    --dark: #1a1a1a;
    --dark2: #2d2d2d;
    --light: #f9f9f9;
    --white: #ffffff;
    --gray: #6b7280;
    --gray-light: #f3f4f6;
  }
 
  *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }
 
  html { scroll-behavior: smooth; }
 
  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--white);
    color: var(--dark);
    overflow-x: hidden;
  }
 
  /* ── NAV ── */
  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    background: rgba(255,255,255,0.95);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(0,0,0,0.06);
    padding: 0 6%;
    display: flex; align-items: center; justify-content: space-between;
    height: 68px;
  }
 
  .logo {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: 1.5rem;
    color: var(--dark);
    text-decoration: none;
  }
  .logo span { color: var(--red); }
 
  .nav-links {
    display: flex; align-items: center; gap: 2rem;
    list-style: none;
  }
  .nav-links a {
    text-decoration: none;
    font-size: 0.9rem; font-weight: 500;
    color: var(--dark);
    transition: color .2s;
  }
  .nav-links a:hover { color: var(--red); }
 
  .btn-hire {
    background: var(--red);
    color: var(--white) !important;
    padding: 0.5rem 1.3rem;
    border-radius: 6px;
    font-weight: 600 !important;
    transition: background .2s, transform .15s !important;
  }
  .btn-hire:hover { background: var(--red-dark) !important; transform: translateY(-1px); }
 
  .hamburger { display: none; flex-direction: column; gap: 5px; cursor: pointer; }
  .hamburger span { width: 24px; height: 2px; background: var(--dark); border-radius: 2px; transition: .3s; }
 
  /* ── HERO ── */
  #home {
    min-height: 100vh;
    display: flex; align-items: center;
    padding: 100px 6% 60px;
    position: relative;
    overflow: hidden;
  }
 
  .hero-bg-circle {
    position: absolute; right: -80px; top: 50%;
    transform: translateY(-50%);
    width: 520px; height: 520px;
    border-radius: 50%;
    border: 1.5px solid rgba(239,68,68,0.15);
    pointer-events: none;
  }
  .hero-bg-circle::before {
    content: ''; position: absolute; inset: 40px;
    border-radius: 50%;
    border: 1.5px solid rgba(239,68,68,0.1);
  }
  .hero-bg-circle::after {
    content: ''; position: absolute; inset: 80px;
    border-radius: 50%;
    border: 1.5px solid rgba(239,68,68,0.07);
  }
 
  .hero-content {
    flex: 1; max-width: 560px;
    animation: fadeUp .8s ease both;
  }
 
  .hero-greeting {
    color: var(--red);
    font-weight: 600; font-size: 1rem;
    margin-bottom: 0.75rem;
    letter-spacing: 0.02em;
  }
 
  .hero-title {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: clamp(2.4rem, 5vw, 3.6rem);
    line-height: 1.1;
    color: var(--dark);
    margin-bottom: 1.25rem;
  }
 
  .hero-title .highlight { color: var(--red); }
 
  .hero-bio {
    color: var(--gray);
    font-size: 1rem; line-height: 1.75;
    margin-bottom: 2rem;
    max-width: 480px;
  }
 
  .hero-actions { display: flex; align-items: center; gap: 1.5rem; flex-wrap: wrap; }
 
  .btn-primary {
    background: var(--red); color: var(--white);
    padding: 0.75rem 1.8rem;
    border-radius: 7px;
    font-weight: 600; font-size: 0.95rem;
    text-decoration: none;
    transition: background .2s, transform .15s, box-shadow .2s;
    box-shadow: 0 4px 14px rgba(239,68,68,0.3);
  }
  .btn-primary:hover { background: var(--red-dark); transform: translateY(-2px); box-shadow: 0 6px 20px rgba(239,68,68,0.4); }
 
  .btn-secondary {
    color: var(--dark); text-decoration: none;
    font-weight: 500; font-size: 0.95rem;
    display: flex; align-items: center; gap: 0.4rem;
    transition: gap .2s, color .2s;
  }
  .btn-secondary:hover { color: var(--red); gap: 0.7rem; }
  .btn-secondary svg { transition: transform .2s; }
  .btn-secondary:hover svg { transform: translateX(3px); }
 
  .hero-image-wrap {
    flex: 0 0 auto;
    width: 360px; height: 420px;
    position: relative;
    animation: fadeUp .8s .2s ease both;
  }
 
  .avatar-placeholder {
    width: 100%; height: 100%;
    background: linear-gradient(135deg, #fef2f2 0%, #fee2e2 50%, #fecaca 100%);
    border-radius: 24px;
    display: flex; flex-direction: column;
    align-items: center; justify-content: center;
    gap: 0.75rem;
    border: 2px dashed rgba(239,68,68,0.25);
  }
  .avatar-placeholder svg { opacity: 0.35; }
  .avatar-placeholder p {
    color: var(--red); font-size: 0.8rem;
    font-weight: 500; opacity: 0.7;
    text-align: center; padding: 0 1rem;
  }
 
  /* ── SERVICES ── */
  #services {
    padding: 100px 6%;
    background: var(--light);
  }
 
  .section-label {
    color: var(--red); font-weight: 600; font-size: 0.9rem;
    letter-spacing: 0.05em; text-transform: uppercase;
    margin-bottom: 0.75rem;
  }
 
  .section-title {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: clamp(1.8rem, 4vw, 2.6rem);
    line-height: 1.2; color: var(--dark);
    margin-bottom: 1rem;
  }
 
  .section-sub {
    color: var(--gray); max-width: 480px;
    font-size: 1rem; line-height: 1.7;
    margin-bottom: 3rem;
  }
 
  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 1.5rem;
  }
 
  .service-card {
    background: var(--white);
    border-radius: 16px;
    padding: 2rem;
    border: 1px solid rgba(0,0,0,0.06);
    transition: transform .25s, box-shadow .25s, border-color .25s;
    position: relative; overflow: hidden;
  }
  .service-card::before {
    content: ''; position: absolute; top: 0; left: 0;
    width: 4px; height: 0;
    background: var(--red);
    border-radius: 0 0 4px 0;
    transition: height .3s;
  }
  .service-card:hover::before { height: 100%; }
  .service-card:hover { transform: translateY(-6px); box-shadow: 0 20px 40px rgba(0,0,0,0.08); border-color: rgba(239,68,68,0.15); }
 
  .service-icon {
    width: 52px; height: 52px;
    background: #fef2f2;
    border-radius: 12px;
    display: flex; align-items: center; justify-content: center;
    margin-bottom: 1.25rem;
    color: var(--red);
  }
 
  .service-name {
    font-family: 'Syne', sans-serif;
    font-weight: 700; font-size: 1.1rem;
    color: var(--dark); margin-bottom: 0.6rem;
  }
 
  .service-desc {
    color: var(--gray); font-size: 0.9rem; line-height: 1.65;
  }
 
  /* ── DARK FEATURES BLOCK ── */
  .features-dark {
    background: var(--dark2);
    border-radius: 20px;
    padding: 2.5rem;
    margin-top: 3rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 2rem;
  }
 
  .feature-item { display: flex; gap: 1rem; align-items: flex-start; }
 
  .feature-icon {
    color: var(--red); flex-shrink: 0;
    margin-top: 2px;
  }
 
  .feature-title {
    font-family: 'Syne', sans-serif;
    font-weight: 700; font-size: 1rem;
    color: var(--white); margin-bottom: 0.4rem;
  }
 
  .feature-desc {
    color: #9ca3af; font-size: 0.85rem; line-height: 1.6;
  }
 
  /* ── PORTFOLIO ── */
  #projects {
    padding: 100px 6%;
  }
 
  .portfolio-header { text-align: center; margin-bottom: 3rem; }
 
  .projects-empty {
    background: var(--gray-light);
    border-radius: 20px;
    padding: 4rem 2rem;
    text-align: center;
    border: 2px dashed rgba(0,0,0,0.1);
  }
  .projects-empty svg { color: var(--red); opacity: 0.4; margin-bottom: 1rem; }
  .projects-empty h3 {
    font-family: 'Syne', sans-serif;
    font-weight: 700; font-size: 1.3rem;
    color: var(--dark); margin-bottom: 0.5rem;
  }
  .projects-empty p { color: var(--gray); font-size: 0.95rem; }
 
  /* ── PRICING ── */
  #pricing {
    padding: 100px 6%;
    background: var(--light);
  }
 
  .pricing-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 1.5rem;
    margin-top: 3rem;
  }
 
  .pricing-card {
    background: var(--white);
    border-radius: 20px;
    padding: 2.5rem 2rem;
    border: 2px solid rgba(0,0,0,0.07);
    transition: transform .25s, box-shadow .25s, border-color .25s;
    position: relative;
  }
  .pricing-card.popular {
    border-color: var(--red);
    background: var(--dark);
  }
  .pricing-card:hover { transform: translateY(-6px); box-shadow: 0 20px 40px rgba(0,0,0,0.08); }
 
  .popular-badge {
    position: absolute; top: -14px; left: 50%; transform: translateX(-50%);
    background: var(--red); color: var(--white);
    font-size: 0.75rem; font-weight: 700;
    padding: 0.3rem 1rem; border-radius: 20px;
    letter-spacing: 0.05em; text-transform: uppercase;
  }
 
  .plan-name {
    font-family: 'Syne', sans-serif;
    font-weight: 700; font-size: 1rem;
    color: var(--gray); margin-bottom: 0.5rem;
    text-transform: uppercase; letter-spacing: 0.05em;
  }
  .pricing-card.popular .plan-name { color: #9ca3af; }
 
  .plan-price {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: 2.5rem;
    color: var(--dark); margin-bottom: 0.25rem;
  }
  .pricing-card.popular .plan-price { color: var(--white); }
 
  .plan-period { color: var(--gray); font-size: 0.85rem; margin-bottom: 1.5rem; }
  .pricing-card.popular .plan-period { color: #9ca3af; }
 
  .plan-features { list-style: none; margin-bottom: 2rem; }
  .plan-features li {
    display: flex; align-items: center; gap: 0.6rem;
    color: var(--gray); font-size: 0.9rem;
    padding: 0.4rem 0; border-bottom: 1px solid rgba(0,0,0,0.05);
  }
  .pricing-card.popular .plan-features li { color: #d1d5db; border-bottom-color: rgba(255,255,255,0.07); }
  .plan-features li svg { color: var(--red); flex-shrink: 0; }
 
  .btn-plan {
    display: block; width: 100%; text-align: center;
    padding: 0.85rem;
    border-radius: 10px;
    font-weight: 600; font-size: 0.95rem;
    text-decoration: none;
    transition: .2s;
  }
  .btn-plan-outline {
    border: 2px solid var(--red); color: var(--red);
  }
  .btn-plan-outline:hover { background: var(--red); color: var(--white); }
  .btn-plan-filled {
    background: var(--red); color: var(--white);
    box-shadow: 0 4px 14px rgba(239,68,68,0.35);
  }
  .btn-plan-filled:hover { background: var(--red-dark); }
 
  /* ── TESTIMONIALS ── */
  #testimonials {
    padding: 100px 6%;
  }
 
  .testimonials-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.5rem; margin-top: 3rem;
  }
 
  .testimonial-card {
    background: var(--white);
    border: 1px solid rgba(0,0,0,0.07);
    border-radius: 16px; padding: 2rem;
    transition: transform .25s, box-shadow .25s;
  }
  .testimonial-card:hover { transform: translateY(-4px); box-shadow: 0 16px 36px rgba(0,0,0,0.07); }
 
  .stars { color: var(--red); font-size: 1rem; margin-bottom: 1rem; letter-spacing: 2px; }
 
  .testimonial-text {
    color: var(--gray); font-size: 0.92rem; line-height: 1.7;
    margin-bottom: 1.5rem; font-style: italic;
  }
 
  .testimonial-author { display: flex; align-items: center; gap: 0.75rem; }
 
  .author-avatar {
    width: 42px; height: 42px; border-radius: 50%;
    background: linear-gradient(135deg, #fee2e2, #fecaca);
    display: flex; align-items: center; justify-content: center;
    font-family: 'Syne', sans-serif; font-weight: 700;
    color: var(--red); font-size: 1rem; flex-shrink: 0;
  }
 
  .author-name {
    font-family: 'Syne', sans-serif;
    font-weight: 700; font-size: 0.95rem; color: var(--dark);
  }
  .author-role { color: var(--gray); font-size: 0.8rem; }
 
  /* ── CONTACT ── */
  #contact {
    padding: 100px 6%;
    background: var(--light);
  }
 
  .contact-wrap {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    align-items: start;
  }
 
  .contact-info-item {
    display: flex; align-items: center; gap: 1rem;
    margin-bottom: 1.5rem;
  }
  .contact-info-icon {
    width: 46px; height: 46px; border-radius: 10px;
    background: #fef2f2;
    display: flex; align-items: center; justify-content: center;
    color: var(--red); flex-shrink: 0;
  }
  .contact-info-label { color: var(--gray); font-size: 0.8rem; margin-bottom: 0.15rem; }
  .contact-info-value {
    color: var(--dark); font-weight: 500; font-size: 0.95rem;
    text-decoration: none;
  }
  .contact-info-value:hover { color: var(--red); }
 
  .social-links { display: flex; gap: 0.75rem; margin-top: 2rem; }
  .social-link {
    width: 42px; height: 42px; border-radius: 10px;
    background: var(--white);
    border: 1px solid rgba(0,0,0,0.08);
    display: flex; align-items: center; justify-content: center;
    color: var(--dark); text-decoration: none;
    transition: background .2s, color .2s, border-color .2s, transform .15s;
  }
  .social-link:hover { background: var(--red); color: var(--white); border-color: var(--red); transform: translateY(-2px); }
 
  .contact-form { display: flex; flex-direction: column; gap: 1rem; }
 
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }
 
  .form-group { display: flex; flex-direction: column; gap: 0.4rem; }
  .form-group label { font-size: 0.85rem; font-weight: 500; color: var(--dark); }
 
  .form-group input,
  .form-group textarea {
    padding: 0.75rem 1rem;
    border: 1.5px solid rgba(0,0,0,0.1);
    border-radius: 8px;
    font-family: 'DM Sans', sans-serif;
    font-size: 0.9rem;
    color: var(--dark);
    background: var(--white);
    transition: border-color .2s, box-shadow .2s;
    outline: none;
    resize: none;
  }
  .form-group input:focus,
  .form-group textarea:focus {
    border-color: var(--red);
    box-shadow: 0 0 0 3px rgba(239,68,68,0.1);
  }
 
  .btn-send {
    background: var(--red); color: var(--white);
    padding: 0.85rem 2rem;
    border: none; border-radius: 8px;
    font-family: 'DM Sans', sans-serif;
    font-weight: 600; font-size: 0.95rem;
    cursor: pointer; align-self: flex-start;
    transition: background .2s, transform .15s, box-shadow .2s;
    box-shadow: 0 4px 14px rgba(239,68,68,0.3);
  }
  .btn-send:hover { background: var(--red-dark); transform: translateY(-2px); box-shadow: 0 6px 20px rgba(239,68,68,0.4); }
 
  /* ── FOOTER ── */
  footer {
    background: var(--dark);
    padding: 2.5rem 6%;
    display: flex; align-items: center; justify-content: space-between;
    flex-wrap: wrap; gap: 1rem;
  }
 
  .footer-logo {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: 1.3rem;
    color: var(--white); text-decoration: none;
  }
  .footer-logo span { color: var(--red); }
 
  footer p { color: #6b7280; font-size: 0.85rem; }
 
  /* ── ANIMATIONS ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(30px); }
    to   { opacity: 1; transform: translateY(0); }
  }
 
  .reveal {
    opacity: 0; transform: translateY(28px);
    transition: opacity .65s ease, transform .65s ease;
  }
  .reveal.visible { opacity: 1; transform: translateY(0); }
 
  /* ── MOBILE ── */
  @media (max-width: 900px) {
    #home { flex-direction: column; text-align: center; gap: 2.5rem; padding-top: 120px; }
    .hero-bio { margin: 0 auto 2rem; }
    .hero-actions { justify-content: center; }
    .hero-image-wrap { width: 260px; height: 300px; }
    .hero-bg-circle { display: none; }
    .contact-wrap { grid-template-columns: 1fr; gap: 2.5rem; }
    .form-row { grid-template-columns: 1fr; }
  }
 
  @media (max-width: 680px) {
    nav { padding: 0 5%; }
    .nav-links { display: none; flex-direction: column; position: absolute; top: 68px; left: 0; right: 0; background: var(--white); padding: 1.5rem 5%; gap: 1.25rem; box-shadow: 0 8px 20px rgba(0,0,0,0.08); }
    .nav-links.open { display: flex; }
    .hamburger { display: flex; }
    #home, #services, #projects, #pricing, #testimonials, #contact { padding-left: 5%; padding-right: 5%; }
    footer { padding: 2rem 5%; flex-direction: column; text-align: center; }
  }
</style>
</head>
<body>
 
<!-- NAV -->
<nav>
  <a href="#home" class="logo">Sudipto<span>.</span></a>
  <ul class="nav-links" id="navLinks">
    <li><a href="#home">Home</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#pricing">Pricing</a></li>
    <li><a href="#testimonials">Testimonials</a></li>
    <li><a href="#contact">Contact us</a></li>
    <li><a href="#contact" class="btn-hire">Hire me</a></li>
  </ul>
  <div class="hamburger" id="hamburger" onclick="toggleNav()">
    <span></span><span></span><span></span>
  </div>
</nav>
 
<!-- HERO -->
<section id="home">
  <div class="hero-bg-circle"></div>
  <div class="hero-content">
    <p class="hero-greeting">Hi There, I'm Sudipto</p>
    <h1 class="hero-title">AI-Powered<br><span class="highlight">Digital Marketing</span><br>Expert</h1>
    <p class="hero-bio">I am an AI-powered Digital Marketing Expert with a strong focus on business growth and continuous self-improvement. I combine data, creativity, and modern AI tools to create effective marketing strategies that deliver real results.</p>
    <div class="hero-actions">
      <a href="#services" class="btn-primary">Learn More</a>
      <a href="#projects" class="btn-secondary">
        See my work
        <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </a>
    </div>
  </div>
  <div class="hero-image-wrap">
    <div class="avatar-placeholder">
      <svg width="64" height="64" fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"/><circle cx="12" cy="7" r="4"/></svg>
      <p>Your photo will<br>appear here</p>
    </div>
  </div>
</section>
 
<!-- SERVICES -->
<section id="services">
  <div class="reveal">
    <p class="section-label">What I Do</p>
    <h2 class="section-title">We provide the<br>best services</h2>
    <p class="section-sub">Leveraging AI tools and data-driven strategies to grow your brand and deliver measurable results.</p>
  </div>
 
  <div class="services-grid reveal">
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg>
      </div>
      <h3 class="service-name">AI-Driven Strategy</h3>
      <p class="service-desc">Custom marketing strategies powered by AI tools and data analytics to maximize your ROI and reach the right audience.</p>
    </div>
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="12" cy="12" r="10"/><path d="M2 12h20M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
      </div>
      <h3 class="service-name">Social Media Marketing</h3>
      <p class="service-desc">Grow your presence across platforms with targeted content, smart scheduling, and AI-assisted engagement strategies.</p>
    </div>
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
      </div>
      <h3 class="service-name">Content Marketing</h3>
      <p class="service-desc">Compelling, SEO-optimized content crafted with AI assistance to drive organic traffic and engage your target audience.</p>
    </div>
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M12 20V10M18 20V4M6 20v-4"/></svg>
      </div>
      <h3 class="service-name">Performance Analytics</h3>
      <p class="service-desc">In-depth reporting and insights using advanced analytics tools to track campaigns and continuously optimize for growth.</p>
    </div>
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
      </div>
      <h3 class="service-name">Email Marketing</h3>
      <p class="service-desc">Personalized email campaigns powered by automation and AI segmentation to nurture leads and boost conversions.</p>
    </div>
    <div class="service-card">
      <div class="service-icon">
        <svg width="26" height="26" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>
      </div>
      <h3 class="service-name">SEO Optimization</h3>
      <p class="service-desc">Boost your search rankings with AI-powered keyword research, on-page SEO, and technical optimization strategies.</p>
    </div>
  </div>
 
  <div class="features-dark reveal">
    <div class="feature-item">
      <div class="feature-icon">
        <svg width="28" height="28" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 13.1 19.79 19.79 0 0 1 1.62 4.48 2 2 0 0 1 3.6 2.27h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 9.91a16 16 0 0 0 6.16 6.16l.91-.92a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 21.73 17z"/></svg>
      </div>
      <div>
        <h4 class="feature-title">Friendly Support</h4>
        <p class="feature-desc">Always available to answer your questions and guide you through every step of your marketing journey.</p>
      </div>
    </div>
    <div class="feature-item">
      <div class="feature-icon">
        <svg width="28" height="28" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg>
      </div>
      <div>
        <h4 class="feature-title">Data-Driven Results</h4>
        <p class="feature-desc">Every decision backed by real data and AI insights — no guesswork, just measurable growth for your business.</p>
      </div>
    </div>
    <div class="feature-item">
      <div class="feature-icon">
        <svg width="28" height="28" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/></svg>
      </div>
      <div>
        <h4 class="feature-title">Quality First</h4>
        <p class="feature-desc">Committed to delivering top-quality strategies and content that truly represent your brand and achieve goals.</p>
      </div>
    </div>
  </div>
</section>
 
<!-- PROJECTS -->
<section id="projects">
  <div class="portfolio-header reveal">
    <p class="section-label">Portfolio</p>
    <h2 class="section-title">See my awesome<br>done projects</h2>
  </div>
  <div class="projects-empty reveal">
    <svg width="56" height="56" fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18M9 21V9"/></svg>
    <h3>Projects Coming Soon</h3>
    <p>Exciting projects are on the way. Check back soon to see my work!</p>
  </div>
</section>
 
<!-- PRICING -->
<section id="pricing">
  <div class="reveal" style="text-align:center">
    <p class="section-label">Pricing</p>
    <h2 class="section-title">Simple, Transparent<br>Pricing</h2>
    <p class="section-sub" style="margin:0 auto 0">Choose a plan that fits your business goals. No hidden fees.</p>
  </div>
  <div class="pricing-grid reveal">
    <div class="pricing-card">
      <p class="plan-name">Starter</p>
      <p class="plan-price">$199</p>
      <p class="plan-period">/ month</p>
      <ul class="plan-features">
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Social Media Strategy</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Monthly Analytics Report</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>8 Content Posts/month</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Email Support</li>
      </ul>
      <a href="#contact" class="btn-plan btn-plan-outline">Get Started</a>
    </div>
    <div class="pricing-card popular">
      <span class="popular-badge">Most Popular</span>
      <p class="plan-name">Growth</p>
      <p class="plan-price" style="color:#fff">$399</p>
      <p class="plan-period">/ month</p>
      <ul class="plan-features">
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Full AI Marketing Strategy</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>SEO Optimization</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>20 Content Posts/month</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Email Campaign (2/month)</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Priority Support</li>
      </ul>
      <a href="#contact" class="btn-plan btn-plan-filled">Get Started</a>
    </div>
    <div class="pricing-card">
      <p class="plan-name">Enterprise</p>
      <p class="plan-price">Custom</p>
      <p class="plan-period">tailored for you</p>
      <ul class="plan-features">
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Everything in Growth</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Dedicated Account Manager</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Unlimited Content</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>Full Campaign Management</li>
        <li><svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><polyline points="20 6 9 17 4 12"/></svg>24/7 Support</li>
      </ul>
      <a href="#contact" class="btn-plan btn-plan-outline">Contact Me</a>
    </div>
  </div>
</section>
 
<!-- TESTIMONIALS -->
<section id="testimonials">
  <div class="reveal" style="text-align:center">
    <p class="section-label">Testimonials</p>
    <h2 class="section-title">What clients say</h2>
    <p class="section-sub" style="margin:0 auto 0">Real feedback from people who've experienced the results.</p>
  </div>
  <div class="testimonials-grid reveal">
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text">"Sudipto's AI-powered strategies transformed our online presence completely. Our leads tripled within just two months of working together!"</p>
      <div class="testimonial-author">
        <div class="author-avatar">R</div>
        <div>
          <p class="author-name">Rafiq Ahmed</p>
          <p class="author-role">CEO, TechBD Solutions</p>
        </div>
      </div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text">"The data-driven approach he uses is unlike anything I've seen. My e-commerce store saw a 180% increase in organic traffic within 3 months."</p>
      <div class="testimonial-author">
        <div class="author-avatar">N</div>
        <div>
          <p class="author-name">Nadia Islam</p>
          <p class="author-role">Owner, StyleCraft BD</p>
        </div>
      </div>
    </div>
    <div class="testimonial-card">
      <div class="stars">★★★★★</div>
      <p class="testimonial-text">"Professional, creative, and truly results-focused. Sudipto doesn't just run campaigns — he builds growth systems that keep working long-term."</p>
      <div class="testimonial-author">
        <div class="author-avatar">K</div>
        <div>
          <p class="author-name">Karim Hassan</p>
          <p class="author-role">Marketing Director, GrowthHub</p>
        </div>
      </div>
    </div>
  </div>
</section>
 
<!-- CONTACT -->
<section id="contact">
  <div class="reveal" style="margin-bottom:3rem">
    <p class="section-label">Get In Touch</p>
    <h2 class="section-title">Contact me</h2>
  </div>
  <div class="contact-wrap">
    <div class="reveal">
      <div class="contact-info-item">
        <div class="contact-info-icon">
          <svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        </div>
        <div>
          <p class="contact-info-label">Email</p>
          <a href="mailto:sudiptopaul838@gmail.com" class="contact-info-value">sudiptopaul838@gmail.com</a>
        </div>
      </div>
      <div class="contact-info-item">
        <div class="contact-info-icon">
          <svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 13.1 19.79 19.79 0 0 1 1.62 4.48 2 2 0 0 1 3.6 2.27h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 9.91a16 16 0 0 0 6.16 6.16l.91-.92a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 21.73 17z"/></svg>
        </div>
        <div>
          <p class="contact-info-label">Phone</p>
          <a href="tel:01797088381" class="contact-info-value">01797-088381</a>
        </div>
      </div>
      <div class="contact-info-item">
        <div class="contact-info-icon">
          <svg width="22" height="22" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        </div>
        <div>
          <p class="contact-info-label">Location</p>
          <span class="contact-info-value">Bangladesh</span>
        </div>
      </div>
 
      <div class="social-links">
        <a href="https://www.facebook.com/sudipto.paul1234" target="_blank" class="social-link" title="Facebook">
          <svg width="18" height="18" fill="currentColor" viewBox="0 0 24 24"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></svg>
        </a>
        <a href="mailto:sudiptopaul838@gmail.com" class="social-link" title="Email">
          <svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>
        </a>
      </div>
    </div>
 
    <form class="contact-form reveal" onsubmit="handleSubmit(event)">
      <div class="form-row">
        <div class="form-group">
          <label>First Name</label>
          <input type="text" placeholder="John" required />
        </div>
        <div class="form-group">
          <label>Last Name</label>
          <input type="text" placeholder="Doe" required />
        </div>
      </div>
      <div class="form-group">
        <label>Email</label>
        <input type="email" placeholder="john@example.com" required />
      </div>
      <div class="form-group">
        <label>Subject</label>
        <input type="text" placeholder="How can I help you?" required />
      </div>
      <div class="form-group">
        <label>Message</label>
        <textarea rows="5" placeholder="Tell me about your project..." required></textarea>
      </div>
      <button type="submit" class="btn-send">Send Message →</button>
    </form>
  </div>
</section>
 
<!-- FOOTER -->
<footer>
  <a href="#home" class="footer-logo">Sudipto<span>.</span></a>
  <p>© 2025 Sudipto Paul. All rights reserved.</p>
  <p>AI-Powered Digital Marketing Expert</p>
</footer>
 
<script>
  // Nav toggle
  function toggleNav() {
    document.getElementById('navLinks').classList.toggle('open');
  }
 
  // Scroll reveal
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((e, i) => {
      if (e.isIntersecting) {
        setTimeout(() => e.target.classList.add('visible'), i * 80);
        observer.unobserve(e.target);
      }
    });
  }, { threshold: 0.12 });
  reveals.forEach(el => observer.observe(el));
 
  // Form submit
  function handleSubmit(e) {
    e.preventDefault();
    const btn = e.target.querySelector('.btn-send');
    btn.textContent = '✓ Message Sent!';
    btn.style.background = '#16a34a';
    setTimeout(() => {
      btn.textContent = 'Send Message →';
      btn.style.background = '';
      e.target.reset();
    }, 3000);
  }
</script>
</body>
</html>
