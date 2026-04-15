<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0"/>
<title>Parmit Singh | Mobile Engineering Lead</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;1,9..40,300&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --navy:#0B1F3A;--navy2:#0F2645;--blue:#1D5FA8;--accent:#3B9EFF;
  --gold:#F0A500;--white:#F0F6FF;--muted:#7A9BBF;--light:#B8D0E8;
  --card:#0D2340;--border:rgba(59,158,255,0.14);
  --fh:'Syne',sans-serif;--fb:'DM Sans',sans-serif;
}
html{scroll-behavior:smooth}
body{background:var(--navy);color:var(--white);font-family:var(--fb);overflow-x:hidden;font-size:16px;line-height:1.7}
body::after{content:'';position:fixed;inset:0;background:linear-gradient(rgba(59,158,255,0.025) 1px,transparent 1px),linear-gradient(90deg,rgba(59,158,255,0.025) 1px,transparent 1px);background-size:64px 64px;pointer-events:none;z-index:0}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:200;padding:16px 60px;display:flex;align-items:center;justify-content:space-between;backdrop-filter:blur(24px);-webkit-backdrop-filter:blur(24px);background:rgba(11,31,58,0.88);border-bottom:1px solid var(--border)}
.nav-logo{font-family:var(--fh);font-weight:800;font-size:1.3rem;letter-spacing:-0.02em;color:var(--white)}
.nav-logo span{color:var(--accent)}
.nav-links{display:flex;gap:34px;list-style:none}
.nav-links a{color:var(--muted);text-decoration:none;font-size:.875rem;font-weight:500;letter-spacing:.04em;transition:color .2s}
.nav-links a:hover{color:var(--white)}
.nav-cta{background:var(--accent);color:var(--navy);padding:10px 24px;border-radius:7px;font-weight:700;font-size:.85rem;text-decoration:none;font-family:var(--fh);transition:transform .2s,box-shadow .2s;letter-spacing:.02em}
.nav-cta:hover{transform:translateY(-2px);box-shadow:0 10px 28px rgba(59,158,255,.45)}

