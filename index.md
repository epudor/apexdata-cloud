---
layout: default
title: "Apex Data & Marketing Cloud | AI-Powered Marketing Intelligence Consulting"
description: "We help CMOs, founders, and growth teams turn customer data into measurable revenue — combining AI, customer segmentation, marketing analytics, and predictive intelligence to drive sustainable growth."
image: "/apex_logo.PNG"
author: "Apex Data & Marketing Cloud"
lang: en-US
---

<!-- Performance: Preconnect to external origins -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="preconnect" href="https://www.googletagmanager.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Space+Grotesk:wght@500;600;700;800&display=swap" rel="stylesheet">

<!-- Fallback SEO meta injection (for Jekyll themes that don't load head-custom.html) -->
<script>
(function(){
  var head = document.head;
  var tags = [
    ['meta', {property:'og:type', content:'website'}],
    ['meta', {property:'og:title', content:'Apex Data & Marketing Cloud | AI-Powered Marketing Intelligence Consulting'}],
    ['meta', {property:'og:description', content:'We help CMOs, founders, and growth teams turn customer data into measurable revenue — combining AI, customer segmentation, marketing analytics, and predictive intelligence.'}],
    ['meta', {property:'og:image', content:'https://apexdata.cloud/apex_logo.PNG'}],
    ['meta', {property:'og:site_name', content:'Apex Data & Marketing Cloud'}],
    ['meta', {name:'twitter:card', content:'summary_large_image'}],
    ['meta', {name:'twitter:title', content:'Apex Data & Marketing Cloud | AI-Powered Marketing Intelligence Consulting'}],
    ['link', {rel:'canonical', href:'https://apexdata.cloud/'}]
  ];
  tags.forEach(function(t){
    if(!head.querySelector('[property="'+t[1].property+'"], [name="'+t[1].name+'"], [rel="canonical"]')){
      var el=document.createElement(t[0]);
      for(var k in t[1]) el.setAttribute(k,t[1][k]);
      head.appendChild(el);
    }
  });
})();
</script>

<style>
/* ============================================================
   RESET & JEKYLL OVERRIDES
   ============================================================ */
.page-content { padding: 0 !important; }
.wrapper { max-width: 100% !important; padding: 0 !important; }
.site-header, .site-footer { display: none !important; }
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }

/* ============================================================
   DESIGN TOKENS
   ============================================================ */
:root {
  --navy:      #060D1A;
  --navy-2:    #0A1628;
  --navy-3:    #112240;
  --navy-4:    #1a3a6b;
  --blue:      #F1C6D3;
  --blue-2:    #EAA0B5;
  --blue-3:    #F8DDE5;
  --rose:      #C96B87;
  --gold:      #F59E0B;
  --green:     #10B981;
  --white:     #F8FAFC;
  --text:      #94A3B8;
  --text-2:    #CBD5E1;
  --border:    rgba(241,198,211,0.22);
  --border-2:  rgba(241,198,211,0.09);
  --shadow-sm: 0 4px 20px rgba(0,0,0,0.35);
  --shadow-md: 0 12px 40px rgba(0,0,0,0.45);
  --shadow-glow: 0 8px 36px rgba(241,198,211,0.28);
}

/* ============================================================
   BASE
   ============================================================ */
.apex-site {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  background: var(--navy);
  color: var(--white);
  overflow-x: hidden;
  line-height: 1.6;
}

/* ============================================================
   SCROLL PROGRESS BAR
   ============================================================ */
.scroll-progress {
  position: fixed; top: 0; left: 0; height: 2px; z-index: 9999;
  background: linear-gradient(90deg, var(--blue), var(--rose), var(--gold));
  width: 0%; transition: width 0.08s linear;
}

/* ============================================================
   NAVBAR
   ============================================================ */
.nav {
  position: fixed; top: 2px; left: 0; right: 0; z-index: 1000;
  padding: 14px 32px;
  background: rgba(6,13,26,0.88);
  backdrop-filter: blur(24px);
  -webkit-backdrop-filter: blur(24px);
  border-bottom: 1px solid var(--border-2);
  transition: padding 0.3s, background 0.3s;
}
.nav.scrolled {
  padding: 10px 32px;
  background: rgba(6,13,26,0.97);
  border-bottom-color: var(--border);
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
.nav-logo-text span { color: var(--blue-2); }
.nav-links {
  display: flex; align-items: center; gap: 28px; list-style: none;
}
.nav-links a {
  font-size: 14px; font-weight: 500; color: var(--text-2);
  text-decoration: none; transition: color 0.2s;
}
.nav-links a:hover { color: var(--white); }
.nav-cta {
  background: linear-gradient(135deg, var(--blue), var(--rose)) !important;
  color: #060D1A !important;
  padding: 9px 22px; border-radius: 8px; font-weight: 700 !important;
  box-shadow: var(--shadow-glow); transition: all 0.3s;
}
.nav-cta:hover {
  transform: translateY(-1px);
  box-shadow: 0 6px 28px rgba(241,198,211,0.48) !important;
  color: #060D1A !important;
}

/* Hamburger */
.hamburger-btn {
  display: none; background: none; border: none; cursor: pointer;
  padding: 6px; flex-direction: column; gap: 5px; z-index: 1100;
}
.hamburger-btn span {
  display: block; width: 22px; height: 2px; background: var(--white);
  border-radius: 2px; transition: all 0.3s;
}
.hamburger-btn.open span:nth-child(1) { transform: translateY(7px) rotate(45deg); }
.hamburger-btn.open span:nth-child(2) { opacity: 0; }
.hamburger-btn.open span:nth-child(3) { transform: translateY(-7px) rotate(-45deg); }

/* Mobile menu overlay */
.mobile-menu {
  display: none; position: fixed; inset: 0; z-index: 1050;
  background: rgba(6,13,26,0.98); backdrop-filter: blur(20px);
  flex-direction: column; align-items: center; justify-content: center; gap: 36px;
  opacity: 0; transition: opacity 0.3s;
}
.mobile-menu.active { display: flex; opacity: 1; }
.mobile-menu a {
  font-family: 'Space Grotesk', sans-serif; font-size: 28px; font-weight: 700;
  color: var(--white); text-decoration: none; transition: color 0.2s;
}
.mobile-menu a:hover { color: var(--blue-2); }
.mobile-menu .m-cta {
  background: linear-gradient(135deg, var(--blue), var(--rose));
  color: #060D1A !important; padding: 14px 36px; border-radius: 12px;
  font-size: 20px;
}

/* ============================================================
   SCROLL REVEAL ANIMATION
   ============================================================ */
.reveal {
  opacity: 0; transform: translateY(28px);
  transition: opacity 0.75s cubic-bezier(.22,1,.36,1), transform 0.75s cubic-bezier(.22,1,.36,1);
}
.reveal.visible { opacity: 1; transform: none; }
.reveal-delay-1 { transition-delay: 0.1s; }
.reveal-delay-2 { transition-delay: 0.2s; }
.reveal-delay-3 { transition-delay: 0.3s; }
.reveal-delay-4 { transition-delay: 0.4s; }
.reveal-delay-5 { transition-delay: 0.5s; }

/* ============================================================
   HERO
   ============================================================ */
.hero {
  min-height: 100vh;
  display: flex; align-items: center;
  padding: 140px 32px 100px;
  position: relative; overflow: hidden;
  background: var(--navy);
}
.hero-grid-bg {
  position: absolute; inset: 0; pointer-events: none;
  background-image:
    linear-gradient(rgba(241,198,211,0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(241,198,211,0.03) 1px, transparent 1px);
  background-size: 64px 64px;
  animation: gridShift 30s linear infinite;
}
@keyframes gridShift {
  0% { background-position: 0 0; }
  100% { background-position: 64px 64px; }
}
.hero-glow-1 {
  position: absolute; top: -5%; right: -5%; width: 800px; height: 800px;
  background: radial-gradient(circle, rgba(241,198,211,0.09) 0%, transparent 65%);
  pointer-events: none; animation: breathe 8s ease-in-out infinite;
}
.hero-glow-2 {
  position: absolute; bottom: -15%; left: -8%; width: 600px; height: 600px;
  background: radial-gradient(circle, rgba(245,158,11,0.055) 0%, transparent 65%);
  pointer-events: none; animation: breathe 10s ease-in-out infinite reverse;
}
.hero-glow-3 {
  position: absolute; top: 40%; left: 30%; width: 400px; height: 400px;
  background: radial-gradient(circle, rgba(201,107,135,0.04) 0%, transparent 65%);
  pointer-events: none; animation: breathe 12s ease-in-out infinite;
}
@keyframes breathe {
  0%, 100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.1); opacity: 0.8; }
}
.hero-inner {
  max-width: 1200px; margin: 0 auto;
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 72px; align-items: center; width: 100%; position: relative; z-index: 1;
}

