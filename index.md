---
layout: default
title: Apex Data Cloud | AI & Data Strategy Consulting
description: Apex Data Cloud partners with executives and founders to transform complex data into decisive strategy using AI, analytics, and modern cloud platforms.
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@500;600;700;800&display=swap" rel="stylesheet">

<style>
/* === RESET & JEKYLL OVERRIDES === */
.page-content { padding: 0 !important; }
.wrapper { max-width: 100% !important; padding: 0 !important; }
.site-header, .site-footer { display: none !important; }
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

:root {
  --navy:     #060D1A;
  --navy-2:   #0A1628;
  --navy-3:   #112240;
  --navy-4:   #1a3a6b;
  --blue:     #0EA5E9;
  --blue-2:   #38BDF8;
  --blue-3:   #7DD3FC;
  --gold:     #F59E0B;
  --white:    #F8FAFC;
  --text:     #94A3B8;
  --text-2:   #CBD5E1;
  --border:   rgba(14,165,233,0.18);
  --border-2: rgba(14,165,233,0.08);
}

.apex-site {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  background: var(--navy);
  color: var(--white);
  overflow-x: hidden;
  line-height: 1.6;
}

/* === NAVBAR === */
.nav {
  position: fixed; top: 0; left: 0; right: 0;
  z-index: 1000;
  padding: 14px 32px;
  background: rgba(6,13,26,0.88);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border-bottom: 1px solid var(--border-2);
  transition: all 0.3s;
}
.nav-inner {
  max-width: 1200px; margin: 0 auto;
  display: flex; align-items: center; justify-content: space-between;
}
.nav-logo {
  display: flex; align-items: center; gap: 10px; text-decoration: none;
}
.nav-logo img { height: 34px; width: auto; }
.nav-logo-text {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700; font-size: 17px; color: var(--white);
}
.nav-logo-text span { color: var(--blue); }
.nav-links {
  display: flex; align-items: center; gap: 28px; list-style: none;
}
.nav-links a {
  font-size: 14px; font-weight: 500; color: var(--text-2);
  text-decoration: none; transition: color 0.2s;
}
.nav-links a:hover { color: var(--white); }
.nav-cta {
  background: linear-gradient(135deg, var(--blue), #0284C7) !important;
  color: white !important;
  padding: 9px 22px; border-radius: 8px; font-weight: 600;
  box-shadow: 0 2px 14px rgba(14,165,233,0.28); transition: all 0.3s;
}
.nav-cta:hover { transform: translateY(-1px); box-shadow: 0 5px 22px rgba(14,165,233,0.42) !important; }

/* === HERO === */
.hero {
  min-height: 100vh;
  display: flex; align-items: center;
  padding: 130px 32px 90px;
  position: relative; overflow: hidden;
  background: var(--navy);
}
.hero-grid-bg {
  position: absolute; inset: 0; pointer-events: none;
  background-image:
    linear-gradient(rgba(14,165,233,0.035) 1px, transparent 1px),
    linear-gradient(90deg, rgba(14,165,233,0.035) 1px, transparent 1px);
  background-size: 64px 64px;
}
.hero-glow-1 {
  position: absolute; top: 0; right: -5%; width: 750px; height: 750px;
  background: radial-gradient(circle, rgba(14,165,233,0.10) 0%, transparent 65%);
  pointer-events: none;
}
.hero-glow-2 {
  position: absolute; bottom: -10%; left: -8%; width: 550px; height: 550px;
  background: radial-gradient(circle, rgba(245,158,11,0.06) 0%, transparent 65%);
  pointer-events: none;
}
.hero-inner {
  max-width: 1200px; margin: 0 auto;
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 72px; align-items: center; width: 100%; position: relative; z-index: 1;
}
.hero-badge {
  display: inline-flex; align-items: center; gap: 7px;
  background: rgba(14,165,233,0.08); border: 1px solid rgba(14,165,233,0.25);
  border-radius: 50px; padding: 5px 16px;
  font-size: 11px; font-weight: 600; letter-spacing: 1.5px;
  text-transform: uppercase; color: var(--blue-2); margin-bottom: 20px;
}
.live-dot {
  width: 7px; height: 7px; border-radius: 50%; background: var(--blue);
  animation: pulse-dot 2.2s infinite;
}
@keyframes pulse-dot {
  0%, 100% { opacity: 1; transform: scale(1); }
  50% { opacity: 0.4; transform: scale(0.8); }
}
.hero h1 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(36px, 4.6vw, 60px);
  font-weight: 800; line-height: 1.08; letter-spacing: -1.8px;
  color: var(--white); margin-bottom: 22px;
}
.hero h1 .hl {
  background: linear-gradient(130deg, var(--blue) 0%, var(--blue-2) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
}
.hero p {
  font-size: 17px; line-height: 1.75; color: var(--text-2);
  margin-bottom: 40px; max-width: 490px;
}
.hero-cta { display: flex; gap: 14px; flex-wrap: wrap; align-items: center; }

.btn-primary {
  display: inline-flex; align-items: center; gap: 8px;
  background: linear-gradient(135deg, var(--blue), #0284C7);
  color: white; padding: 14px 30px; border-radius: 10px;
  font-size: 15px; font-weight: 600; text-decoration: none;
  border: none; cursor: pointer; transition: all 0.3s;
  box-shadow: 0 4px 24px rgba(14,165,233,0.32);
}
.btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 36px rgba(14,165,233,0.48); }
.btn-ghost {
  display: inline-flex; align-items: center; gap: 8px;
  background: transparent; color: var(--text-2);
  padding: 14px 28px; border-radius: 10px; font-size: 15px; font-weight: 500;
  text-decoration: none; border: 1px solid rgba(255,255,255,0.1); transition: all 0.3s;
}
.btn-ghost:hover { color: var(--white); border-color: rgba(255,255,255,0.28); background: rgba(255,255,255,0.04); }

/* Hero right panel */
.hero-panel {
  background: rgba(17,34,64,0.65);
  border: 1px solid var(--border);
  border-radius: 20px; padding: 28px;
  backdrop-filter: blur(12px); position: relative;
}
.hero-panel::before {
  content: ''; position: absolute; top: -1px; left: 20%; right: 20%;
  height: 1px; background: linear-gradient(90deg, transparent, var(--blue), transparent);
}
.panel-label {
  font-size: 10px; font-weight: 600; letter-spacing: 2px;
  text-transform: uppercase; color: var(--text); margin-bottom: 18px;
}
.panel-metrics {
  display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 18px;
}
.pm-card {
  background: rgba(6,13,26,0.6); border: 1px solid var(--border-2);
  border-radius: 12px; padding: 14px; text-align: center;
}
.pm-val {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 15px; font-weight: 700; color: var(--blue-2); margin-bottom: 3px;
}
.pm-lbl { font-size: 11px; color: var(--text); }
.panel-pills { display: flex; flex-direction: column; gap: 8px; }
.ppill {
  display: flex; align-items: center; gap: 11px;
  background: rgba(6,13,26,0.5); border: 1px solid var(--border-2);
  border-radius: 9px; padding: 10px 14px;
  font-size: 13px; color: var(--text-2); transition: all 0.2s;
}
.ppill:hover { border-color: var(--border); color: var(--white); }
.ppill-icon {
  width: 30px; height: 30px; border-radius: 7px;
  display: flex; align-items: center; justify-content: center;
  font-size: 15px; flex-shrink: 0;
}

/* === TRUST BAR === */
.trust-bar {
  padding: 24px 32px;
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
  background: rgba(17,34,64,0.35);
}
.trust-bar-inner {
  max-width: 1200px; margin: 0 auto;
  display: flex; align-items: center; justify-content: center;
  gap: 48px; flex-wrap: wrap;
}
.t-item {
  display: flex; align-items: center; gap: 9px;
  font-size: 13px; font-weight: 500; color: var(--text);
}
.t-item svg { color: var(--blue); flex-shrink: 0; }

/* === COMMON SECTION === */
section { padding: 96px 32px; }
.container { max-width: 1200px; margin: 0 auto; }
.sec-header { text-align: center; margin-bottom: 60px; }
.sec-label {
  display: inline-block; font-size: 11px; font-weight: 600;
  letter-spacing: 2px; text-transform: uppercase;
  color: var(--blue); margin-bottom: 14px;
}
.sec-title {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(28px, 3.4vw, 44px);
  font-weight: 700; letter-spacing: -1px;
  color: var(--white); margin-bottom: 16px; line-height: 1.2;
}
.sec-sub {
  font-size: 16px; color: var(--text-2);
  max-width: 560px; margin: 0 auto; line-height: 1.75;
}

/* === SERVICES === */
.services-section { background: var(--navy); }
.services-grid {
  display: grid; grid-template-columns: repeat(2, 1fr); gap: 22px;
}
.svc-card {
  background: var(--navy-3); border: 1px solid var(--border-2);
  border-radius: 18px; padding: 36px 30px;
  transition: all 0.35s; position: relative; overflow: hidden;
}
.svc-card::after {
  content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
  background: linear-gradient(90deg, transparent, var(--blue), transparent);
  transform: scaleX(0); transform-origin: center; transition: transform 0.35s;
}
.svc-card:hover { border-color: var(--border); transform: translateY(-5px); box-shadow: 0 20px 50px rgba(14,165,233,0.09); }
.svc-card:hover::after { transform: scaleX(1); }
.svc-icon {
  width: 52px; height: 52px; border-radius: 14px;
  background: rgba(14,165,233,0.1); border: 1px solid rgba(14,165,233,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 22px; margin-bottom: 20px;
}
.svc-card h3 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 19px; font-weight: 600; color: var(--white); margin-bottom: 12px;
}
.svc-card p { font-size: 14px; color: var(--text-2); line-height: 1.72; margin-bottom: 20px; }
.svc-tags { display: flex; flex-wrap: wrap; gap: 7px; }
.tag {
  font-size: 11px; font-weight: 500; color: var(--blue-3);
  background: rgba(14,165,233,0.08); border: 1px solid rgba(14,165,233,0.15);
  border-radius: 50px; padding: 3px 12px;
}

/* === APPROACH === */
.approach-section { background: linear-gradient(180deg, var(--navy) 0%, var(--navy-2) 100%); }
.steps-row {
  display: grid; grid-template-columns: repeat(4, 1fr);
  gap: 0; position: relative;
}
.steps-row::before {
  content: ''; position: absolute; top: 35px; left: 12.5%; right: 12.5%;
  height: 1px; background: linear-gradient(90deg, transparent, var(--border), var(--border), transparent);
}
.step { text-align: center; padding: 0 20px; }
.step-num {
  width: 70px; height: 70px; border-radius: 50%;
  background: var(--navy-3); border: 1px solid var(--border);
  display: flex; align-items: center; justify-content: center; margin: 0 auto 20px;
  font-family: 'Space Grotesk', sans-serif; font-size: 20px; font-weight: 700;
  color: var(--blue); position: relative; z-index: 1;
}
.step h4 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 15px; font-weight: 600; color: var(--white); margin-bottom: 10px;
}
.step p { font-size: 13px; color: var(--text); line-height: 1.65; }