/* HERO */
#hero{min-height:100vh;display:flex;align-items:center;padding:130px 60px 80px;position:relative;z-index:1}
.hero-inner{max-width:1100px;margin:0 auto;width:100%;display:grid;grid-template-columns:1fr auto;gap:60px;align-items:center}
.hero-tag{display:inline-flex;align-items:center;gap:8px;background:rgba(59,158,255,0.1);border:1px solid rgba(59,158,255,0.28);border-radius:100px;padding:7px 18px;font-size:.76rem;color:var(--accent);font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:28px}
.dot{width:7px;height:7px;border-radius:50%;background:#22c55e;flex-shrink:0;animation:pulse 1.8s infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.4;transform:scale(.8)}}
.hero-name{font-family:var(--fh);font-size:clamp(3rem,6vw,5.5rem);font-weight:800;line-height:1.0;letter-spacing:-0.03em;margin-bottom:4px}
.hero-name em{font-style:normal;color:var(--accent);display:block}
.hero-role{font-size:1.1rem;color:var(--muted);font-weight:300;margin:22px 0 36px;max-width:520px;line-height:1.75}
.hero-role strong{color:var(--white);font-weight:500}
.hero-stats{display:flex;gap:40px;margin-bottom:40px;flex-wrap:wrap}
.stat .num{font-family:var(--fh);font-size:2rem;font-weight:800;color:var(--white);line-height:1}
.stat .num span{color:var(--accent)}
.stat .lbl{font-size:.7rem;color:var(--muted);text-transform:uppercase;letter-spacing:.1em;margin-top:3px}
.hero-btns{display:flex;gap:14px;flex-wrap:wrap}
.btn-p{background:var(--accent);color:var(--navy);padding:13px 30px;border-radius:8px;font-weight:700;font-size:.95rem;text-decoration:none;font-family:var(--fh);transition:transform .2s,box-shadow .2s}
.btn-p:hover{transform:translateY(-3px);box-shadow:0 14px 36px rgba(59,158,255,.42)}
.btn-s{border:1px solid var(--border);color:var(--white);padding:13px 30px;border-radius:8px;font-weight:500;font-size:.95rem;text-decoration:none;transition:all .2s;backdrop-filter:blur(8px)}
.btn-s:hover{border-color:var(--accent);color:var(--accent)}

/* PHOTO */
.hero-photo-wrap{position:relative;flex-shrink:0}
.hero-photo-ring{position:absolute;inset:-14px;border:2px solid rgba(59,158,255,0.25);border-radius:50%;animation:spin 18s linear infinite}
.hero-photo-ring2{position:absolute;inset:-28px;border:1px solid rgba(59,158,255,0.1);border-radius:50%;animation:spin 28s linear infinite reverse}
@keyframes spin{to{transform:rotate(360deg)}}
.hero-photo{width:240px;height:240px;border-radius:50%;object-fit:cover;object-position:center top;border:4px solid rgba(59,158,255,0.35);display:block;position:relative;z-index:1}
.hero-glow{position:absolute;inset:-20px;background:radial-gradient(circle,rgba(29,95,168,0.3),transparent 70%);border-radius:50%;z-index:0}

/* SECTION */
.sec{padding:90px 60px;position:relative;z-index:1}
.sec-inner{max-width:1100px;margin:0 auto}
.sec-label{font-size:.72rem;color:var(--accent);font-weight:700;letter-spacing:.14em;text-transform:uppercase;margin-bottom:10px}
.sec-title{font-family:var(--fh);font-size:clamp(1.9rem,3.5vw,2.8rem);font-weight:800;letter-spacing:-0.025em;line-height:1.1;margin-bottom:14px}
.sec-sub{color:var(--muted);font-weight:300;max-width:520px;margin-bottom:52px;font-size:1rem}
.alt{background:rgba(13,35,64,0.6)}

/* WHY ME */
.why-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
.why-card{background:var(--card);border:1px solid var(--border);border-radius:14px;padding:28px;transition:transform .25s,border-color .25s}
.why-card:hover{transform:translateY(-4px);border-color:rgba(59,158,255,.38)}
.why-card .ic{font-size:2rem;margin-bottom:14px}
.why-card h3{font-family:var(--fh);font-weight:700;font-size:1rem;margin-bottom:8px}
.why-card p{color:var(--muted);font-size:.9rem;line-height:1.65}
.why-card p strong{color:var(--white)}

/* SKILLS */
.skills-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(265px,1fr));gap:14px}
.skill-card{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:22px;transition:transform .25s,border-color .25s}
.skill-card:hover{transform:translateY(-4px);border-color:rgba(59,158,255,.35)}
.skill-ic{font-size:1.7rem;margin-bottom:10px}
.skill-name{font-family:var(--fh);font-weight:700;font-size:.95rem;margin-bottom:6px}
.skill-exp{font-size:.75rem;color:var(--accent);font-weight:600;margin-bottom:10px}
.tags{display:flex;flex-wrap:wrap;gap:5px}
.tag{background:rgba(59,158,255,0.1);border:1px solid rgba(59,158,255,0.2);color:var(--accent);font-size:.7rem;padding:3px 9px;border-radius:100px;font-weight:600}