/* Hero left */
.hero-badge {
  display: inline-flex; align-items: center; gap: 7px;
  background: rgba(241,198,211,0.08); border: 1px solid rgba(241,198,211,0.28);
  border-radius: 50px; padding: 5px 16px;
  font-size: 11px; font-weight: 600; letter-spacing: 1.5px;
  text-transform: uppercase; color: var(--blue-2); margin-bottom: 22px;
}
.live-dot {
  width: 7px; height: 7px; border-radius: 50%; background: var(--green);
  animation: pulse-dot 2.2s infinite;
}
@keyframes pulse-dot {
  0%, 100% { opacity: 1; transform: scale(1); box-shadow: 0 0 0 0 rgba(16,185,129,0.5); }
  50% { opacity: 0.7; transform: scale(0.85); box-shadow: 0 0 0 6px rgba(16,185,129,0); }
}
.hero h1 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(36px, 4.8vw, 62px);
  font-weight: 800; line-height: 1.07; letter-spacing: -2px;
  color: var(--white); margin-bottom: 22px;
}
.hero h1 .hl {
  background: linear-gradient(130deg, var(--blue) 0%, var(--blue-2) 50%, var(--rose) 100%);
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
}
.hero p {
  font-size: 17px; line-height: 1.78; color: var(--text-2);
  margin-bottom: 40px; max-width: 500px;
}
.hero-cta { display: flex; gap: 14px; flex-wrap: wrap; align-items: center; }

.btn-primary {
  display: inline-flex; align-items: center; gap: 9px;
  background: linear-gradient(135deg, var(--blue), var(--rose));
  color: #060D1A; padding: 15px 32px; border-radius: 10px;
  font-size: 15px; font-weight: 700; text-decoration: none;
  border: none; cursor: pointer; transition: all 0.3s;
  box-shadow: var(--shadow-glow); white-space: nowrap;
}
.btn-primary:hover { transform: translateY(-2px); box-shadow: 0 10px 42px rgba(241,198,211,0.48); }
.btn-ghost {
  display: inline-flex; align-items: center; gap: 9px;
  background: transparent; color: var(--text-2);
  padding: 15px 28px; border-radius: 10px; font-size: 15px; font-weight: 500;
  text-decoration: none; border: 1px solid rgba(255,255,255,0.12); transition: all 0.3s;
  white-space: nowrap;
}
.btn-ghost:hover { color: var(--white); border-color: rgba(255,255,255,0.3); background: rgba(255,255,255,0.05); }

/* Hero right panel */
.hero-panel {
  background: rgba(17,34,64,0.7);
  border: 1px solid var(--border);
  border-radius: 22px; padding: 30px;
  backdrop-filter: blur(16px); position: relative;
  box-shadow: var(--shadow-md);
}
.hero-panel::before {
  content: ''; position: absolute; top: -1px; left: 22%; right: 22%;
  height: 1px; background: linear-gradient(90deg, transparent, var(--blue), var(--rose), transparent);
}
.panel-label {
  font-size: 10px; font-weight: 700; letter-spacing: 2.5px;
  text-transform: uppercase; color: var(--text); margin-bottom: 20px;
}
.panel-metrics {
  display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 18px;
}
.pm-card {
  background: rgba(6,13,26,0.65); border: 1px solid var(--border-2);
  border-radius: 12px; padding: 14px; text-align: center;
  transition: border-color 0.2s;
}
.pm-card:hover { border-color: var(--border); }
.pm-val {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 14px; font-weight: 700; color: var(--blue-2); margin-bottom: 3px;
}
.pm-lbl { font-size: 11px; color: var(--text); }
.panel-pills { display: flex; flex-direction: column; gap: 8px; }
.ppill {
  display: flex; align-items: center; gap: 12px;
  background: rgba(6,13,26,0.5); border: 1px solid var(--border-2);
  border-radius: 10px; padding: 11px 14px;
  font-size: 13px; color: var(--text-2); transition: all 0.25s;
}
.ppill:hover { border-color: var(--border); color: var(--white); background: rgba(241,198,211,0.04); }
.ppill-icon {
  width: 32px; height: 32px; border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-size: 16px; flex-shrink: 0;
}
.ppill-arrow { margin-left: auto; color: var(--text); font-size: 12px; }

/* ============================================================
   TRUST BAR
   ============================================================ */
.trust-bar {
  padding: 22px 32px;
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
  background: rgba(17,34,64,0.4);
}
.trust-bar-inner {
  max-width: 1200px; margin: 0 auto;
  display: flex; align-items: center; justify-content: center;
  gap: 48px; flex-wrap: wrap;
}
.t-item {
  display: flex; align-items: center; gap: 8px;
  font-size: 13px; font-weight: 500; color: var(--text);
}
.t-item svg { color: var(--green); flex-shrink: 0; }

/* ============================================================
   COMMON SECTION STYLES
   ============================================================ */
section { padding: 100px 32px; }
.container { max-width: 1200px; margin: 0 auto; }
.sec-header { text-align: center; margin-bottom: 64px; }
.sec-label {
  display: inline-block; font-size: 11px; font-weight: 700;
  letter-spacing: 2.5px; text-transform: uppercase;
  color: var(--blue-2); margin-bottom: 14px;
}
.sec-title {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(28px, 3.5vw, 46px);
  font-weight: 700; letter-spacing: -1px;
  color: var(--white); margin-bottom: 18px; line-height: 1.18;
}
.sec-sub {
  font-size: 17px; color: var(--text-2);
  max-width: 580px; margin: 0 auto; line-height: 1.78;
}

/* ============================================================
   IMPACT STATS
   ============================================================ */
.stats-section {
  padding: 80px 32px;
  background: linear-gradient(180deg, var(--navy-3) 0%, var(--navy-2) 100%);
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
}
.stats-grid {
  max-width: 1000px; margin: 0 auto;
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 28px; text-align: center;
}
.stat-item { padding: 8px; }
.stat-num {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(36px, 4vw, 56px); font-weight: 800; line-height: 1;
  background: linear-gradient(135deg, var(--blue), var(--blue-2));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
  margin-bottom: 10px; display: block;
}
.stat-label { font-size: 15px; font-weight: 600; color: var(--white); margin-bottom: 6px; }
.stat-sublabel { font-size: 13px; color: var(--text); line-height: 1.4; }
.stat-divider {
  width: 1px; background: var(--border-2);
  display: none;
}

/* ============================================================
   SERVICES
   ============================================================ */
.services-section { background: var(--navy); }
.services-grid {
  display: grid; grid-template-columns: repeat(3, 1fr); gap: 22px;
}
.services-primary-grid {
  display: grid; grid-template-columns: repeat(2, 1fr); gap: 22px; margin-bottom: 0;
}
.capabilities-subheader {
  text-align: center; margin: 72px 0 48px;
  padding-top: 64px; border-top: 1px solid var(--border-2);
}
.capabilities-subheader .sec-label { margin-bottom: 14px; display: block; }
.svc-card {
  background: var(--navy-3); border: 1px solid var(--border-2);
  border-radius: 20px; padding: 36px 28px;
  transition: all 0.35s; position: relative; overflow: hidden;
  display: flex; flex-direction: column;
}
.svc-card::after {
  content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
  background: linear-gradient(90deg, transparent, var(--blue), var(--rose), transparent);
  transform: scaleX(0); transform-origin: center; transition: transform 0.4s;
}
.svc-card:hover { border-color: var(--border); transform: translateY(-6px); box-shadow: 0 24px 56px rgba(241,198,211,0.10); }
.svc-card:hover::after { transform: scaleX(1); }
.svc-icon {
  width: 54px; height: 54px; border-radius: 15px;
  background: rgba(241,198,211,0.1); border: 1px solid rgba(241,198,211,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 24px; margin-bottom: 22px; flex-shrink: 0;
  transition: background 0.3s;
}
.svc-card:hover .svc-icon { background: rgba(241,198,211,0.18); }
.svc-new-badge {
  position: absolute; top: 20px; right: 20px;
  background: linear-gradient(135deg, var(--gold), #D97706);
  color: #060D1A; font-size: 9px; font-weight: 800; letter-spacing: 1.2px;
  text-transform: uppercase; padding: 3px 9px; border-radius: 50px;
}
.svc-card h3 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 18px; font-weight: 700; color: var(--white); margin-bottom: 12px;
  line-height: 1.3;
}
.svc-card p { font-size: 14px; color: var(--text-2); line-height: 1.75; margin-bottom: 22px; flex: 1; }
.svc-tags { display: flex; flex-wrap: wrap; gap: 7px; margin-bottom: 20px; }
.tag {
  font-size: 11px; font-weight: 500; color: var(--blue-3);
  background: rgba(241,198,211,0.08); border: 1px solid rgba(241,198,211,0.15);
  border-radius: 50px; padding: 3px 12px; white-space: nowrap;
}
.svc-link {
  display: inline-flex; align-items: center; gap: 6px;
  font-size: 13px; font-weight: 600; color: var(--blue-2);
  text-decoration: none; transition: gap 0.2s;
  margin-top: auto;
}
.svc-link:hover { gap: 10px; }

/* ============================================================
   MID-PAGE CTA BANNER
   ============================================================ */
.cta-banner {
  padding: 88px 32px; position: relative; overflow: hidden;
  background: linear-gradient(135deg,
    rgba(241,198,211,0.06) 0%,
    rgba(201,107,135,0.06) 50%,
    rgba(245,158,11,0.04) 100%);
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
}
.cta-banner::before {
  content: ''; position: absolute; top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 1000px; height: 400px;
  background: radial-gradient(ellipse, rgba(241,198,211,0.05) 0%, transparent 70%);
  pointer-events: none;
}
.cta-banner-inner {
  max-width: 700px; margin: 0 auto;
  text-align: center; position: relative; z-index: 1;
}
.cta-banner h2 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(26px, 3vw, 42px); font-weight: 800;
  color: var(--white); margin-bottom: 16px; letter-spacing: -1px;
  line-height: 1.15;
}
.cta-banner p {
  font-size: 17px; color: var(--text-2); line-height: 1.75; margin-bottom: 36px;
}
.cta-banner-btns { display: flex; gap: 14px; justify-content: center; flex-wrap: wrap; }