/* === WHY APEX === */
.why-section { background: var(--navy-2); }
.why-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: center; }
.why-content h2 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(26px, 2.8vw, 40px); font-weight: 700; letter-spacing: -0.8px;
  color: var(--white); margin-bottom: 16px; line-height: 1.2;
}
.why-content > p { font-size: 16px; color: var(--text-2); line-height: 1.75; margin-bottom: 36px; }
.diffs { display: flex; flex-direction: column; gap: 20px; }
.diff {
  display: flex; gap: 16px; align-items: flex-start;
  padding: 18px; border-radius: 12px;
  border: 1px solid var(--border-2); background: rgba(6,13,26,0.3);
  transition: border-color 0.2s;
}
.diff:hover { border-color: var(--border); }
.diff-ico {
  width: 40px; height: 40px; border-radius: 10px;
  background: rgba(14,165,233,0.1); border: 1px solid rgba(14,165,233,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 18px; flex-shrink: 0; margin-top: 1px;
}
.diff h4 { font-size: 14px; font-weight: 600; color: var(--white); margin-bottom: 5px; }
.diff p { font-size: 13px; color: var(--text); line-height: 1.6; }
.why-cards { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; }
.why-card {
  background: var(--navy-3); border: 1px solid var(--border-2);
  border-radius: 16px; padding: 28px; text-align: center; transition: all 0.3s;
}
.why-card:hover { border-color: var(--border); transform: translateY(-3px); }
.why-card:first-child { grid-column: 1 / -1; }
.wc-val {
  font-family: 'Space Grotesk', sans-serif; font-size: 22px; font-weight: 700;
  background: linear-gradient(135deg, var(--blue), var(--blue-2));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
  margin-bottom: 8px;
}
.wc-lbl { font-size: 13px; color: var(--text); line-height: 1.5; }

/* === INDUSTRIES === */
.industries-section { background: var(--navy); }
.ind-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
.ind-card {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 14px;
  padding: 22px 18px; display: flex; align-items: center; gap: 14px; transition: all 0.3s;
}
.ind-card:hover { border-color: var(--border); transform: translateY(-3px); }
.ind-ico { font-size: 26px; flex-shrink: 0; }
.ind-card h4 { font-size: 14px; font-weight: 600; color: var(--white); margin-bottom: 4px; }
.ind-card p { font-size: 12px; color: var(--text); }

/* === TECH STACK === */
.tech-section {
  padding: 56px 32px;
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
  background: rgba(17,34,64,0.3);
}
.tech-inner { max-width: 1100px; margin: 0 auto; text-align: center; }
.tech-inner .sec-label { margin-bottom: 24px; }
.tech-badges { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; }
.tbadge {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 8px;
  padding: 8px 18px; font-size: 13px; font-weight: 500;
  color: var(--text-2); transition: all 0.2s;
}
.tbadge:hover { border-color: var(--border); color: var(--white); }

/* === CONTACT === */
.contact-section {
  background: var(--navy); position: relative; overflow: hidden;
}
.contact-section::before {
  content: ''; position: absolute; top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 900px; height: 400px;
  background: radial-gradient(ellipse, rgba(14,165,233,0.06) 0%, transparent 70%);
  pointer-events: none;
}
.contact-inner {
  max-width: 1100px; margin: 0 auto;
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 72px; align-items: start; position: relative; z-index: 1;
}
.contact-info h2 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(26px, 2.8vw, 40px); font-weight: 700; letter-spacing: -0.8px;
  color: var(--white); margin-bottom: 16px; line-height: 1.2;
}
.contact-info > p { font-size: 16px; color: var(--text-2); line-height: 1.75; margin-bottom: 36px; }
.c-methods { display: flex; flex-direction: column; gap: 16px; }
.c-method {
  display: flex; align-items: center; gap: 14px;
  text-decoration: none; color: var(--text-2); transition: color 0.2s;
  padding: 14px 16px; border-radius: 12px; border: 1px solid var(--border-2);
  background: rgba(6,13,26,0.3); transition: all 0.2s;
}
.c-method:hover { color: var(--white); border-color: var(--border); background: rgba(14,165,233,0.05); }
.c-ico {
  width: 42px; height: 42px; border-radius: 10px;
  background: rgba(14,165,233,0.1); border: 1px solid rgba(14,165,233,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 18px; flex-shrink: 0;
}
.c-lbl { font-size: 10px; text-transform: uppercase; letter-spacing: 1px; color: var(--text); margin-bottom: 3px; }
.c-val { font-size: 15px; font-weight: 500; }

/* Contact form */
.c-form-box {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 20px; padding: 36px 30px;
}
.c-form-box::before {
  content: ''; display: block; margin: -36px -30px 28px;
  height: 2px; border-radius: 20px 20px 0 0;
  background: linear-gradient(90deg, transparent, var(--blue), transparent);
}
.cf-head {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 20px; font-weight: 600; color: var(--white); margin-bottom: 6px;
}
.cf-sub { font-size: 13px; color: var(--text); margin-bottom: 26px; }
.fg { margin-bottom: 14px; }
.fg label {
  display: block; font-size: 11px; font-weight: 600; letter-spacing: 0.5px;
  text-transform: uppercase; color: var(--text-2); margin-bottom: 7px;
}
.fg input, .fg select, .fg textarea {
  width: 100%; background: rgba(6,13,26,0.7); border: 1px solid rgba(255,255,255,0.08);
  border-radius: 9px; padding: 11px 14px; font-size: 14px; color: var(--white);
  font-family: 'Inter', sans-serif; outline: none; resize: none; transition: border-color 0.2s;
}
.fg input:focus, .fg select:focus, .fg textarea:focus {
  border-color: rgba(14,165,233,0.4); box-shadow: 0 0 0 3px rgba(14,165,233,0.07);
}
.fg input::placeholder, .fg textarea::placeholder { color: var(--text); }
.fg select option { background: var(--navy-2); color: var(--white); }
.fg-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
.cf-submit {
  width: 100%; background: linear-gradient(135deg, var(--blue), #0284C7);
  color: white; border: none; border-radius: 9px; padding: 13px;
  font-size: 15px; font-weight: 600; cursor: pointer;
  font-family: 'Inter', sans-serif; transition: all 0.3s;
  box-shadow: 0 4px 20px rgba(14,165,233,0.28); margin-top: 6px;
}
.cf-submit:hover { transform: translateY(-2px); box-shadow: 0 8px 32px rgba(14,165,233,0.44); }

/* === FOOTER === */
.footer {
  background: var(--navy);
  border-top: 1px solid var(--border-2);
  padding: 44px 32px;
}
.footer-inner {
  max-width: 1200px; margin: 0 auto;
  display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 22px;
}
.f-brand { display: flex; align-items: center; gap: 10px; }
.f-brand img { height: 28px; }
.f-brand-name {
  font-family: 'Space Grotesk', sans-serif; font-weight: 700; font-size: 15px; color: var(--white);
}
.f-links { display: flex; gap: 28px; flex-wrap: wrap; }
.f-links a { font-size: 13px; color: var(--text); text-decoration: none; transition: color 0.2s; }
.f-links a:hover { color: var(--white); }
.f-copy { font-size: 12px; color: var(--text); }

/* === RESPONSIVE === */
@media (max-width: 960px) {
  .hero-inner { grid-template-columns: 1fr; gap: 40px; }
  .hero-visual { display: none; }
  .services-grid { grid-template-columns: 1fr; }
  .steps-row { grid-template-columns: 1fr 1fr; }
  .steps-row::before { display: none; }
  .why-grid { grid-template-columns: 1fr; gap: 40px; }
  .contact-inner { grid-template-columns: 1fr; gap: 40px; }
  .ind-grid { grid-template-columns: 1fr 1fr; }
}
@media (max-width: 640px) {
  .nav-links { display: none; }
  section { padding: 64px 20px; }
  .steps-row { grid-template-columns: 1fr; }
  .why-cards { grid-template-columns: 1fr; }
  .why-card:first-child { grid-column: 1; }
  .ind-grid { grid-template-columns: 1fr; }
  .fg-row { grid-template-columns: 1fr; }
  .footer-inner { flex-direction: column; text-align: center; }
  .trust-bar-inner { gap: 24px; }
  .panel-metrics { grid-template-columns: 1fr 1fr; }
}
</style>

<div class="apex-site">

<!-- ======================== NAVBAR ======================== -->
<nav class="nav">
  <div class="nav-inner">
    <a href="#" class="nav-logo">
      <img src="apex_logo.PNG" alt="Apex Data Cloud">
      <span class="nav-logo-text">Apex <span>Data</span> Cloud</span>
    </a>
    <ul class="nav-links">
      <li><a href="#services">Services</a></li>
      <li><a href="#approach">Approach</a></li>
      <li><a href="#why-apex">Why Apex</a></li>
      <li><a href="#industries">Industries</a></li>
      <li><a href="#contact" class="nav-cta">Get in Touch</a></li>
    </ul>
  </div>
</nav>

<!-- ======================== HERO ======================== -->
<section class="hero">
  <div class="hero-grid-bg"></div>
  <div class="hero-glow-1"></div>
  <div class="hero-glow-2"></div>
  <div class="hero-inner">
    <div>
      <div class="hero-badge">
        <span class="live-dot"></span>
        AI &amp; Data Strategy Consulting
      </div>
      <h1>Turn Data Into<br><span class="hl">Competitive Edge</span></h1>
      <p>We partner with executives, operators, and founders to transform complex data into decisive strategy—combining timeless business principles with modern AI and analytical capabilities.</p>
      <div class="hero-cta">
        <a href="#contact" class="btn-primary">Start a Conversation &#8594;</a>
        <a href="#services" class="btn-ghost">Explore Services</a>
      </div>
    </div>
    <div class="hero-visual">
      <div class="hero-panel">
        <div class="panel-label">Core Capabilities</div>
        <div class="panel-metrics">
          <div class="pm-card">
            <div class="pm-val">AI / ML</div>
            <div class="pm-lbl">Advisory &amp; Deploy</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">Cloud</div>
            <div class="pm-lbl">Architecture</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">Strategy</div>
            <div class="pm-lbl">Data &amp; Digital</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">Analytics</div>
            <div class="pm-lbl">Predictive</div>
          </div>
        </div>
        <div class="panel-pills">
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(14,165,233,0.12);">&#128202;</div>
            Predictive Analytics &amp; Forecasting
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(245,158,11,0.12);">&#129302;</div>
            AI &amp; Machine Learning Deployment
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(16,185,129,0.12);">&#9729;&#65039;</div>
            Cloud Platform Optimization
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(139,92,246,0.12);">&#128300;</div>
            Business &amp; Digital Strategy
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== TRUST BAR ======================== -->
<div class="trust-bar">
  <div class="trust-bar-inner">
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Advisor-First Philosophy
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Evidence-Based Strategy
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      End-to-End Execution
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Measurable Business Outcomes
    </div>
  </div>
</div>

<!-- ======================== SERVICES ======================== -->
<section id="services" class="services-section">
  <div class="container">
    <div class="sec-header">
      <div class="sec-label">What We Do</div>
      <h2 class="sec-title">Advisory &amp; Implementation Services</h2>
      <p class="sec-sub">We work at the intersection of strategy, analytics, and execution—aligning every data initiative directly to measurable business outcomes.</p>
    </div>
    <div class="services-grid">
      <div class="svc-card">
        <div class="svc-icon">&#128202;</div>
        <h3>Strategic Analytics &amp; Predictive Insight</h3>
        <p>We identify the metrics that matter, uncover performance drivers, and model future scenarios to support confident, evidence-based decisions at every level of the organization.</p>
        <div class="svc-tags">
          <span class="tag">KPI Design</span>
          <span class="tag">Forecasting</span>
          <span class="tag">Scenario Modeling</span>
          <span class="tag">Executive Dashboards</span>
        </div>
      </div>
      <div class="svc-card">
        <div class="svc-icon">&#129302;</div>
        <h3>AI &amp; Machine Learning Advisory</h3>
        <p>From use-case definition to model governance and production deployment, we help organizations apply AI pragmatically—where it delivers real value, not experimentation for its own sake.</p>
        <div class="svc-tags">
          <span class="tag">Use-Case Discovery</span>
          <span class="tag">Model Development</span>
          <span class="tag">MLOps</span>
          <span class="tag">AI Governance</span>
        </div>
      </div>
      <div class="svc-card">
        <div class="svc-icon">&#128300;</div>
        <h3>Business, Data &amp; Digital Strategy</h3>
        <p>We assess your current state, define a clear roadmap, and guide execution—turning ambiguity into structured, achievable initiatives aligned with your strategic objectives.</p>
        <div class="svc-tags">
          <span class="tag">Data Roadmap</span>
          <span class="tag">Digital Transformation</span>
          <span class="tag">Change Management</span>
          <span class="tag">OKR Alignment</span>
        </div>
      </div>
      <div class="svc-card">
        <div class="svc-icon">&#9729;&#65039;</div>
        <h3>Cloud, Platform &amp; Operating Model</h3>
        <p>We design scalable, secure cloud environments and data operating models that support sustained growth, organizational resilience, and rigorous cost discipline.</p>
        <div class="svc-tags">
          <span class="tag">Cloud Architecture</span>
          <span class="tag">Data Platform</span>
          <span class="tag">Cost Optimization</span>
          <span class="tag">Security &amp; Governance</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== APPROACH ======================== -->
<section id="approach" class="approach-section">
  <div class="container">
    <div class="sec-header">
      <div class="sec-label">How We Work</div>
      <h2 class="sec-title">A Disciplined, Four-Phase Approach</h2>
      <p class="sec-sub">Meaningful transformation starts with clarity. Our structured methodology ensures every engagement delivers durable, measurable results.</p>
    </div>
    <div class="steps-row">
      <div class="step">
        <div class="step-num">01</div>
        <h4>Discover &amp; Diagnose</h4>
        <p>We immerse ourselves in your business context, data landscape, and strategic goals to establish a clear picture of where you are and where you need to go.</p>
      </div>
      <div class="step">
        <div class="step-num">02</div>
        <h4>Strategize &amp; Design</h4>
        <p>We develop a prioritized roadmap—identifying highest-impact opportunities and designing the right solutions before a single line of code is written.</p>
      </div>
      <div class="step">
        <div class="step-num">03</div>
        <h4>Build &amp; Deploy</h4>
        <p>Our team executes with precision—building scalable models, platforms, and processes that integrate seamlessly into your existing operations.</p>
      </div>
      <div class="step">
        <div class="step-num">04</div>
        <h4>Measure &amp; Optimize</h4>
        <p>We establish feedback loops, track performance against business KPIs, and continuously refine to ensure sustained competitive advantage.</p>
      </div>
    </div>
  </div>
</section>

<!-- ======================== WHY APEX ======================== -->
<section id="why-apex" class="why-section">
  <div class="container">
    <div class="why-grid">
      <div class="why-content">
        <div class="sec-label">Why Choose Apex</div>
        <h2>Trusted Advisors First.<br>Technologists Second.</h2>
        <p>Meaningful transformation doesn't start with tools—it starts with clarity, disciplined thinking, and informed judgment. We bring both strategic depth and technical excellence to every engagement.</p>
        <div class="diffs">
          <div class="diff">
            <div class="diff-ico">&#127919;</div>
            <div>
              <h4>Outcome-Oriented Engagements</h4>
              <p>Every recommendation ties to a measurable business result. We don't deliver reports—we deliver impact.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico">&#128275;</div>
            <div>
              <h4>Uncompromising Clarity</h4>
              <p>We translate complex data realities into language leadership teams can act on immediately and confidently.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico">&#9881;&#65039;</div>
            <div>
              <h4>Pragmatic AI Deployment</h4>
              <p>We apply AI where it genuinely creates value—with robust governance and a clear path to production.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico">&#128736;&#65039;</div>
            <div>
              <h4>End-to-End Partnership</h4>
              <p>From strategy through deployment and optimization—one trusted partner across the full data journey.</p>
            </div>
          </div>
        </div>
      </div>
      <div class="why-cards">
        <div class="why-card">
          <div class="wc-val">Strategy + Execution</div>
          <div class="wc-lbl">We bridge the gap between boardroom strategy and engineering delivery, ensuring nothing gets lost in translation.</div>
        </div>
        <div class="why-card">
          <div class="wc-val">AI-Native</div>
          <div class="wc-lbl">Modern ML tooling built into every engagement from day one.</div>
        </div>
        <div class="why-card">
          <div class="wc-val">ROI-Focused</div>
          <div class="wc-lbl">Every initiative measured against clear business KPIs and financial outcomes.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== INDUSTRIES ======================== -->
<section id="industries" class="industries-section">
  <div class="container">
    <div class="sec-header">
      <div class="sec-label">Industries We Serve</div>
      <h2 class="sec-title">Deep Domain Expertise</h2>
      <p class="sec-sub">We bring industry-specific context to every engagement, ensuring solutions address real-world constraints and opportunities unique to your sector.</p>
    </div>
    <div class="ind-grid">
      <div class="ind-card">
        <div class="ind-ico">&#127970;</div>
        <div>
          <h4>Financial Services</h4>
          <p>Risk modeling, fraud detection, regulatory analytics</p>
        </div>
      </div>
      <div class="ind-card">
        <div class="ind-ico">&#128138;</div>
        <div>
          <h4>Healthcare &amp; Life Sciences</h4>
          <p>Clinical analytics, patient outcomes, operational efficiency</p>
        </div>
      </div>
      <div class="ind-card">
        <div class="ind-ico">&#128722;</div>
        <div>
          <h4>Retail &amp; E-Commerce</h4>
          <p>Demand forecasting, personalization, supply chain optimization</p>
        </div>
      </div>
      <div class="ind-card">
        <div class="ind-ico">&#128679;</div>
        <div>
          <h4>Manufacturing &amp; Operations</h4>
          <p>Predictive maintenance, process optimization, IoT analytics</p>
        </div>
      </div>
      <div class="ind-card">
        <div class="ind-ico">&#128640;</div>
        <div>
          <h4>Technology &amp; SaaS</h4>
          <p>Product analytics, growth metrics, churn and retention modeling</p>
        </div>
      </div>
      <div class="ind-card">
        <div class="ind-ico">&#127968;</div>
        <div>
          <h4>Real Estate &amp; PropTech</h4>
          <p>Market intelligence, valuation models, portfolio analytics</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== TECH STACK ======================== -->
<div class="tech-section">
  <div class="tech-inner">
    <div class="sec-label">Technology Ecosystem</div>
    <div class="tech-badges">
      <span class="tbadge">Python</span>
      <span class="tbadge">Apache Spark</span>
      <span class="tbadge">dbt</span>
      <span class="tbadge">Snowflake</span>
      <span class="tbadge">BigQuery</span>
      <span class="tbadge">Databricks</span>
      <span class="tbadge">AWS</span>
      <span class="tbadge">Google Cloud</span>
      <span class="tbadge">Azure</span>
      <span class="tbadge">Tableau</span>
      <span class="tbadge">Power BI</span>
      <span class="tbadge">TensorFlow</span>
      <span class="tbadge">PyTorch</span>
      <span class="tbadge">Apache Airflow</span>
      <span class="tbadge">Kafka</span>
      <span class="tbadge">Looker</span>
    </div>
  </div>
</div>

<!-- ======================== CONTACT ======================== -->
<section id="contact" class="contact-section">
  <div class="contact-inner">
    <div class="contact-info">
      <div class="sec-label">Get in Touch</div>
      <h2>Let's Build Something<br>Extraordinary Together</h2>
      <p>Whether you're looking to modernize your data infrastructure, deploy AI at scale, or clarify your data strategy—we're ready to help you move forward with confidence.</p>
      <div class="c-methods">
        <a href="mailto:ezequiel@apexdata.cloud" class="c-method">
          <div class="c-ico">&#9993;&#65039;</div>
          <div>
            <div class="c-lbl">Email</div>
            <div class="c-val">ezequiel@apexdata.cloud</div>
          </div>
        </a>
        <a href="tel:+13057788223" class="c-method">
          <div class="c-ico">&#128222;</div>
          <div>
            <div class="c-lbl">Phone (US)</div>
            <div class="c-val">+1 305 778 8223</div>
          </div>
        </a>
      </div>
    </div>
    <!-- To activate form submissions: sign up at formspree.io and replace YOUR_FORM_ID below -->
    <div class="c-form-box">
      <div class="cf-head">Start a Conversation</div>
      <div class="cf-sub">Tell us about your challenge. We'll respond within one business day.</div>
      <form action="https://formspree.io/f/https://formspree.io/f/xqedrddj" method="POST">
        <div class="fg-row">
          <div class="fg">
            <label>First Name</label>
            <input type="text" name="first_name" placeholder="John" required>
          </div>
          <div class="fg">
            <label>Last Name</label>
            <input type="text" name="last_name" placeholder="Smith" required>
          </div>
        </div>
        <div class="fg">
          <label>Work Email</label>
          <input type="email" name="email" placeholder="john@company.com" required>
        </div>
        <div class="fg">
          <label>Company</label>
          <input type="text" name="company" placeholder="Company name">
        </div>
        <div class="fg">
          <label>Area of Interest</label>
          <select name="interest">
            <option value="" disabled selected>Select a service...</option>
            <option>Strategic Analytics &amp; Predictive Insight</option>
            <option>AI &amp; Machine Learning Advisory</option>
            <option>Business, Data &amp; Digital Strategy</option>
            <option>Cloud &amp; Platform Optimization</option>
            <option>General Inquiry</option>
          </select>
        </div>
        <div class="fg">
          <label>Message</label>
          <textarea name="message" rows="4" placeholder="Briefly describe your challenge or objective..."></textarea>
        </div>
        <button type="submit" class="cf-submit">Send Message &#8594;</button>
      </form>
    </div>
  </div>
</section>

<!-- ======================== FOOTER ======================== -->
<footer class="footer">
  <div class="footer-inner">
    <div class="f-brand">
      <img src="apex_logo.PNG" alt="Apex Data Cloud">
      <span class="f-brand-name">Apex Data Cloud</span>
    </div>
    <div class="f-links">
      <a href="#services">Services</a>
      <a href="#approach">Approach</a>
      <a href="#industries">Industries</a>
      <a href="#contact">Contact</a>
      <a href="mailto:ezequiel@apexdata.cloud">Email Us</a>
    </div>
    <div class="f-copy">&copy; 2026 Apex Data Cloud. All rights reserved.</div>
  </div>
</footer>

</div><!-- end .apex-site -->

<script src="https://www.gstatic.com/dialogflow-console/fast/messenger/bootstrap.js?v=1"></script>
<df-messenger
  intent="WELCOME"
  chat-title="Harvey"
  agent-id="54ef4ef9-6e87-4fa1-af93-c16c4dcfcb6f"
  language-code="en"
></df-messenger>