/* EXPERIENCE */
.timeline{padding-left:28px;position:relative}
.timeline::before{content:'';position:absolute;left:0;top:8px;bottom:8px;width:2px;background:linear-gradient(to bottom,var(--accent),rgba(59,158,255,0.05))}
.exp{position:relative;margin-bottom:48px}
.exp::before{content:'';position:absolute;left:-34px;top:8px;width:12px;height:12px;background:var(--accent);border-radius:50%;box-shadow:0 0 0 4px rgba(59,158,255,.15)}
.exp-date{font-size:.73rem;color:var(--accent);font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:5px}
.exp-title{font-family:var(--fh);font-size:1.2rem;font-weight:700;margin-bottom:3px}
.exp-co{font-size:.9rem;color:var(--muted);margin-bottom:14px}
.exp-co strong{color:var(--white);font-weight:500}
.exp-buls{list-style:none;display:flex;flex-direction:column;gap:7px}
.exp-buls li{color:var(--muted);font-size:.9rem;padding-left:18px;position:relative;line-height:1.6}
.exp-buls li::before{content:"→";position:absolute;left:0;color:var(--accent);font-size:.78rem;top:3px}
.exp-buls li strong{color:var(--white)}
.badges{display:flex;flex-wrap:wrap;gap:8px;margin-top:14px}
.badge{background:rgba(240,165,0,0.1);border:1px solid rgba(240,165,0,.22);color:var(--gold);font-size:.72rem;padding:4px 12px;border-radius:6px;font-weight:700}

/* PROJECTS */
.proj-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(320px,1fr));gap:18px}
.proj{background:var(--card);border:1px solid var(--border);border-radius:16px;overflow:hidden;transition:all .25s;position:relative}
.proj::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,var(--accent),var(--blue))}
.proj:hover{transform:translateY(-5px);box-shadow:0 26px 52px rgba(0,0,0,.4);border-color:rgba(59,158,255,.3)}
.proj-body{padding:26px}
.proj-ic{font-size:2rem;margin-bottom:14px}
.proj-title{font-family:var(--fh);font-weight:700;font-size:1.05rem;margin-bottom:6px}
.proj-stat{font-size:.75rem;color:var(--accent);font-weight:700;margin-bottom:10px}
.proj-desc{color:var(--muted);font-size:.87rem;line-height:1.65;margin-bottom:14px}
.proj-link{display:inline-flex;align-items:center;gap:6px;background:rgba(59,158,255,0.1);border:1px solid rgba(59,158,255,.25);color:var(--accent);font-size:.78rem;font-weight:700;padding:7px 14px;border-radius:7px;text-decoration:none;transition:all .2s;margin-top:4px}
.proj-link:hover{background:rgba(59,158,255,.2)}

/* CONTACT */
#contact{background:linear-gradient(140deg,#0F2645,var(--navy));border-top:1px solid var(--border);padding:90px 60px;position:relative;z-index:1}
.contact-inner{max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:start}
.contact-links{display:flex;flex-direction:column;gap:13px;margin-top:32px}
.cl{display:flex;align-items:center;gap:14px;padding:16px 20px;background:var(--card);border:1px solid var(--border);border-radius:12px;text-decoration:none;color:var(--white);transition:all .2s}
.cl:hover{border-color:var(--accent);transform:translateX(6px)}
.cl-ic{font-size:1.3rem;width:36px;text-align:center;flex-shrink:0}
.cl-lbl{font-size:.67rem;color:var(--muted);text-transform:uppercase;letter-spacing:.1em}
.cl-val{font-weight:500;font-size:.9rem;margin-top:1px}
.edu-cards{display:flex;flex-direction:column;gap:12px;margin-top:18px}
.edu-card{background:var(--card);border:1px solid var(--border);border-radius:10px;padding:18px 20px}
.edu-deg{font-family:var(--fh);font-weight:700;font-size:.94rem;margin-bottom:3px}
.edu-uni{color:var(--muted);font-size:.82rem}
.edu-yr{color:var(--accent);font-size:.75rem;font-weight:700;margin-top:4px}