/* ============================================================
   APPROACH
   ============================================================ */
.approach-section { background: linear-gradient(180deg, var(--navy) 0%, var(--navy-2) 100%); }
.steps-row {
  display: grid; grid-template-columns: repeat(4, 1fr);
  gap: 0; position: relative;
}
.steps-row::before {
  content: ''; position: absolute; top: 34px; left: 12.5%; right: 12.5%;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--border), var(--border), transparent);
}
.step { text-align: center; padding: 0 20px; }
.step-num {
  width: 68px; height: 68px; border-radius: 50%;
  background: var(--navy-3); border: 1px solid var(--border);
  display: flex; align-items: center; justify-content: center; margin: 0 auto 22px;
  font-family: 'Space Grotesk', sans-serif; font-size: 19px; font-weight: 700;
  color: var(--blue-2); position: relative; z-index: 1;
  transition: all 0.3s;
}
.step:hover .step-num {
  background: rgba(241,198,211,0.1);
  border-color: var(--blue-2);
  box-shadow: 0 0 24px rgba(241,198,211,0.18);
}
.step h4 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 15px; font-weight: 700; color: var(--white); margin-bottom: 10px;
}
.step p { font-size: 13px; color: var(--text); line-height: 1.7; }

/* ============================================================
   WHY APEX
   ============================================================ */
.why-section { background: var(--navy-2); }
.why-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 80px; align-items: center; }
.why-content h2 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(26px, 2.8vw, 42px); font-weight: 700; letter-spacing: -0.8px;
  color: var(--white); margin-bottom: 16px; line-height: 1.18;
}
.why-content > p { font-size: 16px; color: var(--text-2); line-height: 1.78; margin-bottom: 36px; }
.diffs { display: flex; flex-direction: column; gap: 16px; }
.diff {
  display: flex; gap: 16px; align-items: flex-start;
  padding: 18px 20px; border-radius: 14px;
  border: 1px solid var(--border-2); background: rgba(6,13,26,0.3);
  transition: all 0.25s;
}
.diff:hover { border-color: var(--border); background: rgba(241,198,211,0.03); }
.diff-ico {
  width: 42px; height: 42px; border-radius: 11px;
  background: rgba(241,198,211,0.1); border: 1px solid rgba(241,198,211,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 19px; flex-shrink: 0; margin-top: 1px;
}
.diff h4 { font-size: 14px; font-weight: 600; color: var(--white); margin-bottom: 5px; }
.diff p { font-size: 13px; color: var(--text); line-height: 1.65; }
.why-cards { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; }
.why-card {
  background: var(--navy-3); border: 1px solid var(--border-2);
  border-radius: 18px; padding: 28px; text-align: center; transition: all 0.3s;
}
.why-card:hover { border-color: var(--border); transform: translateY(-3px); box-shadow: var(--shadow-sm); }
.why-card:first-child { grid-column: 1 / -1; }
.wc-val {
  font-family: 'Space Grotesk', sans-serif; font-size: 21px; font-weight: 700;
  background: linear-gradient(135deg, var(--blue), var(--blue-2));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
  margin-bottom: 8px;
}
.wc-lbl { font-size: 13px; color: var(--text); line-height: 1.55; }

/* ============================================================
   INDUSTRIES
   ============================================================ */
.industries-section { background: var(--navy); }
.ind-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
.ind-card {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 16px;
  padding: 22px 18px; display: flex; align-items: center; gap: 14px;
  transition: all 0.3s; text-decoration: none;
}
.ind-card:hover { border-color: var(--border); transform: translateY(-3px); box-shadow: var(--shadow-sm); }
.ind-ico { font-size: 28px; flex-shrink: 0; }
.ind-card h4 { font-size: 14px; font-weight: 600; color: var(--white); margin-bottom: 4px; }
.ind-card p { font-size: 12px; color: var(--text); line-height: 1.5; }

/* ============================================================
   TESTIMONIALS
   ============================================================ */
.testimonials-section { background: var(--navy-2); }
.testimonials-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 22px; }
.testimonial-card {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 20px;
  padding: 32px 26px; position: relative; transition: all 0.35s;
  display: flex; flex-direction: column;
}
.testimonial-card:hover { border-color: var(--border); transform: translateY(-5px); box-shadow: 0 20px 48px rgba(241,198,211,0.09); }
.testimonial-card::before {
  content: ''; position: absolute; top: 0; left: 20%; right: 20%; height: 1px;
  background: linear-gradient(90deg, transparent, var(--border), transparent);
}
.stars {
  display: flex; gap: 2px; margin-bottom: 18px;
}
.stars span { color: var(--gold); font-size: 14px; }
.quote-icon {
  font-size: 44px; line-height: 1; color: var(--blue); opacity: 0.35;
  font-family: Georgia, serif; margin-bottom: 10px; display: block; margin-top: -10px;
}
.testimonial-text {
  font-size: 14px; color: var(--text-2); line-height: 1.8;
  margin-bottom: 24px; font-style: italic; flex: 1;
}
.testimonial-author { display: flex; align-items: center; gap: 14px; }
.author-avatar {
  width: 44px; height: 44px; border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  font-weight: 800; font-size: 16px; color: var(--navy); flex-shrink: 0;
}
.author-name { font-size: 14px; font-weight: 600; color: var(--white); margin-bottom: 3px; }
.author-title { font-size: 12px; color: var(--text); }

/* ============================================================
   TECH STACK
   ============================================================ */
.tech-section {
  padding: 60px 32px;
  border-top: 1px solid var(--border-2); border-bottom: 1px solid var(--border-2);
  background: rgba(17,34,64,0.35);
}
.tech-inner { max-width: 1100px; margin: 0 auto; text-align: center; }
.tech-inner .sec-label { margin-bottom: 26px; display: block; }
.tech-badges { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; }
.tbadge {
  background: var(--navy-3); border: 1px solid var(--border-2); border-radius: 8px;
  padding: 8px 20px; font-size: 13px; font-weight: 500;
  color: var(--text-2); transition: all 0.25s; cursor: default;
}
.tbadge:hover { border-color: var(--border); color: var(--white); background: rgba(241,198,211,0.06); }

/* ============================================================
   FAQ
   ============================================================ */
.faq-section { background: var(--navy); }
.faq-list { max-width: 800px; margin: 0 auto; }
.faq-item {
  border: 1px solid var(--border-2); border-radius: 14px; margin-bottom: 12px;
  overflow: hidden; transition: border-color 0.25s;
  background: rgba(17,34,64,0.4);
}
.faq-item.open { border-color: var(--border); background: rgba(241,198,211,0.025); }
.faq-question {
  width: 100%; display: flex; justify-content: space-between; align-items: center;
  padding: 20px 24px; background: none; border: none; cursor: pointer;
  font-family: 'Inter', sans-serif; font-size: 15px; font-weight: 500;
  color: var(--white); text-align: left; gap: 16px;
}
.faq-question:hover { color: var(--blue-3); }
.faq-icon {
  width: 26px; height: 26px; border-radius: 50%; border: 1px solid var(--border);
  display: flex; align-items: center; justify-content: center;
  font-size: 18px; color: var(--blue-2); flex-shrink: 0;
  transition: transform 0.35s, border-color 0.25s;
}
.faq-item.open .faq-icon { transform: rotate(45deg); border-color: var(--blue); }
.faq-answer {
  max-height: 0; overflow: hidden;
  transition: max-height 0.4s cubic-bezier(.4,0,.2,1);
  padding: 0 24px;
}
.faq-item.open .faq-answer { max-height: 300px; padding: 0 24px 22px; }
.faq-answer p { font-size: 14px; color: var(--text-2); line-height: 1.78; }

/* ============================================================
   CONTACT
   ============================================================ */
.contact-section {
  background: var(--navy); position: relative; overflow: hidden;
}
.contact-section::before {
  content: ''; position: absolute; top: 50%; left: 50%;
  transform: translate(-50%, -50%);
  width: 1000px; height: 450px;
  background: radial-gradient(ellipse, rgba(241,198,211,0.055) 0%, transparent 70%);
  pointer-events: none;
}
.contact-inner {
  max-width: 1100px; margin: 0 auto;
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 72px; align-items: start; position: relative; z-index: 1;
}
.contact-info h2 {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(26px, 2.8vw, 42px); font-weight: 700; letter-spacing: -0.8px;
  color: var(--white); margin-bottom: 16px; line-height: 1.18;
}
.contact-info > p { font-size: 16px; color: var(--text-2); line-height: 1.78; margin-bottom: 36px; }
.c-methods { display: flex; flex-direction: column; gap: 14px; margin-bottom: 32px; }
.c-method {
  display: flex; align-items: center; gap: 14px;
  text-decoration: none; color: var(--text-2); transition: all 0.2s;
  padding: 14px 18px; border-radius: 14px; border: 1px solid var(--border-2);
  background: rgba(6,13,26,0.3);
}
.c-method:hover { color: var(--white); border-color: var(--border); background: rgba(241,198,211,0.05); }
.c-ico {
  width: 44px; height: 44px; border-radius: 11px;
  background: rgba(241,198,211,0.1); border: 1px solid rgba(241,198,211,0.2);
  display: flex; align-items: center; justify-content: center;
  font-size: 19px; flex-shrink: 0;
}
.c-lbl { font-size: 10px; text-transform: uppercase; letter-spacing: 1.2px; color: var(--text); margin-bottom: 3px; }
.c-val { font-size: 15px; font-weight: 500; }
.c-guarantee {
  display: flex; align-items: flex-start; gap: 12px; padding: 16px 18px;
  background: rgba(16,185,129,0.07); border: 1px solid rgba(16,185,129,0.2);
  border-radius: 12px;
}
.c-guarantee-ico { font-size: 18px; flex-shrink: 0; margin-top: 1px; }
.c-guarantee p { font-size: 13px; color: var(--text-2); line-height: 1.65; }
.c-guarantee strong { color: var(--white); }

