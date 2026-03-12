---
# https://vitepress.dev/reference/default-theme-home-page
layout: home

hero:
  name: "DTI Notes"
  text: "Digital Technology & Innovation"
  tagline: "The Elite Convergence of Logic and Disruption"
  actions:
    - theme: brand
      text: "Refer Notes"
      link: "/computer-science/terminal"
    - theme: alt
      text: "Innovation Roadmap"
      link: "#roadmap"

features:
  - icon: 🛰️
    title: "Computing Core"
    details: "Master the low-level logic, OS architectures, and hardware protocols that underpin the digital world."
  - icon: ⚡
    title: "Digital Strategy"
    details: "Architecting disruption. Navigating the shift from legacy systems to agile innovation."
  - icon: 🌌
    title: "Innovation Lab"
    details: "Deep dives into Neural Networks, Quantum Logic, and high-performance Terminal workflows."
---

<div class="premium-wrapper">
<div class="orb orb-1"></div>
<div class="orb orb-2"></div>
<div class="orb orb-3"></div>
<div class="glass-content">
<div class="status-badge">SYSTEMS ACTIVE</div>
<h1 class="main-title">🚀 Welcome to the Future</h1>
<p class="description">A specialized knowledge base for <strong>Digital Technology & Innovation</strong>. Designed for those who code the future and lead the disruption.</p>
<div class="quick-stats">
<div class="stat-item">
<span class="count">01</span>
<span class="label">Research</span>
</div>
<div class="stat-item">
<span class="count">02</span>
<span class="label">Architect</span>
</div>
<div class="stat-item">
<span class="count">03</span>
<span class="label">Deploy</span>
</div>
</div>
</div>
<section id="roadmap" class="roadmap-section">
<h2 class="section-title">Innovation Roadmap</h2>
<div class="roadmap-grid">
<div class="roadmap-card">
<div class="step-num">PHASE I</div>
<h3>Foundation</h3>
<p>Linux Internals, Networking Protocols, and System Architecture.</p>
</div>
<div class="roadmap-card">
<div class="step-num">PHASE II</div>
<h3>Strategy</h3>
<p>Digital Transformation frameworks and Disruption engineering.</p>
</div>
<div class="roadmap-card">
<div class="step-num">PHASE III</div>
<h3>Future</h3>
<p>AI Integration, Quantum Computing, and Advanced Security.</p>
</div>
</div>
</section>
</div>

<style>
:root {
  --vp-home-hero-name-color: transparent;
  --vp-home-hero-name-background: linear-gradient(135deg, #00d2ff 0%, #3a7bd5 100%);
  --brand-glow: rgba(0, 210, 255, 0.4);
}

.premium-wrapper {
    position: relative;
    padding: 6rem 1.5rem;
    overflow: hidden;
    min-height: 80vh;
}

.orb {
    position: absolute;
    border-radius: 50%;
    filter: blur(80px);
    z-index: -1;
    opacity: 0.4;
    animation: float 20s infinite alternate ease-in-out;
}

.orb-1 { width: 300px; height: 300px; background: #3a7bd5; top: 10%; left: -5%; }
.orb-2 { width: 400px; height: 400px; background: #00d2ff; bottom: 10%; right: -5%; animation-delay: -5s; }
.orb-3 { width: 250px; height: 250px; background: #42d392; top: 40%; left: 40%; animation-delay: -10s; }

@keyframes float {
    from { transform: translate(0, 0) scale(1); }
    to { transform: translate(30px, 50px) scale(1.1); }
}

.glass-content {
    background: rgba(var(--vp-c-bg-soft-rgb), 0.7);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: 32px;
    padding: 4rem 2rem;
    max-width: 900px;
    margin: 0 auto;
    text-align: center;
    box-shadow: 0 20px 50px rgba(0, 0, 0, 0.2);
}

.status-badge {
    display: inline-block;
    padding: 6px 16px;
    background: rgba(0, 210, 255, 0.1);
    border: 1px solid #00d2ff;
    color: #00d2ff;
    border-radius: 50px;
    font-size: 0.75rem;
    font-weight: bold;
    letter-spacing: 2px;
    margin-bottom: 2rem;
}

.main-title {
    font-size: 3.5rem !important;
    font-weight: 900 !important;
    margin-bottom: 1.5rem !important;
    letter-spacing: -2px !important;
    background: linear-gradient(to bottom right, #fff, #999);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.description {
    font-size: 1.25rem !important;
    line-height: 1.8 !important;
    color: var(--vp-c-text-2) !important;
    max-width: 600px;
    margin: 0 auto 3rem !important;
}

.quick-stats {
    display: flex;
    justify-content: center;
    gap: 4rem;
}

.stat-item {
    display: flex;
    flex-direction: column;
}

.stat-item .count {
    font-size: 2rem;
    font-weight: 800;
    color: var(--vp-c-brand);
}

.stat-item .label {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    color: var(--vp-c-text-3);
}

.roadmap-section {
    margin-top: 10rem;
    text-align: center;
}

.section-title {
    font-size: 2.5rem !important;
    font-weight: 800 !important;
    margin-bottom: 4rem !important;
}

.roadmap-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    max-width: 1100px;
    margin: 0 auto;
}

.roadmap-card {
    background: var(--vp-c-bg-soft);
    padding: 2.5rem;
    border-radius: 24px;
    border: 1px solid var(--vp-c-divider);
    text-align: left;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.roadmap-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; width: 100%; height: 100%;
    background: radial-gradient(circle at top left, var(--brand-glow), transparent);
    opacity: 0;
    transition: opacity 0.3s ease;
}

.roadmap-card:hover {
    transform: translateY(-10px);
    border-color: #00d2ff;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
}

.roadmap-card:hover::before {
    opacity: 1;
}

.step-num {
    font-weight: bold;
    color: #00d2ff;
    font-size: 0.8rem;
    letter-spacing: 2px;
    margin-bottom: 1rem;
}

.roadmap-card h3 {
    margin-top: 0 !important;
    font-size: 1.5rem !important;
    margin-bottom: 1rem !important;
}

:deep(.VPFeature) {
    transition: all 0.3s ease !important;
}

:deep(.VPFeature:hover) {
    border-color: #00d2ff !important;
    box-shadow: 0 0 20px var(--brand-glow) !important;
    transform: scale(1.02);
}

@media (max-width: 768px) {
    .main-title { font-size: 2.5rem !important; }
    .quick-stats { gap: 2rem; }
    .roadmap-section { margin-top: 5rem; }
}
</style>