/* CONTACT FORM */
.contact-form{display:flex;flex-direction:column;gap:14px;margin-top:32px}
.contact-form input,.contact-form textarea{background:var(--card);border:1px solid var(--border);border-radius:10px;padding:14px 16px;color:var(--white);font-family:var(--fb);font-size:.92rem;outline:none;transition:border-color .2s;resize:none}
.contact-form input:focus,.contact-form textarea:focus{border-color:var(--accent)}
.contact-form input::placeholder,.contact-form textarea::placeholder{color:var(--muted)}
.contact-form button{background:var(--accent);color:var(--navy);border:none;padding:14px;border-radius:10px;font-weight:700;font-size:.95rem;font-family:var(--fh);cursor:pointer;transition:transform .2s,box-shadow .2s}
.contact-form button:hover{transform:translateY(-2px);box-shadow:0 10px 28px rgba(59,158,255,.4)}

footer{text-align:center;padding:28px;color:var(--muted);font-size:.8rem;border-top:1px solid var(--border);position:relative;z-index:1}

/* REVEAL */
.r{opacity:0;transform:translateY(32px);transition:opacity .7s ease,transform .7s ease}
.r.v{opacity:1;transform:none}

@media(max-width:960px){
  nav{padding:16px 24px}.nav-links{display:none}
  #hero{padding:90px 24px 60px}
  .hero-inner{grid-template-columns:1fr;gap:40px}
  .hero-photo-wrap{order:-1;display:flex;justify-content:center}
  .hero-photo{width:180px;height:180px}
  .sec,#contact{padding:70px 24px}
  .contact-inner{grid-template-columns:1fr;gap:40px}
  .why-grid{grid-template-columns:1fr}
}
</style>
</head>
<body>

<nav>
  <div class="nav-logo">PS<span>.</span></div>
  <ul class="nav-links">
    <li><a href="#hero">About</a></li>
    <li><a href="#why">Why Me</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
  <a href="https://drive.google.com/file/d/YOUR_RESUME_ID/view" target="_blank" class="nav-cta">Download CV</a>
</nav>

<!-- HERO -->
<div id="hero">
  <div class="hero-inner">
    <div>
      <div class="hero-tag"><span class="dot"></span> Open to Senior / Lead Mobile Roles · Gurgaon / Remote</div>
      <h1 class="hero-name">Parmit<em>Singh</em></h1>
      <p class="hero-role">
        <strong>Mobile Engineering Lead</strong> — 9+ years building Android, Flutter & iOS apps at scale.<br>
        Architected platforms serving <strong>5M+ users</strong> with 99.9% uptime. IoT · BLE · Clean Architecture.
      </p>
      <div class="hero-stats">
        <div class="stat"><div class="num">9<span>+</span></div><div class="lbl">Years Exp</div></div>
        <div class="stat"><div class="num">5<span>M+</span></div><div class="lbl">App Users</div></div>
        <div class="stat"><div class="num">99<span>.9%</span></div><div class="lbl">Uptime</div></div>
        <div class="stat"><div class="num">6<span>+</span></div><div class="lbl">Apps Shipped</div></div>
      </div>
      <div class="hero-btns">
        <a href="#projects" class="btn-p">View My Work</a>
        <a href="#contact" class="btn-s">Get In Touch</a>
      </div>
    </div>
    <div class="hero-photo-wrap">
      <div class="hero-glow"></div>
      <div class="hero-photo-ring"></div>
      <div class="hero-photo-ring2"></div>
      <img class="hero-photo" src="data:image/jpeg;base64,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" alt="Parmit Singh"/>
    </div>
  </div>
</div>