/* Contact form */
.c-form-box {
  background: var(--navy-3); border: 1px solid var(--border-2);
  border-radius: 22px; padding: 36px 32px;
  box-shadow: var(--shadow-md);
}
.c-form-box::before {
  content: ''; display: block; margin: -36px -32px 30px;
  height: 2px; border-radius: 22px 22px 0 0;
  background: linear-gradient(90deg, transparent, var(--blue), var(--rose), transparent);
}
.cf-head {
  font-family: 'Space Grotesk', sans-serif;
  font-size: 20px; font-weight: 700; color: var(--white); margin-bottom: 6px;
}
.cf-sub { font-size: 13px; color: var(--text); margin-bottom: 28px; }
.fg { margin-bottom: 14px; }
.fg label {
  display: block; font-size: 11px; font-weight: 700; letter-spacing: 0.6px;
  text-transform: uppercase; color: var(--text-2); margin-bottom: 7px;
}
.fg input, .fg select, .fg textarea {
  width: 100%; background: rgba(6,13,26,0.75); border: 1px solid rgba(255,255,255,0.09);
  border-radius: 10px; padding: 12px 16px; font-size: 14px; color: var(--white);
  font-family: 'Inter', sans-serif; outline: none; resize: none;
  transition: border-color 0.2s, box-shadow 0.2s;
}
.fg input:focus, .fg select:focus, .fg textarea:focus {
  border-color: rgba(241,198,211,0.45);
  box-shadow: 0 0 0 3px rgba(241,198,211,0.08);
}
.fg input::placeholder, .fg textarea::placeholder { color: rgba(148,163,184,0.5); }
.fg select option { background: var(--navy-2); color: var(--white); }
.fg-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
.cf-submit {
  width: 100%; background: linear-gradient(135deg, var(--blue), var(--rose));
  color: #060D1A; border: none; border-radius: 10px; padding: 14px;
  font-size: 15px; font-weight: 700; cursor: pointer;
  font-family: 'Inter', sans-serif; transition: all 0.3s;
  box-shadow: var(--shadow-glow); margin-top: 6px; letter-spacing: 0.2px;
}
.cf-submit:hover { transform: translateY(-2px); box-shadow: 0 10px 38px rgba(241,198,211,0.44); }
.cf-submit:active { transform: none; }
.form-success {
  display: none; text-align: center; padding: 28px 20px;
}
.form-success-icon { font-size: 44px; margin-bottom: 14px; }
.form-success h3 {
  font-family: 'Space Grotesk', sans-serif; font-size: 20px; font-weight: 700;
  color: var(--white); margin-bottom: 10px;
}
.form-success p { font-size: 14px; color: var(--text-2); }

/* ============================================================
   FOOTER
   ============================================================ */
.footer {
  background: var(--navy);
  border-top: 1px solid var(--border-2);
  padding: 60px 32px 32px;
}
.footer-top {
  max-width: 1200px; margin: 0 auto;
  display: grid; grid-template-columns: 2fr 1fr 1fr 1fr;
  gap: 48px; margin-bottom: 48px;
}
.f-brand { }
.f-brand-row { display: flex; align-items: center; gap: 10px; margin-bottom: 14px; }
.f-brand-row img { height: 30px; }
.f-brand-name {
  font-family: 'Space Grotesk', sans-serif; font-weight: 700; font-size: 16px; color: var(--white);
}
.f-brand-desc { font-size: 13px; color: var(--text); line-height: 1.7; max-width: 280px; margin-bottom: 20px; }
.f-social { display: flex; gap: 10px; }
.f-social-link {
  width: 36px; height: 36px; border-radius: 9px;
  border: 1px solid var(--border-2); background: rgba(255,255,255,0.04);
  display: flex; align-items: center; justify-content: center;
  font-size: 15px; text-decoration: none; transition: all 0.2s; color: var(--text);
}
.f-social-link:hover { border-color: var(--border); color: var(--white); background: rgba(241,198,211,0.08); }
.f-col h5 {
  font-size: 12px; font-weight: 700; letter-spacing: 1.5px;
  text-transform: uppercase; color: var(--text); margin-bottom: 18px;
}
.f-col ul { list-style: none; display: flex; flex-direction: column; gap: 12px; }
.f-col ul a { font-size: 13px; color: var(--text-2); text-decoration: none; transition: color 0.2s; }
.f-col ul a:hover { color: var(--white); }
.footer-bottom {
  max-width: 1200px; margin: 0 auto;
  display: flex; align-items: center; justify-content: space-between;
  flex-wrap: wrap; gap: 16px;
  padding-top: 28px; border-top: 1px solid var(--border-2);
}
.f-copy { font-size: 12px; color: var(--text); }
.f-bottom-links { display: flex; gap: 24px; }
.f-bottom-links a { font-size: 12px; color: var(--text); text-decoration: none; transition: color 0.2s; }
.f-bottom-links a:hover { color: var(--white); }

/* ============================================================
   RESPONSIVE
   ============================================================ */