<!-- WHY ME -->
<div class="sec alt" id="why">
  <div class="sec-inner">
    <div class="sec-label r">Why Hire Me</div>
    <h2 class="sec-title r">What Makes Me Different</h2>
    <p class="sec-sub r">I don't just write code — I own products, lead teams, and deliver results that move business metrics.</p>
    <div class="why-grid">
      <div class="why-card r">
        <div class="ic">🚀</div>
        <h3>IoT + Android Expert</h3>
        <p>One of the very few engineers who has shipped <strong>BLE + OTA firmware + IoT Wi-Fi apps at 5M+ scale</strong>. Rare combination that most teams cannot find.</p>
      </div>
      <div class="why-card r">
        <div class="ic">🏗️</div>
        <h3>Architecture Ownership</h3>
        <p>I've migrated a <strong>monolithic legacy Android app to modular Clean Architecture</strong>, reducing build time by 40% and enabling independent feature teams.</p>
      </div>
      <div class="why-card r">
        <div class="ic">📉</div>
        <h3>Cost & Speed Impact</h3>
        <p>Led Flutter adoption that <strong>cut dev cost by 30%</strong> by enabling Android + iOS delivery from a single codebase without sacrificing quality.</p>
      </div>
      <div class="why-card r">
        <div class="ic">👨‍💼</div>
        <h3>Tech Lead + IC</h3>
        <p>I operate both as an <strong>individual contributor</strong> writing production-grade Kotlin/Flutter code and as a <strong>team lead</strong> managing engineers, QA, and DevOps.</p>
      </div>
      <div class="why-card r">
        <div class="ic">🔒</div>
        <h3>Production Stability</h3>
        <p>Maintained <strong>99.9% uptime</strong> across 3 IoT apps. Set up CI/CD, crash monitoring, and automated release pipelines — so quality is baked in, not bolted on.</p>
      </div>
      <div class="why-card r">
        <div class="ic">🌐</div>
        <h3>Website & Community</h3>
        <p>Runs <strong>codeplayon.com</strong> — a developer resource site. Active on Stack Overflow. Demonstrates passion for engineering beyond the day job.</p>
      </div>
    </div>
  </div>
</div>

<!-- SKILLS -->
<div class="sec" id="skills">
  <div class="sec-inner">
    <div class="sec-label r">Technical Stack</div>
    <h2 class="sec-title r">What I Build With</h2>
    <p class="sec-sub r">Deep expertise across the full mobile stack — architecture, hardware integration, and CI/CD.</p>
    <div class="skills-grid">
      <div class="skill-card r"><div class="skill-ic">🤖</div><div class="skill-name">Android</div><div class="skill-exp">7+ Years · Expert</div><div class="tags"><span class="tag">Kotlin</span><span class="tag">Java</span><span class="tag">Jetpack Compose</span><span class="tag">XML</span><span class="tag">Android SDK</span></div></div>
      <div class="skill-card r"><div class="skill-ic">🦋</div><div class="skill-name">Cross-Platform</div><div class="skill-exp">3+ Years · Proficient</div><div class="tags"><span class="tag">Flutter</span><span class="tag">Dart</span><span class="tag">SwiftUI</span><span class="tag">iOS</span></div></div>
      <div class="skill-card r"><div class="skill-ic">🏛️</div><div class="skill-name">Architecture</div><div class="skill-exp">5+ Years · Expert</div><div class="tags"><span class="tag">Clean Arch</span><span class="tag">MVVM</span><span class="tag">Modular</span><span class="tag">Hilt</span></div></div>
      <div class="skill-card r"><div class="skill-ic">🔵</div><div class="skill-name">IoT & BLE</div><div class="skill-exp">4+ Years · Expert</div><div class="tags"><span class="tag">Bluetooth BLE</span><span class="tag">OTA Firmware</span><span class="tag">Wi-Fi IoT</span><span class="tag">AR Core</span></div></div>
      <div class="skill-card r"><div class="skill-ic">📡</div><div class="skill-name">Networking</div><div class="skill-exp">7+ Years · Expert</div><div class="tags"><span class="tag">Retrofit</span><span class="tag">REST API</span><span class="tag">Coroutines</span><span class="tag">Kotlin Flow</span></div></div>
      <div class="skill-card r"><div class="skill-ic">🔥</div><div class="skill-name">Firebase</div><div class="skill-exp">5+ Years · Proficient</div><div class="tags"><span class="tag">Crashlytics</span><span class="tag">Analytics</span><span class="tag">Push Notif</span><span class="tag">Auth</span></div></div>
      <div class="skill-card r"><div class="skill-ic">⚙️</div><div class="skill-name">CI/CD & DevOps</div><div class="skill-exp">4+ Years · Proficient</div><div class="tags"><span class="tag">GitHub</span><span class="tag">Azure DevOps</span><span class="tag">Pipelines</span><span class="tag">Play Store</span></div></div>
      <div class="skill-card r"><div class="skill-ic">👥</div><div class="skill-name">Leadership</div><div class="skill-exp">3+ Years · Strong</div><div class="tags"><span class="tag">Team Lead</span><span class="tag">Agile/Scrum</span><span class="tag">Mentoring</span><span class="tag">Product</span></div></div>
    </div>
  </div>
</div>

<!-- EXPERIENCE -->
<div class="sec alt" id="experience">
  <div class="sec-inner">
    <div class="sec-label r">Career</div>
    <h2 class="sec-title r">Work Experience</h2>
    <p class="sec-sub r">9 years of building and shipping production mobile applications across India's leading companies.</p>
    <div class="timeline">
      <div class="exp r">
        <div class="exp-date">Apr 2023 – Present · 2+ Yrs</div>
        <div class="exp-title">Mobile Engineering Lead</div>
        <div class="exp-co"><strong>Luminous Power Technologies</strong> · Android · Flutter · IoT · BLE · Team of 6+</div>
        <ul class="exp-buls">
          <li>Architected 3 IoT-connected energy apps with <strong>5M+ combined installs & 99.9% uptime</strong></li>
          <li>Migrated monolithic Android app to modular Clean Architecture — <strong>build time ↓ 40%</strong></li>
          <li>Led Flutter adoption for cross-platform delivery — <strong>dev cost ↓ 30%</strong></li>
          <li>Manage cross-functional team: Mobile Engineers, QA, UI/UX, DevOps</li>
          <li>Own CI/CD pipeline, Play Store / App Store releases, stakeholder reporting to CTO</li>
        </ul>
        <div class="badges"><span class="badge">Luminous ConnectX</span><span class="badge">LitCore</span><span class="badge">SYNC-XBLE</span></div>
      </div>
      <div class="exp r">
        <div class="exp-date">Feb 2020 – Apr 2023 · 3 Yrs</div>
        <div class="exp-title">Senior Software Engineer / Acting Tech Lead</div>
        <div class="exp-co"><strong>Bellurbis LLC</strong> · Flutter · Android · iOS · Fintech · EV</div>
        <ul class="exp-buls">
          <li>Technical lead for SPIN EV Charging App (Flutter – Android & iOS) for Exicom</li>
          <li>Delivered Aavas Loan App — 100k+ customers, EMI, payment, branch locator</li>
          <li>Built Technical & Risk Evaluation App for Aavas field agents</li>
          <li>Mentored junior engineers, led code reviews, defined team standards</li>
        </ul>
        <div class="badges"><span class="badge">SPIN EV</span><span class="badge">Aavas Loan</span><span class="badge">Risk Eval</span></div>
      </div>
      <div class="exp r">
        <div class="exp-date">Jul 2017 – Feb 2020 · 2.5 Yrs</div>
        <div class="exp-title">Android Software Developer</div>
        <div class="exp-co"><strong>3DLogic Pvt. Ltd.</strong> · Android · Java · REST APIs</div>
        <ul class="exp-buls">
          <li>Built RO Care India Partner, Service Engineer & Customer apps — full service ecosystem</li>
          <li>Vendor management, job dispatch, and customer-facing service booking</li>
        </ul>
      </div>
      <div class="exp r">
        <div class="exp-date">Jul 2016 – Jun 2017 · 1 Yr</div>
        <div class="exp-title">Android Software Developer</div>
        <div class="exp-co"><strong>Ideating Solutions Pvt. Ltd.</strong> · Android · NFC · Security</div>
        <ul class="exp-buls">
          <li>S3 Smart Society Security — NFC-based visitor access control (Guard + Resident apps)</li>
          <li>Enterprise Office Attendance App with NFC card integration</li>
        </ul>
      </div>
    </div>
  </div>