@media (max-width: 1024px) {
  .footer-top { grid-template-columns: 1fr 1fr; }
}
@media (max-width: 960px) {
  .hero-inner { grid-template-columns: 1fr; gap: 48px; }
  .hero-visual { display: none; }
  .services-grid { grid-template-columns: 1fr 1fr; }
  .steps-row { grid-template-columns: 1fr 1fr; }
  .steps-row::before { display: none; }
  .why-grid { grid-template-columns: 1fr; gap: 48px; }
  .testimonials-grid { grid-template-columns: 1fr 1fr; }
  .contact-inner { grid-template-columns: 1fr; gap: 48px; }
  .ind-grid { grid-template-columns: 1fr 1fr; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
}
@media (max-width: 768px) {
  .nav-links { display: none; }
  .hamburger-btn { display: flex; }
  .services-grid { grid-template-columns: 1fr; }
  .services-primary-grid { grid-template-columns: 1fr; }
  .testimonials-grid { grid-template-columns: 1fr; }
  .footer-top { grid-template-columns: 1fr; gap: 32px; }
}
@media (max-width: 640px) {
  section { padding: 72px 20px; }
  .stats-grid { grid-template-columns: 1fr 1fr; }
  .steps-row { grid-template-columns: 1fr; }
  .why-cards { grid-template-columns: 1fr; }
  .why-card:first-child { grid-column: 1; }
  .ind-grid { grid-template-columns: 1fr; }
  .fg-row { grid-template-columns: 1fr; }
  .footer-inner { flex-direction: column; text-align: center; }
  .trust-bar-inner { gap: 20px; }
  .cta-banner-btns { flex-direction: column; align-items: center; }
  .footer-bottom { flex-direction: column; text-align: center; }
}
</style>

<div class="apex-site" role="main">

<!-- ======================== SCROLL PROGRESS ======================== -->
<div class="scroll-progress" id="scrollProgress" aria-hidden="true"></div>

<!-- ======================== MOBILE MENU ======================== -->
<div class="mobile-menu" id="mobileMenu" role="dialog" aria-label="Navigation menu">
  <a href="#services" class="mobile-link">Services</a>
  <a href="#approach" class="mobile-link">Approach</a>
  <a href="#why-apex" class="mobile-link">Why Apex</a>
  <a href="#industries" class="mobile-link">Industries</a>
  <a href="#contact" class="m-cta mobile-link">Get in Touch</a>
</div>

<!-- ======================== NAVBAR ======================== -->
<nav class="nav" id="mainNav" aria-label="Main navigation">
  <div class="nav-inner">
    <a href="#" class="nav-logo" aria-label="Apex Data &amp; Marketing Cloud home">
      <img src="apex_logo.PNG" alt="Apex Data &amp; Marketing Cloud logo" width="34" height="34">
      <span class="nav-logo-text">Apex <span>Data &amp; Marketing</span> Cloud</span>
    </a>
    <ul class="nav-links" role="list">
      <li><a href="#services">Services</a></li>
      <li><a href="#approach">Approach</a></li>
      <li><a href="#why-apex">Why Apex</a></li>
      <li><a href="#industries">Industries</a></li>
      <li><a href="#contact" class="nav-cta">Get in Touch</a></li>
    </ul>
    <button class="hamburger-btn" id="hamburgerBtn" aria-label="Toggle mobile menu" aria-expanded="false">
      <span></span><span></span><span></span>
    </button>
  </div>
</nav>

<!-- ======================== HERO ======================== -->
<section class="hero" aria-labelledby="hero-heading">
  <div class="hero-grid-bg" aria-hidden="true"></div>
  <div class="hero-glow-1" aria-hidden="true"></div>
  <div class="hero-glow-2" aria-hidden="true"></div>
  <div class="hero-glow-3" aria-hidden="true"></div>
  <div class="hero-inner">
    <div>
      <div class="hero-badge" aria-label="AI-Powered Marketing Intelligence Consulting firm">
        <span class="live-dot" aria-hidden="true"></span>
        AI-Powered Marketing Intelligence
      </div>
      <h1 id="hero-heading">Turn Customer Intelligence Into<br><span class="hl">Unstoppable Growth</span></h1>
      <p>We partner with CMOs, founders, and growth leaders to transform raw customer data into revenue-driving marketing strategy — combining AI, predictive segmentation, attribution science, and machine learning to deliver measurable, compounding results.</p>
      <div class="hero-cta">
        <a href="#contact" class="btn-primary" onclick="gtag('event','click',{event_category:'CTA',event_label:'Hero Primary'})">
          Start a Conversation &#8594;
        </a>
        <a href="#services" class="btn-ghost">
          Explore Our Services
        </a>
      </div>
    </div>
    <div class="hero-visual" aria-hidden="true">
      <div class="hero-panel">
        <div class="panel-label">Core Capabilities</div>
        <div class="panel-metrics">
          <div class="pm-card">
            <div class="pm-val">Segmentation</div>
            <div class="pm-lbl">Audience Intelligence</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">Attribution</div>
            <div class="pm-lbl">Multi-Touch ROI</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">Predictive</div>
            <div class="pm-lbl">LTV &amp; Churn Models</div>
          </div>
          <div class="pm-card">
            <div class="pm-val">GenAI</div>
            <div class="pm-lbl">Personalization at Scale</div>
          </div>
        </div>
        <div class="panel-pills">
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(241,198,211,0.12);">&#128202;</div>
            Customer Segmentation &amp; Audience Intelligence
            <span class="ppill-arrow">&#8594;</span>
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(245,158,11,0.12);">&#127919;</div>
            Marketing Analytics &amp; Attribution
            <span class="ppill-arrow">&#8594;</span>
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(16,185,129,0.12);">&#129302;</div>
            AI-Powered Personalization
            <span class="ppill-arrow">&#8594;</span>
          </div>
          <div class="ppill">
            <div class="ppill-icon" style="background:rgba(139,92,246,0.12);">&#128200;</div>
            Demand Generation &amp; Growth Analytics
            <span class="ppill-arrow">&#8594;</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== TRUST BAR ======================== -->
<div class="trust-bar" role="complementary" aria-label="Trust signals">
  <div class="trust-bar-inner">
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Advisor-First Philosophy
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Full-Funnel Attribution
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      AI-Native Intelligence
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      Measurable Revenue Impact
    </div>
    <div class="t-item">
      <svg width="16" height="16" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
      15+ Industries Served
    </div>
  </div>
</div>

<!-- ======================== IMPACT STATS ======================== -->
<div class="stats-section" aria-label="Impact statistics">
  <div class="stats-grid">
    <div class="stat-item reveal">
      <span class="stat-num" data-target="4.2" data-suffix="×" data-decimal="1">0×</span>
      <div class="stat-label">Average Campaign ROI</div>
      <div class="stat-sublabel">Delivered within 12 months</div>
    </div>
    <div class="stat-item reveal reveal-delay-1">
      <span class="stat-num" data-target="50" data-suffix="+">0+</span>
      <div class="stat-label">Enterprise Engagements</div>
      <div class="stat-sublabel">Completed end-to-end</div>
    </div>
    <div class="stat-item reveal reveal-delay-2">
      <span class="stat-num" data-target="68" data-suffix="%">0%</span>
      <div class="stat-label">Average CAC Reduction</div>
      <div class="stat-sublabel">Across client portfolio</div>
    </div>
    <div class="stat-item reveal reveal-delay-3">
      <span class="stat-num" data-target="98" data-suffix="%">0%</span>
      <div class="stat-label">Client Satisfaction</div>
      <div class="stat-sublabel">Return engagement rate</div>
    </div>
  </div>
</div>

<!-- ======================== SERVICES ======================== -->
<section id="services" class="services-section" aria-labelledby="services-heading">
  <div class="container">
    <div class="sec-header reveal">
      <div class="sec-label">What We Do</div>
      <h2 class="sec-title" id="services-heading">Intelligence-Driven Marketing, End to End</h2>
      <p class="sec-sub">We operate at the intersection of marketing strategy, data science, and AI — connecting every customer insight directly to pipeline, revenue, and sustainable competitive advantage.</p>
    </div>
    <div class="services-primary-grid">

      <div class="svc-card reveal">
        <div class="svc-icon" aria-hidden="true">&#128101;</div>
        <h3>Customer Segmentation &amp; Audience Intelligence</h3>
        <p>We build precision audience models that go far beyond demographics — RFM analysis, behavioral cohorts, psychographic profiling, and lookalike modeling — so every campaign reaches exactly the right customer at exactly the right moment.</p>
        <div class="svc-tags">
          <span class="tag">RFM Modeling</span>
          <span class="tag">Behavioral Cohorts</span>
          <span class="tag">Persona Mapping</span>
          <span class="tag">Lookalike Audiences</span>
          <span class="tag">Churn Segmentation</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-1">
        <div class="svc-icon" aria-hidden="true">&#127919;</div>
        <h3>Marketing Analytics &amp; Attribution</h3>
        <p>We replace vanity metrics with revenue truth — designing full-funnel attribution frameworks, campaign ROI dashboards, and multi-touch models that tell you precisely which channels, messages, and moments drive conversion and growth.</p>
        <div class="svc-tags">
          <span class="tag">Multi-Touch Attribution</span>
          <span class="tag">Funnel Analytics</span>
          <span class="tag">Campaign ROI</span>
          <span class="tag">Marketing Dashboards</span>
          <span class="tag">A/B Testing</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-2">
        <div class="svc-new-badge">New</div>
        <div class="svc-icon" aria-hidden="true">&#129302;</div>
        <h3>AI-Powered Personalization</h3>
        <p>We engineer real-time personalization systems powered by machine learning — dynamic content engines, next-best-action models, and recommendation algorithms — delivering hyper-relevant experiences that convert and retain at scale.</p>
        <div class="svc-tags">
          <span class="tag">Recommendation Engines</span>
          <span class="tag">Next-Best-Action</span>
          <span class="tag">Dynamic Content</span>
          <span class="tag">Real-Time Decisioning</span>
          <span class="tag">LLM-Driven Copy</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-3">
        <div class="svc-icon" aria-hidden="true">&#128200;</div>
        <h3>Demand Generation &amp; Growth Analytics</h3>
        <p>We model the full revenue engine — lead scoring, pipeline forecasting, CAC/LTV optimization, and churn prediction — giving your growth team the intelligence to acquire better customers, faster, at lower cost.</p>
        <div class="svc-tags">
          <span class="tag">Lead Scoring</span>
          <span class="tag">Pipeline Forecasting</span>
          <span class="tag">CAC / LTV Modeling</span>
          <span class="tag">Churn Prediction</span>
          <span class="tag">Revenue Attribution</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

    </div>

    <div class="capabilities-subheader reveal">
      <div class="sec-label">The Intelligence Engine Behind Every Campaign</div>
      <p class="sec-sub">Our marketing work is powered by enterprise-grade data and AI infrastructure — capabilities most agencies simply don't have.</p>
    </div>
    <div class="services-grid">

      <div class="svc-card reveal">
        <div class="svc-icon" aria-hidden="true">&#129302;</div>
        <h3>AI &amp; Machine Learning Advisory</h3>
        <p>From use-case discovery to production deployment, we apply AI pragmatically — where it creates genuine, sustained marketing value rather than experimental novelty.</p>
        <div class="svc-tags">
          <span class="tag">Model Development</span>
          <span class="tag">MLOps</span>
          <span class="tag">AI Governance</span>
          <span class="tag">Responsible AI</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-1">
        <div class="svc-new-badge">New</div>
        <div class="svc-icon" aria-hidden="true">&#10024;</div>
        <h3>Generative AI &amp; LLM Strategy</h3>
        <p>We help marketing organizations deploy GenAI capabilities responsibly — RAG-powered content systems, AI copywriting agents, and fine-tuned LLMs that scale creative output without sacrificing brand integrity.</p>
        <div class="svc-tags">
          <span class="tag">RAG Systems</span>
          <span class="tag">AI Content Agents</span>
          <span class="tag">LLM Fine-Tuning</span>
          <span class="tag">Prompt Engineering</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-2">
        <div class="svc-icon" aria-hidden="true">&#128300;</div>
        <h3>Business, Data &amp; Digital Strategy</h3>
        <p>We assess your current marketing data landscape, define a clear strategic roadmap, and guide execution — transforming fragmented data assets into a unified, revenue-generating intelligence layer.</p>
        <div class="svc-tags">
          <span class="tag">Data Roadmap</span>
          <span class="tag">MarTech Strategy</span>
          <span class="tag">Digital Transformation</span>
          <span class="tag">OKR Alignment</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal">
        <div class="svc-icon" aria-hidden="true">&#9729;&#65039;</div>
        <h3>Cloud &amp; Data Platform Architecture</h3>
        <p>We design the scalable, secure data infrastructure your marketing stack requires — from customer data platforms to real-time event pipelines — built for sustained growth.</p>
        <div class="svc-tags">
          <span class="tag">CDP Architecture</span>
          <span class="tag">Real-Time Pipelines</span>
          <span class="tag">Data Lakehouse</span>
          <span class="tag">DataOps</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

      <div class="svc-card reveal reveal-delay-1">
        <div class="svc-icon" aria-hidden="true">&#128737;&#65039;</div>
        <h3>Data Governance &amp; Compliance</h3>
        <p>We ensure your customer data assets meet the highest standards of quality, lineage, and regulatory compliance — turning governance into a marketing competitive advantage.</p>
        <div class="svc-tags">
          <span class="tag">Data Quality</span>
          <span class="tag">GDPR / CCPA</span>
          <span class="tag">Consent Management</span>
          <span class="tag">Master Data Mgmt</span>
        </div>
        <a href="#contact" class="svc-link">Explore this service &#8594;</a>
      </div>

    </div>
  </div>
</section>

<!-- ======================== MID-PAGE CTA ======================== -->
<div class="cta-banner" role="complementary">
  <div class="cta-banner-inner reveal">
    <div class="sec-label">Ready to Move Forward?</div>
    <h2>Not Sure Where to Start?<br>We'll Help You Find the Right Path.</h2>
    <p>Whether you're a Fortune 500 enterprise or a growth-stage startup—our advisory process is designed to meet you exactly where you are and define a clear, high-impact roadmap.</p>
    <div class="cta-banner-btns">
      <a href="#contact" class="btn-primary" onclick="gtag('event','click',{event_category:'CTA',event_label:'Mid-Page Primary'})">
        Book a Discovery Call &#8594;
      </a>
      <a href="#approach" class="btn-ghost">See How We Work</a>
    </div>
  </div>
</div>

<!-- ======================== APPROACH ======================== -->
<section id="approach" class="approach-section" aria-labelledby="approach-heading">
  <div class="container">
    <div class="sec-header reveal">
      <div class="sec-label">How We Work</div>
      <h2 class="sec-title" id="approach-heading">A Disciplined, Four-Phase Engagement Model</h2>
      <p class="sec-sub">Sustainable marketing performance doesn't come from tactics — it comes from a rigorous, repeatable methodology that connects every initiative to measurable business outcomes.</p>
    </div>
    <div class="steps-row">
      <div class="step reveal">
        <div class="step-num" aria-hidden="true">01</div>
        <h4>Audit &amp; Diagnose</h4>
        <p>We assess your current data assets, MarTech stack, audience quality, and attribution gaps — establishing a precise baseline before recommending a single initiative.</p>
      </div>
      <div class="step reveal reveal-delay-1">
        <div class="step-num" aria-hidden="true">02</div>
        <h4>Strategy &amp; Blueprint</h4>
        <p>We design a prioritized marketing intelligence roadmap — identifying highest-impact opportunities and the exact models, platforms, and campaigns that will move your most critical KPIs.</p>
      </div>
      <div class="step reveal reveal-delay-2">
        <div class="step-num" aria-hidden="true">03</div>
        <h4>Build &amp; Activate</h4>
        <p>We build, deploy, and activate — segmentation models, attribution frameworks, personalization engines, and demand generation systems — integrated seamlessly into your existing stack.</p>
      </div>
      <div class="step reveal reveal-delay-3">
        <div class="step-num" aria-hidden="true">04</div>
        <h4>Measure &amp; Scale</h4>
        <p>We close the loop with rigorous performance tracking against agreed business KPIs, continuously optimizing to compound returns and extend your competitive advantage over time.</p>
      </div>
    </div>
  </div>
</section>

<!-- ======================== WHY APEX ======================== -->
<section id="why-apex" class="why-section" aria-labelledby="why-heading">
  <div class="container">
    <div class="why-grid">
      <div class="why-content reveal">
        <div class="sec-label">Why Choose Apex</div>
        <h2 id="why-heading">Data Scientists Who Think Like Marketers.<br>Marketers Who Are Fluent in Data.</h2>
        <p>Most marketing agencies can't build a predictive churn model. Most data consultancies can't write a go-to-market strategy. We sit at that rare intersection — bringing both the strategic depth of a senior marketing partner and the technical precision of an AI and data science firm to every engagement.</p>
        <div class="diffs">
          <div class="diff">
            <div class="diff-ico" aria-hidden="true">&#127919;</div>
            <div>
              <h4>Revenue-Tied Outcomes</h4>
              <p>Every recommendation maps to pipeline, CAC, LTV, or conversion rate. We don't deliver reports — we deliver measurable revenue impact with clear attribution.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico" aria-hidden="true">&#128275;</div>
            <div>
              <h4>Audience Clarity</h4>
              <p>We eliminate the guesswork from audience strategy. Our segmentation models give your team the precision to personalize at scale and acquire customers that actually stay.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico" aria-hidden="true">&#9881;&#65039;</div>
            <div>
              <h4>Pragmatic AI Deployment</h4>
              <p>We apply AI where it genuinely moves the needle — with robust governance and a clear path to production, not proof-of-concept theater.</p>
            </div>
          </div>
          <div class="diff">
            <div class="diff-ico" aria-hidden="true">&#128736;&#65039;</div>
            <div>
              <h4>End-to-End Partnership</h4>
              <p>From strategy through activation and optimization — one trusted partner across your entire marketing intelligence journey, with no handoffs and full accountability.</p>
            </div>
          </div>
        </div>
      </div>
      <div class="why-cards reveal reveal-delay-2">
        <div class="why-card">
          <div class="wc-val">Marketing Strategy + Data Science</div>
          <div class="wc-lbl">We bridge the gap between CMO priorities and data engineering reality, ensuring your marketing vision becomes measurable operational performance.</div>
        </div>
        <div class="why-card">
          <div class="wc-val">AI-Native</div>
          <div class="wc-lbl">Modern ML, predictive modeling, and GenAI tooling embedded in every engagement from day one — not bolted on afterward.</div>
        </div>
        <div class="why-card">
          <div class="wc-val">ROI-Focused</div>
          <div class="wc-lbl">Every initiative measured against clear revenue KPIs from kickoff to close. No vanity metrics, no ambiguity.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== INDUSTRIES ======================== -->
<section id="industries" class="industries-section" aria-labelledby="industries-heading">
  <div class="container">
    <div class="sec-header reveal">
      <div class="sec-label">Industries We Serve</div>
      <h2 class="sec-title" id="industries-heading">Deep Domain Expertise Across Every Growth Vertical</h2>
      <p class="sec-sub">We bring industry-specific marketing intelligence to every engagement — ensuring solutions address the real acquisition, retention, and monetization challenges unique to your sector.</p>
    </div>
    <div class="ind-grid">
      <div class="ind-card reveal">
        <div class="ind-ico" aria-hidden="true">&#127970;</div>
        <div>
          <h4>Financial Services</h4>
          <p>Customer acquisition models, retention analytics, cross-sell intelligence, regulatory-compliant personalization</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-1">
        <div class="ind-ico" aria-hidden="true">&#128138;</div>
        <div>
          <h4>Healthcare &amp; Life Sciences</h4>
          <p>Patient journey analytics, HCP engagement modeling, compliant segmentation, outcomes-based attribution</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-2">
        <div class="ind-ico" aria-hidden="true">&#128722;</div>
        <div>
          <h4>Retail &amp; E-Commerce</h4>
          <p>Customer lifetime value optimization, purchase propensity, abandoned cart intelligence, loyalty segmentation</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-1">
        <div class="ind-ico" aria-hidden="true">&#128679;</div>
        <div>
          <h4>Manufacturing &amp; Operations</h4>
          <p>Dealer/distributor analytics, B2B demand generation, account scoring, market penetration modeling</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-2">
        <div class="ind-ico" aria-hidden="true">&#128640;</div>
        <div>
          <h4>Technology &amp; SaaS</h4>
          <p>Product-led growth analytics, churn modeling, expansion revenue intelligence, trial-to-paid conversion</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-3">
        <div class="ind-ico" aria-hidden="true">&#127968;</div>
        <div>
          <h4>Real Estate &amp; PropTech</h4>
          <p>Buyer intent modeling, market intelligence, lead scoring, digital campaign attribution</p>
        </div>
      </div>
      <div class="ind-card reveal">
        <div class="ind-ico" aria-hidden="true">&#9889;</div>
        <div>
          <h4>Energy &amp; Utilities</h4>
          <p>Customer engagement analytics, retention modeling, sustainability campaign performance, ESG communications</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-1">
        <div class="ind-ico" aria-hidden="true">&#127979;</div>
        <div>
          <h4>Education &amp; EdTech</h4>
          <p>Enrollment funnel analytics, student acquisition intelligence, engagement scoring, retention campaigns</p>
        </div>
      </div>
      <div class="ind-card reveal reveal-delay-2">
        <div class="ind-ico" aria-hidden="true">&#128241;</div>
        <div>
          <h4>Media &amp; Entertainment</h4>
          <p>Audience monetization, subscriber retention, content personalization, ad revenue optimization</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ======================== TESTIMONIALS ======================== -->
<section class="testimonials-section" aria-labelledby="testimonials-heading">
  <div class="container">
    <div class="sec-header reveal">
      <div class="sec-label">Client Voices</div>
      <h2 class="sec-title" id="testimonials-heading">Results Our Partners Speak To</h2>
      <p class="sec-sub">We measure success not by deliverables — but by the revenue, growth, and competitive advantage we create alongside our clients.</p>
    </div>
    <div class="testimonials-grid">

      <div class="testimonial-card reveal">
        <div class="stars" aria-label="5 out of 5 stars">
          <span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span>
        </div>
        <span class="quote-icon" aria-hidden="true">&ldquo;</span>
        <p class="testimonial-text">Apex rebuilt how our marketing team thinks about customers entirely. Their segmentation models identified three audience cohorts we had never monetized — within six months, those segments alone drove a 40% lift in campaign conversion and our first AI-powered personalization engine in production.</p>
        <div class="testimonial-author">
          <div class="author-avatar" style="background:linear-gradient(135deg,#F1C6D3,#C96B87);" aria-hidden="true">SC</div>
          <div>
            <div class="author-name">Sarah Chen</div>
            <div class="author-title">Chief Data Officer, FinServ Enterprise</div>
          </div>
        </div>
      </div>

      <div class="testimonial-card reveal reveal-delay-1">
        <div class="stars" aria-label="5 out of 5 stars">
          <span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span>
        </div>
        <span class="quote-icon" aria-hidden="true">&ldquo;</span>
        <p class="testimonial-text">What sets Apex apart is that they speak both languages — they can align with your CMO on growth strategy, then turn around and architect the data models to make it real. We went from zero marketing intelligence capability to production-grade lead scoring in 14 weeks. Pipeline quality transformed overnight.</p>
        <div class="testimonial-author">
          <div class="author-avatar" style="background:linear-gradient(135deg,#F59E0B,#D97706);" aria-hidden="true">MR</div>
          <div>
            <div class="author-name">Marcus Rivera</div>
            <div class="author-title">VP Growth, HealthTech Scale-Up</div>
          </div>
        </div>
      </div>

      <div class="testimonial-card reveal reveal-delay-2">
        <div class="stars" aria-label="5 out of 5 stars">
          <span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span><span>&#9733;</span>
        </div>
        <span class="quote-icon" aria-hidden="true">&ldquo;</span>
        <p class="testimonial-text">We engaged Apex to overhaul our customer segmentation and attribution. They delivered a comprehensive roadmap, built our first RFM model, and stayed with us through full deployment. Three months later, CAC was down 31% and our best-fit customer cohort had doubled in size.</p>
        <div class="testimonial-author">
          <div class="author-avatar" style="background:linear-gradient(135deg,#10B981,#059669);" aria-hidden="true">AB</div>
          <div>
            <div class="author-name">Alexandra Brooks</div>
            <div class="author-title">CEO, Retail Analytics Company</div>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ======================== TECH STACK ======================== -->
<div class="tech-section" role="complementary" aria-label="Technology ecosystem">
  <div class="tech-inner">
    <span class="sec-label">Technology Ecosystem</span>
    <div class="tech-badges" role="list">
      <span class="tbadge" role="listitem">Python</span>
      <span class="tbadge" role="listitem">R</span>
      <span class="tbadge" role="listitem">Apache Spark</span>
      <span class="tbadge" role="listitem">dbt</span>
      <span class="tbadge" role="listitem">Snowflake</span>
      <span class="tbadge" role="listitem">BigQuery</span>
      <span class="tbadge" role="listitem">Databricks</span>
      <span class="tbadge" role="listitem">AWS</span>
      <span class="tbadge" role="listitem">Google Cloud</span>
      <span class="tbadge" role="listitem">Azure</span>
      <span class="tbadge" role="listitem">Salesforce</span>
      <span class="tbadge" role="listitem">HubSpot</span>
      <span class="tbadge" role="listitem">Marketo</span>
      <span class="tbadge" role="listitem">Segment</span>
      <span class="tbadge" role="listitem">mParticle</span>
      <span class="tbadge" role="listitem">Amplitude</span>
      <span class="tbadge" role="listitem">Mixpanel</span>
      <span class="tbadge" role="listitem">Braze</span>
      <span class="tbadge" role="listitem">Klaviyo</span>
      <span class="tbadge" role="listitem">GA4</span>
      <span class="tbadge" role="listitem">Tableau</span>
      <span class="tbadge" role="listitem">Power BI</span>
      <span class="tbadge" role="listitem">Looker</span>
      <span class="tbadge" role="listitem">TensorFlow</span>
      <span class="tbadge" role="listitem">PyTorch</span>
      <span class="tbadge" role="listitem">OpenAI / GPT-4</span>
      <span class="tbadge" role="listitem">LangChain</span>
      <span class="tbadge" role="listitem">Apache Airflow</span>
      <span class="tbadge" role="listitem">Kafka</span>
      <span class="tbadge" role="listitem">Vertex AI</span>
      <span class="tbadge" role="listitem">Meta Ads API</span>
      <span class="tbadge" role="listitem">Google Ads API</span>
    </div>
  </div>
</div>

<!-- ======================== FAQ ======================== -->
<section class="faq-section" aria-labelledby="faq-heading">
  <div class="container">
    <div class="sec-header reveal">
      <div class="sec-label">Common Questions</div>
      <h2 class="sec-title" id="faq-heading">Frequently Asked Questions</h2>
      <p class="sec-sub">Have a question not answered here? <a href="#contact" style="color:var(--blue-2);">Reach out directly</a> and we'll respond within one business day.</p>
    </div>
    <div class="faq-list" role="list">

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          What types of organizations do you work with?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>We partner with CMOs, marketing directors, founders, and growth leaders across a broad range of organizations — from mid-to-large enterprises optimizing marketing spend at scale, to growth-stage startups building their first customer intelligence infrastructure. If your challenge involves customers, data, or growth, we can help.</p>
        </div>
      </div>

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          How is this different from a traditional marketing agency?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>Traditional agencies focus on creative execution and media buying. We focus on the intelligence layer underneath — the segmentation models, attribution frameworks, and predictive systems that make every campaign smarter and every dollar more accountable. We make your existing agency more effective, or replace the need for one entirely.</p>
        </div>
      </div>

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          How long does a typical engagement take?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>Marketing audits and segmentation assessments typically run 4–6 weeks. Full attribution framework builds and AI personalization deployments range from 10–20 weeks. We also offer ongoing advisory retainers for organizations that want continuous marketing intelligence support. We'll scope accurately on our discovery call.</p>
        </div>
      </div>

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          Do you integrate with our existing MarTech stack?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>Yes — always. We work within and around your existing platforms (Salesforce, HubSpot, Segment, GA4, and more) rather than replacing them. Our role is to extract maximum intelligence from the tools you already have, and recommend additions only when the ROI is clear and justified.</p>
        </div>
      </div>

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          How do you measure success?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>Against pre-agreed, financial business KPIs — not impressions, clicks, or vanity metrics. Before any engagement begins, we align on what success looks like in measurable terms: pipeline growth, CAC reduction, LTV improvement, conversion rate uplift. We track and report transparently throughout.</p>
        </div>
      </div>

      <div class="faq-item" role="listitem">
        <button class="faq-question" aria-expanded="false">
          Can you work alongside our internal marketing team?
          <span class="faq-icon" aria-hidden="true">+</span>
        </button>
        <div class="faq-answer">
          <p>Yes — and this is often our most effective model. We integrate as a senior extension of your team: setting intelligence strategy, building the models, and upskilling your marketers in the process. We're not here to replace internal capability — we're here to give it an unfair advantage.</p>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ======================== CONTACT ======================== -->
<section id="contact" class="contact-section" aria-labelledby="contact-heading">
  <div class="contact-inner">
    <div class="contact-info reveal">
      <div class="sec-label">Get in Touch</div>
      <h2 id="contact-heading">Let's Build Your Marketing Intelligence Advantage</h2>
      <p>Whether you're looking to understand your customers more precisely, attribute marketing spend more accurately, deploy AI-powered personalization, or simply clarify your growth strategy — we're ready to help you move forward with confidence.</p>
      <div class="c-methods">
        <a href="mailto:ezequiel@apexdata.cloud" class="c-method" onclick="gtag('event','click',{event_category:'Contact',event_label:'Email'})">
          <div class="c-ico" aria-hidden="true">&#9993;&#65039;</div>
          <div>
            <div class="c-lbl">Email</div>
            <div class="c-val">ezequiel@apexdata.cloud</div>
          </div>
        </a>
      </div>
      <div class="c-guarantee">
        <div class="c-guarantee-ico" aria-hidden="true">&#9989;</div>
        <p><strong>We respond within one business day.</strong> Every inquiry is reviewed personally — no automated responses, no sales handoffs. You'll speak directly with a senior advisor.</p>
      </div>
    </div>

    <div class="c-form-box reveal reveal-delay-2">
      <div id="formContent">
        <div class="cf-head">Start a Conversation</div>
        <div class="cf-sub">Tell us about your challenge. We'll respond within one business day.</div>
        <form action="https://formspree.io/f/xqedrddj" method="POST" id="contactForm" novalidate>
          <div class="fg-row">
            <div class="fg">
              <label for="first_name">First Name</label>
              <input type="text" id="first_name" name="first_name" placeholder="Jane" required autocomplete="given-name">
            </div>
            <div class="fg">
              <label for="last_name">Last Name</label>
              <input type="text" id="last_name" name="last_name" placeholder="Smith" required autocomplete="family-name">
            </div>
          </div>
          <div class="fg">
            <label for="email">Work Email</label>
            <input type="email" id="email" name="email" placeholder="jane@company.com" required autocomplete="email">
          </div>
          <div class="fg">
            <label for="company">Company</label>
            <input type="text" id="company" name="company" placeholder="Company name" autocomplete="organization">
          </div>
          <div class="fg">
            <label for="interest">Area of Interest</label>
            <select id="interest" name="interest">
              <option value="" disabled selected>Select a service...</option>
              <option>Customer Segmentation &amp; Audience Intelligence</option>
              <option>Marketing Analytics &amp; Attribution</option>
              <option>AI-Powered Personalization</option>
              <option>Demand Generation &amp; Growth Analytics</option>
              <option>AI &amp; Machine Learning Advisory</option>
              <option>Generative AI &amp; LLM Strategy</option>
              <option>Data &amp; MarTech Strategy</option>
              <option>Cloud &amp; Data Platform Architecture</option>
              <option>Data Governance &amp; Compliance</option>
              <option>General Inquiry</option>
            </select>
          </div>
          <div class="fg">
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="4" placeholder="Briefly describe your challenge or objective..."></textarea>
          </div>
          <button type="submit" class="cf-submit" id="submitBtn">Send Message &#8594;</button>
        </form>
      </div>
      <div class="form-success" id="formSuccess">
        <div class="form-success-icon" aria-hidden="true">&#10003;</div>
        <h3>Message Received</h3>
        <p>Thank you for reaching out. A senior advisor will be in touch within one business day.</p>
      </div>
    </div>
  </div>
</section>

<!-- ======================== FOOTER ======================== -->
<footer class="footer" role="contentinfo">
  <div class="footer-top">
    <div class="f-brand">
      <div class="f-brand-row">
        <img src="apex_logo.PNG" alt="Apex Data &amp; Marketing Cloud" width="30" height="30">
        <span class="f-brand-name">Apex Data &amp; Marketing Cloud</span>
      </div>
      <p class="f-brand-desc">AI-Powered Marketing Intelligence — helping CMOs, founders, and growth leaders turn customer data into measurable revenue and sustainable competitive advantage.</p>
      <div class="f-social" aria-label="Contact">
        <a href="mailto:ezequiel@apexdata.cloud" class="f-social-link" aria-label="Email us">
          &#9993;
        </a>
      </div>
    </div>
    <div class="f-col">
      <h5>Services</h5>
      <ul role="list">
        <li><a href="#services">Customer Segmentation</a></li>
        <li><a href="#services">Marketing Analytics</a></li>
        <li><a href="#services">AI Personalization</a></li>
        <li><a href="#services">Demand Generation</a></li>
        <li><a href="#services">AI &amp; ML Advisory</a></li>
        <li><a href="#services">Data Strategy</a></li>
      </ul>
    </div>
    <div class="f-col">
      <h5>Company</h5>
      <ul role="list">
        <li><a href="#why-apex">Why Apex</a></li>
        <li><a href="#approach">Our Approach</a></li>
        <li><a href="#industries">Industries</a></li>
        <li><a href="#contact">Contact Us</a></li>
      </ul>
    </div>
    <div class="f-col">
      <h5>Contact</h5>
      <ul role="list">
        <li><a href="mailto:ezequiel@apexdata.cloud">ezequiel@apexdata.cloud</a></li>
      </ul>
    </div>
  </div>
  <div class="footer-bottom">
    <div class="f-copy">&copy; 2026 Apex Data &amp; Marketing Cloud. All rights reserved.</div>
    <div class="f-bottom-links">
      <a href="#services">Services</a>
      <a href="#approach">Approach</a>
      <a href="#contact">Contact</a>
      <a href="mailto:ezequiel@apexdata.cloud">Email Us</a>
    </div>
  </div>
</footer>

</div><!-- end .apex-site -->

<!-- ======================== DIALOGFLOW CHAT (Google) ======================== -->
<script src="https://www.gstatic.com/dialogflow-console/fast/messenger/bootstrap.js?v=1"></script>
<df-messenger
  intent="WELCOME"
  chat-title="Harvey"
  agent-id="54ef4ef9-6e87-4fa1-af93-c16c4dcfcb6f"
  language-code="en"
></df-messenger>

<!-- ======================== JAVASCRIPT ======================== -->
<script>
(function() {
  'use strict';

  // ── Scroll Progress Bar ─────────────────────────────────────────
  var progressBar = document.getElementById('scrollProgress');
  function updateProgress() {
    var scrollTop = window.pageYOffset || document.documentElement.scrollTop;
    var docHeight = document.documentElement.scrollHeight - document.documentElement.clientHeight;
    var pct = docHeight > 0 ? (scrollTop / docHeight) * 100 : 0;
    progressBar.style.width = pct + '%';
  }

  // ── Navbar scroll state ─────────────────────────────────────────
  var nav = document.getElementById('mainNav');
  function updateNav() {
    if (window.pageYOffset > 60) {
      nav.classList.add('scrolled');
    } else {
      nav.classList.remove('scrolled');
    }
  }

  // ── Mobile Menu ─────────────────────────────────────────────────
  var hamburgerBtn = document.getElementById('hamburgerBtn');
  var mobileMenu = document.getElementById('mobileMenu');
  var mobileLinks = document.querySelectorAll('.mobile-link');

  function openMenu() {
    mobileMenu.classList.add('active');
    hamburgerBtn.classList.add('open');
    hamburgerBtn.setAttribute('aria-expanded', 'true');
    document.body.style.overflow = 'hidden';
  }
  function closeMenu() {
    mobileMenu.classList.remove('active');
    hamburgerBtn.classList.remove('open');
    hamburgerBtn.setAttribute('aria-expanded', 'false');
    document.body.style.overflow = '';
  }

  hamburgerBtn.addEventListener('click', function() {
    if (mobileMenu.classList.contains('active')) {
      closeMenu();
    } else {
      openMenu();
    }
  });

  mobileLinks.forEach(function(link) {
    link.addEventListener('click', closeMenu);
  });

  // ── Scroll Reveal (Intersection Observer) ───────────────────────
  var revealEls = document.querySelectorAll('.reveal');
  if ('IntersectionObserver' in window) {
    var observer = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.12, rootMargin: '0px 0px -40px 0px' });

    revealEls.forEach(function(el) { observer.observe(el); });
  } else {
    revealEls.forEach(function(el) { el.classList.add('visible'); });
  }

  // ── Animated Counters ───────────────────────────────────────────
  var counters = document.querySelectorAll('.stat-num[data-target]');
  var countersAnimated = false;

  function animateCounter(el) {
    var target = parseFloat(el.getAttribute('data-target'));
    var suffix = el.getAttribute('data-suffix') || '';
    var decimals = parseInt(el.getAttribute('data-decimal') || '0', 10);
    var duration = 1800;
    var start = performance.now();

    function update(now) {
      var elapsed = now - start;
      var progress = Math.min(elapsed / duration, 1);
      var ease = 1 - Math.pow(1 - progress, 3);
      var current = ease * target;
      el.textContent = (decimals > 0 ? current.toFixed(decimals) : Math.round(current)) + suffix;
      if (progress < 1) requestAnimationFrame(update);
    }
    requestAnimationFrame(update);
  }

  if ('IntersectionObserver' in window && counters.length) {
    var counterObserver = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting && !countersAnimated) {
          countersAnimated = true;
          counters.forEach(animateCounter);
          counterObserver.disconnect();
        }
      });
    }, { threshold: 0.3 });
    counterObserver.observe(document.querySelector('.stats-section'));
  }

  // ── FAQ Accordion ───────────────────────────────────────────────
  var faqItems = document.querySelectorAll('.faq-item');
  faqItems.forEach(function(item) {
    var btn = item.querySelector('.faq-question');
    btn.addEventListener('click', function() {
      var isOpen = item.classList.contains('open');
      faqItems.forEach(function(i) {
        i.classList.remove('open');
        i.querySelector('.faq-question').setAttribute('aria-expanded', 'false');
      });
      if (!isOpen) {
        item.classList.add('open');
        btn.setAttribute('aria-expanded', 'true');
      }
    });
  });

  // ── Contact Form ────────────────────────────────────────────────
  var contactForm = document.getElementById('contactForm');
  var formContent = document.getElementById('formContent');
  var formSuccess = document.getElementById('formSuccess');
  var submitBtn = document.getElementById('submitBtn');

  if (contactForm) {
    contactForm.addEventListener('submit', function(e) {
      e.preventDefault();
      submitBtn.textContent = 'Sending...';
      submitBtn.disabled = true;

      var data = new FormData(contactForm);
      fetch(contactForm.action, {
        method: 'POST',
        body: data,
        headers: { 'Accept': 'application/json' }
      }).then(function(res) {
        if (res.ok) {
          formContent.style.display = 'none';
          formSuccess.style.display = 'block';
          if (typeof gtag !== 'undefined') {
            gtag('event', 'form_submit', {
              event_category: 'Contact',
              event_label: 'Contact Form'
            });
          }
        } else {
          submitBtn.textContent = 'Send Message →';
          submitBtn.disabled = false;
          alert('There was an error. Please email us directly at ezequiel@apexdata.cloud');
        }
      }).catch(function() {
        submitBtn.textContent = 'Send Message →';
        submitBtn.disabled = false;
        alert('There was an error. Please email us directly at ezequiel@apexdata.cloud');
      });
    });
  }

  // ── Throttled scroll handler ────────────────────────────────────
  var ticking = false;
  window.addEventListener('scroll', function() {
    if (!ticking) {
      requestAnimationFrame(function() {
        updateProgress();
        updateNav();
        ticking = false;
      });
      ticking = true;
    }
  }, { passive: true });

  updateNav();

})();
</script>