</div>

<!-- PROJECTS -->
<div class="sec" id="projects">
  <div class="sec-inner">
    <div class="sec-label r">Featured Work</div>
    <h2 class="sec-title r">Apps I've Built & Shipped</h2>
    <p class="sec-sub r">Live on Play Store. Real users. Real impact.</p>
    <div class="proj-grid">

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">☀️</div>
          <div class="proj-title">Luminous ConnectX</div>
          <div class="proj-stat">📈 5M+ Downloads · IoT Solar Energy</div>
          <div class="proj-desc">Real-time solar generation monitoring, ROI tracking, home consumption analytics and power cut alerts for Solarverter Pro, Hybrid & PCU inverters via IoT Wi-Fi Dongle.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Android</span><span class="tag">Kotlin</span><span class="tag">IoT</span><span class="tag">Wi-Fi Dongle</span><span class="tag">MVVM</span></div>
          <a href="https://play.google.com/store/apps/details?id=com.luminous.connectx&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">📶</div>
          <div class="proj-title">SYNC-X BLE</div>
          <div class="proj-stat">📈 BLE OTA · IoT Firmware</div>
          <div class="proj-desc">BLE app for IoT Wi-Fi device OTA firmware upgrades, device log storage, BMS battery integration and real-time BLE device configuration management.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Kotlin</span><span class="tag">BLE</span><span class="tag">OTA</span><span class="tag">IoT</span><span class="tag">Firmware</span></div>
          <a href="https://play.google.com/store/apps/details?id=com.luminous.luminoussyncx&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">⚡</div>
          <div class="proj-title">SPIN EV Charging</div>
          <div class="proj-stat">📈 Flutter · Android & iOS</div>
          <div class="proj-desc">Cross-platform EV charging app by Exicom — station discovery, charging control, real-time session monitoring, and integrated payments. Flutter for Android & iOS.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Flutter</span><span class="tag">Dart</span><span class="tag">Android</span><span class="tag">iOS</span></div>
          <a href="https://play.google.com/store/apps/details?id=com.exicom.android.spinev&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">🏠</div>
          <div class="proj-title">Aavas Loan App</div>
          <div class="proj-stat">📈 Fintech · 100k+ Customers</div>
          <div class="proj-desc">Home & MSME loan management for Aavas Financiers — loan tracking, EMI calculator, payment history, branch locator and dues management.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Android</span><span class="tag">Kotlin</span><span class="tag">Fintech</span><span class="tag">Google Maps</span></div>
          <a href="https://play.google.com/store/apps/details?id=com.aavas.homeloan&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">💧</div>
          <div class="proj-title">RO Care India Partner</div>
          <div class="proj-stat">📈 Vendor Management · B2B</div>
          <div class="proj-desc">Vendor and partner management platform for water RO service network — job allocation, partner tracking, and service management.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Android</span><span class="tag">Java</span><span class="tag">REST API</span><span class="tag">GPS</span></div>
          <a href="https://play.google.com/store/apps/details?id=com.rawlab.vms&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

      <div class="proj r">
        <div class="proj-body">
          <div class="proj-ic">🔧</div>
          <div class="proj-title">RO Care Service Engineer</div>
          <div class="proj-stat">📈 Field Service · B2B</div>
          <div class="proj-desc">Field engineer management app — job dispatch, service scheduling, RO installation and repair tracking for service engineers across India.</div>
          <div class="tags" style="margin-bottom:14px"><span class="tag">Android</span><span class="tag">Java</span><span class="tag">Firebase</span><span class="tag">Maps</span></div>
          <a href="https://play.google.com/store/apps/details?id=in.rocareindia.com.rocareindiaems&hl=en_IN" target="_blank" class="proj-link">▶ View on Play Store</a>
        </div>
      </div>

    </div>
  </div>
</div>

<!-- CONTACT -->
<div id="contact">
  <div class="contact-inner">
    <div>
      <div class="sec-label r">Let's Connect</div>
      <h2 class="sec-title r">Open to New<br>Opportunities</h2>
      <p class="sec-sub r" style="margin-bottom:0">Looking for Senior Android, Mobile Tech Lead, or Staff Engineer roles. Available in Gurgaon / Remote / Bengaluru / Hyderabad.</p>
      <div class="contact-links r">
        <a href="mailto:malik.parmit@gmail.com" class="cl"><div class="cl-ic">✉️</div><div><div class="cl-lbl">Email</div><div class="cl-val">malik.parmit@gmail.com</div></div></a>
        <a href="tel:+919671718285" class="cl"><div class="cl-ic">📱</div><div><div class="cl-lbl">Phone</div><div class="cl-val">+91-9671718285</div></div></a>
        <a href="https://www.linkedin.com/in/parmit-singh-malik-918372255/" target="_blank" class="cl"><div class="cl-ic">💼</div><div><div class="cl-lbl">LinkedIn</div><div class="cl-val">parmit-singh-malik</div></div></a>
        <a href="https://github.com/codeplayon" target="_blank" class="cl"><div class="cl-ic">💻</div><div><div class="cl-lbl">GitHub</div><div class="cl-val">github.com/codeplayon</div></div></a>
        <a href="https://stackoverflow.com/users/12225347/parmit-singh-malik" target="_blank" class="cl"><div class="cl-ic">📚</div><div><div class="cl-lbl">Stack Overflow</div><div class="cl-val">parmit-singh-malik</div></div></a>
        <a href="https://www.codeplayon.com/" target="_blank" class="cl"><div class="cl-ic">🌐</div><div><div class="cl-lbl">Website</div><div class="cl-val">codeplayon.com</div></div></a>
      </div>
    </div>
    <div>
      <div class="sec-label r">Education</div>
      <div class="edu-cards r">
        <div class="edu-card">
          <div class="edu-deg">Master of Computer Applications (MCA)</div>
          <div class="edu-uni">N.C. College of Engineering, Kurukshetra University, Panipat</div>
          <div class="edu-yr">2016</div>
        </div>
        <div class="edu-card">
          <div class="edu-deg">Bachelor of Computer Applications (BCA)</div>
          <div class="edu-uni">Govt. PG College Gohana, MDU Rohtak, Haryana</div>
          <div class="edu-yr">2013</div>
        </div>
      </div>
      <div class="sec-label r" style="margin-top:32px;margin-bottom:14px">Send a Message</div>
      <form class="contact-form r" onsubmit="handleSubmit(event)">
        <input type="text" placeholder="Your Name" required/>
        <input type="email" placeholder="Your Email" required/>
        <input type="text" placeholder="Subject (e.g. Job Opportunity at Razorpay)"/>
        <textarea rows="4" placeholder="Your message..."></textarea>
        <button type="submit">Send Message ✉️</button>
      </form>
    </div>
  </div>
</div>

<footer>
  <p>© 2026 Parmit Singh · Mobile Engineering Lead · <a href="https://www.codeplayon.com/" style="color:var(--accent);text-decoration:none">codeplayon.com</a> · Built with ❤️</p>
</footer>

<script>
const obs = new IntersectionObserver(entries => {
  entries.forEach((e,i) => { if(e.isIntersecting){ setTimeout(()=>e.target.classList.add("v"),i*60); } });
},{threshold:0.1});
document.querySelectorAll(".r").forEach(el=>obs.observe(el));

function handleSubmit(e){
  e.preventDefault();
  const btn=e.target.querySelector("button");
  btn.textContent="✅ Message Sent!";
  btn.style.background="#22c55e";
  setTimeout(()=>{btn.textContent="Send Message ✉️";btn.style.background="";e.target.reset();},3000);
}
</script>
</body>
</html>
