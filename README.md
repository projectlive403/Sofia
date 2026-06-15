<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Evangelin Sofia F — MERN Stack Developer</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Inter:wght@300;400;500&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --dark:#0f0f0f;
  --dark2:#1a1a1a;
  --dark3:#252525;
  --dark-border:#333333;
  --gold:#c9a84c;
  --gold2:#e8c97a;
  --light:#f9f7f4;
  --light2:#ffffff;
  --light3:#f0ede8;
  --ink:#1c1c1c;
  --ink2:#3f3d3a;
  --ink3:#6e6b66;
  --rule:#e0dbd4;
  --rule2:#ccc8c0;
  --blue:#1e4d7b;
  --serif:'Playfair Display',Georgia,serif;
  --sans:'Inter',sans-serif;
  --mono:'JetBrains Mono',monospace;
}
html{scroll-behavior:smooth}
body{background:var(--light);color:var(--ink);font-family:var(--sans);font-weight:300;font-size:15px;line-height:1.7}

/* ── NAV ── */
nav{
  background:var(--dark);
  padding:0 4rem;
  display:flex;align-items:stretch;justify-content:space-between;
  position:sticky;top:0;z-index:100;
  border-bottom:1px solid var(--dark-border);
}
.nav-brand{
  display:flex;align-items:center;gap:10px;
  font-family:var(--serif);
  font-size:1rem;
  font-weight:600;
  color:#fff;
  padding:1.1rem 0;
  border-right:1px solid var(--dark-border);
  padding-right:2rem;
  letter-spacing:0.02em;
}
.nav-dot{width:7px;height:7px;background:var(--gold);border-radius:50%}
.nav-links{display:flex;list-style:none}
.nav-links li{border-left:1px solid var(--dark-border)}
.nav-links a{
  display:flex;align-items:center;
  padding:0 1.5rem;
  font-family:var(--mono);
  font-size:10.5px;
  letter-spacing:0.14em;
  text-transform:uppercase;
  color:#888;
  text-decoration:none;
  height:100%;
  transition:color 0.15s,background 0.15s;
}
.nav-links a:hover{color:var(--gold);background:var(--dark2)}

/* ── HERO (DARK) ── */
.hero{
  background:var(--dark);
  color:#fff;
  padding:5rem 4rem 0;
  border-bottom:1px solid var(--dark-border);
}
.hero-inner{
  display:grid;
  grid-template-columns:1fr 300px;
  gap:4rem;
  align-items:end;
  padding-bottom:3.5rem;
  border-bottom:1px solid var(--dark-border);
}
.hero-eyebrow{
  font-family:var(--mono);
  font-size:10.5px;
  letter-spacing:0.25em;
  text-transform:uppercase;
  color:var(--gold);
  margin-bottom:1.3rem;
  display:flex;align-items:center;gap:12px;
}
.hero-eyebrow::before{content:'';width:28px;height:1px;background:var(--gold)}
h1{
  font-family:var(--serif);
  font-size:clamp(3rem,6vw,5.2rem);
  font-weight:700;
  line-height:0.98;
  letter-spacing:-0.01em;
  color:#fff;
  margin-bottom:1rem;
}
h1 span{color:var(--gold)}
.hero-role{
  font-family:var(--serif);
  font-size:1.1rem;
  font-style:italic;
  color:#888;
  margin-bottom:2rem;
  letter-spacing:0.02em;
}
.hero-summary{
  font-size:14px;
  color:#bbb;
  max-width:520px;
  line-height:1.9;
  padding-left:1rem;
  border-left:2px solid var(--gold);
  font-weight:300;
}
.hero-right{padding-bottom:0.5rem}
.hero-contact{list-style:none}
.hero-contact li{
  padding:0.8rem 0;
  border-bottom:1px solid var(--dark-border);
  display:flex;flex-direction:column;gap:2px;
}
.hero-contact li:last-child{border-bottom:none}
.hc-label{
  font-family:var(--mono);
  font-size:9.5px;
  letter-spacing:0.2em;
  text-transform:uppercase;
  color:#555;
}
.hc-val{font-size:13px;color:#ccc}
.hc-val a{color:var(--gold);text-decoration:none}
.hc-val a:hover{color:var(--gold2)}

/* HERO STATS BAR */
.hero-stats{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  border-top:1px solid var(--dark-border);
}
.stat-item{
  padding:1.4rem 2rem;
  border-right:1px solid var(--dark-border);
  text-align:center;
}
.stat-item:last-child{border-right:none}
.stat-num{
  font-family:var(--serif);
  font-size:1.8rem;
  font-weight:700;
  color:var(--gold);
  line-height:1;
  margin-bottom:0.3rem;
}
.stat-label{
  font-family:var(--mono);
  font-size:9.5px;
  letter-spacing:0.14em;
  text-transform:uppercase;
  color:#555;
}

/* ── BODY LAYOUT ── */
.body-wrap{display:grid;grid-template-columns:290px 1fr}

/* ── SIDEBAR (LIGHT) ── */
.sidebar{
  background:var(--light2);
  border-right:1px solid var(--rule2);
  padding:2.8rem 2.2rem;
}
.sb-sec{margin-bottom:2.5rem}
.sb-sec:last-child{margin-bottom:0}
.sb-head{
  font-family:var(--mono);
  font-size:9.5px;
  letter-spacing:0.24em;
  text-transform:uppercase;
  color:var(--ink3);
  padding-bottom:0.6rem;
  border-bottom:2px solid var(--ink);
  margin-bottom:1.3rem;
}

.edu-item{margin-bottom:1.6rem}
.edu-item:last-child{margin-bottom:0}
.edu-deg{
  font-family:var(--serif);
  font-size:0.92rem;
  font-weight:600;
  color:var(--ink);
  line-height:1.35;
  margin-bottom:0.2rem;
}
.edu-meta{font-size:11.5px;color:var(--ink3);line-height:1.5}
.edu-year{
  display:inline-block;
  margin-top:0.3rem;
  font-family:var(--mono);
  font-size:10px;
  color:var(--light2);
  background:var(--blue);
  padding:1px 8px;
}

.cert-item{
  display:flex;align-items:center;gap:9px;
  padding:0.55rem 0;
  border-bottom:1px solid var(--rule);
  font-size:12.5px;
  color:var(--ink2);
}
.cert-item:last-child{border-bottom:none}
.cert-sq{width:5px;height:5px;background:var(--gold);flex-shrink:0}

.sg{margin-bottom:1.3rem}
.sg:last-child{margin-bottom:0}
.sg-lbl{font-size:10.5px;font-weight:500;letter-spacing:0.08em;text-transform:uppercase;color:var(--ink3);margin-bottom:0.5rem}
.tags{display:flex;flex-wrap:wrap;gap:4px}
.tag{font-family:var(--mono);font-size:10px;padding:3px 9px;border:1px solid var(--rule2);color:var(--ink2);background:var(--light)}
.tag.t{border-color:#c5d6e8;color:var(--blue);background:#eef4fa}

.soft-item{
  display:flex;align-items:center;gap:8px;
  padding:0.45rem 0;
  border-bottom:1px solid var(--rule);
  font-size:12.5px;color:var(--ink2);
}
.soft-item:last-child{border-bottom:none}
.soft-item::before{content:'';width:5px;height:1px;background:var(--ink3);flex-shrink:0}

.lang-row{
  display:flex;justify-content:space-between;align-items:center;
  padding:0.5rem 0;border-bottom:1px solid var(--rule);
}
.lang-row:last-child{border-bottom:none}
.lang-name{font-size:13px;color:var(--ink2)}
.lang-badge{
  font-family:var(--mono);font-size:9.5px;
  letter-spacing:0.1em;
  padding:2px 8px;
  background:var(--light3);
  color:var(--ink3);
  border:1px solid var(--rule2);
}

/* ── MAIN CONTENT (LIGHT) ── */
.main-col{padding:2.8rem 3rem;background:var(--light)}

.sec-hdr{
  display:flex;align-items:center;gap:1rem;
  margin-bottom:2rem;
}
.sec-hdr::after{content:'';flex:1;height:1px;background:var(--rule2)}
.sec-eye{font-family:var(--mono);font-size:9.5px;letter-spacing:0.22em;text-transform:uppercase;color:var(--ink3);white-space:nowrap}
.sec-title{font-family:var(--serif);font-size:1.65rem;font-weight:700;color:var(--ink);white-space:nowrap}

/* Experience */
.exp-card{
  background:var(--light2);
  border:1px solid var(--rule2);
  margin-bottom:1rem;
  overflow:hidden;
}
.exp-card:last-child{margin-bottom:0}
.exp-card-head{
  background:var(--dark);
  padding:1.2rem 1.8rem;
  display:flex;justify-content:space-between;align-items:center;
}
.exp-card-head.muted{background:var(--dark3)}
.exp-role-name{
  font-family:var(--serif);
  font-size:1.05rem;
  font-weight:600;
  color:#fff;
}
.exp-period{
  font-family:var(--mono);
  font-size:10px;
  letter-spacing:0.1em;
  color:var(--gold);
  background:rgba(201,168,76,0.12);
  padding:3px 10px;
  border:1px solid rgba(201,168,76,0.3);
}
.exp-period.past{color:#888;background:rgba(255,255,255,0.04);border-color:#444}
.exp-card-body{padding:1.4rem 1.8rem}
.exp-co{font-size:12px;color:var(--ink3);font-style:italic;margin-bottom:1rem;letter-spacing:0.04em}
.exp-ul{list-style:none;display:flex;flex-direction:column;gap:0.4rem}
.exp-ul li{
  font-size:13.5px;color:var(--ink2);
  padding-left:1.3rem;position:relative;line-height:1.75;
}
.exp-ul li::before{
  content:'▸';position:absolute;left:0;
  color:var(--gold);font-size:10px;top:5px;
}

/* Projects */
.proj-grid{display:grid;grid-template-columns:1fr 1fr;gap:1px;background:var(--rule2);margin-bottom:0}
.proj-card{
  background:var(--light2);
  padding:1.6rem 1.8rem;
  position:relative;
  transition:background 0.15s;
}
.proj-card:hover{background:var(--light3)}
.proj-top-bar{
  height:3px;
  background:var(--dark);
  position:absolute;top:0;left:0;right:0;
}
.proj-num{font-family:var(--mono);font-size:9.5px;letter-spacing:0.18em;color:var(--ink3);margin-bottom:0.8rem;margin-top:0.4rem}
.proj-name{font-family:var(--serif);font-size:1.05rem;font-weight:700;color:var(--ink);margin-bottom:0.4rem}
.proj-desc{font-size:12.5px;color:var(--ink3);line-height:1.7;margin-bottom:0.9rem}
.proj-stack{display:flex;flex-wrap:wrap;gap:4px}
.ptag{font-family:var(--mono);font-size:10px;padding:2px 9px;background:var(--dark);color:var(--gold);border:1px solid var(--dark3)}

/* Interests */
.interest-row{
  display:grid;grid-template-columns:repeat(2,1fr);gap:1px;
  background:var(--rule2);
}
.int-cell{
  background:var(--light2);
  padding:1rem 1.4rem;
  display:flex;align-items:center;gap:10px;
  font-size:13px;color:var(--ink2);
}
.int-mark{
  font-family:var(--mono);font-size:11px;
  color:var(--gold);font-weight:500;
}

/* Main Sections spacing */
.ms{margin-bottom:3rem}
.ms:last-child{margin-bottom:0}

/* ── FOOTER ── */
footer{
  background:var(--dark);
  border-top:1px solid var(--dark-border);
  padding:1.6rem 4rem;
  display:flex;justify-content:space-between;align-items:center;
}
footer p{font-family:var(--mono);font-size:11px;color:#555;letter-spacing:0.06em}
footer span{color:var(--gold)}

@media(max-width:900px){
  nav,footer{padding-left:1.5rem;padding-right:1.5rem}
  .hero{padding:3rem 1.5rem 0}
  .hero-inner{grid-template-columns:1fr;gap:2rem;padding-bottom:2rem}
  .hero-stats{grid-template-columns:repeat(2,1fr)}
  .body-wrap{grid-template-columns:1fr}
  .sidebar{border-right:none;border-bottom:1px solid var(--rule2)}
  .main-col{padding:2rem 1.5rem}
  .proj-grid{grid-template-columns:1fr}
  .interest-row{grid-template-columns:1fr}
  footer{flex-direction:column;gap:0.5rem;text-align:center}
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-brand"><span class="nav-dot"></span>Evangelin Sofia F</div>
  <ul class="nav-links">
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- HERO — DARK -->
<header class="hero">
  <div class="hero-inner">
    <div>
      <div class="hero-eyebrow">MERN Stack Developer</div>
      <h1>Evangelin<br><span>Sofia F</span></h1>
      <p class="hero-role">Full-Stack Web Developer &nbsp;·&nbsp; Trichy, Tamil Nadu</p>
      <p class="hero-summary">MERN Stack Developer with hands-on experience in React, Node.js, MongoDB, PHP, and MySQL. Skilled in building scalable web applications, team collaboration, and project management — with a strong passion for learning new technologies.</p>
    </div>
    <div class="hero-right" id="contact">
      <ul class="hero-contact">
        <li><span class="hc-label">Email</span><span class="hc-val"><a href="mailto:evangelin.sofia24@gmail.com">evangelin.sofia24@gmail.com</a></span></li>
        <li><span class="hc-label">Phone</span><span class="hc-val"><a href="tel:+919940848276">+91 99408 48276</a></span></li>
        <li><span class="hc-label">Location</span><span class="hc-val">Tiruchirapalli, Tamil Nadu</span></li>
        <li><span class="hc-label">Current Role</span><span class="hc-val">Developer @ Astonish Info-Tech</span></li>
        <li><span class="hc-label">Status</span><span class="hc-val" style="color:var(--gold)">Open to Opportunities</span></li>
      </ul>
    </div>
  </div>
  <!-- Stats Bar -->
  <div class="hero-stats">
    <div class="stat-item">
      <div class="stat-num">2+</div>
      <div class="stat-label">Years Dev Exp</div>
    </div>
    <div class="stat-item">
      <div class="stat-num">4</div>
      <div class="stat-label">Projects Built</div>
    </div>
    <div class="stat-item">
      <div class="stat-num">9+</div>
      <div class="stat-label">Tech Skills</div>
    </div>
    <div class="stat-item">
      <div class="stat-num">MBA</div>
      <div class="stat-label">Highest Degree</div>
    </div>
  </div>
</header>

<!-- BODY — LIGHT -->
<div class="body-wrap">

  <!-- SIDEBAR -->
  <aside class="sidebar">

    <div class="sb-sec" id="education">
      <p class="sb-head">Education</p>
      <div class="edu-item">
        <p class="edu-deg">Master of Business Administration</p>
        <p class="edu-meta">Bharathidasan University, India</p>
        <span class="edu-year">2016</span>
      </div>
      <div class="edu-item">
        <p class="edu-deg">Bachelor of Business Administration</p>
        <p class="edu-meta">Bharathidasan University, India</p>
        <span class="edu-year">2011</span>
      </div>
    </div>

    <div class="sb-sec">
      <p class="sb-head">Certifications</p>
      <div class="cert-item"><span class="cert-sq"></span>MERN Stack Course</div>
      <div class="cert-item"><span class="cert-sq"></span>Computer Application</div>
    </div>

    <div class="sb-sec">
      <p class="sb-head">Technical Skills</p>
      <div class="sg"><p class="sg-lbl">Frontend</p>
        <div class="tags"><span class="tag t">React JS</span><span class="tag t">HTML</span><span class="tag t">CSS</span><span class="tag t">JavaScript</span></div>
      </div>
      <div class="sg"><p class="sg-lbl">Backend</p>
        <div class="tags"><span class="tag t">Node JS</span><span class="tag t">Express</span><span class="tag t">PHP</span></div>
      </div>
      <div class="sg"><p class="sg-lbl">Database</p>
        <div class="tags"><span class="tag t">MongoDB</span><span class="tag t">MySQL</span></div>
      </div>
      <div class="sg"><p class="sg-lbl">Tools</p>
        <div class="tags"><span class="tag">MS Office</span><span class="tag">Documentation</span></div>
      </div>
    </div>

    <div class="sb-sec">
      <p class="sb-head">Soft Skills</p>
      <div class="soft-item">Team Collaboration</div>
      <div class="soft-item">Project Management</div>
      <div class="soft-item">Critical Observation</div>
      <div class="soft-item">Decision Making</div>
    </div>

    <div class="sb-sec">
      <p class="sb-head">Languages</p>
      <div class="lang-row"><span class="lang-name">English</span><span class="lang-badge">Proficient</span></div>
      <div class="lang-row"><span class="lang-name">Tamil</span><span class="lang-badge">Native</span></div>
    </div>

  </aside>

  <!-- MAIN -->
  <main class="main-col">

    <div class="ms" id="experience">
      <div class="sec-hdr">
        <span class="sec-eye">Career</span>
        <span class="sec-title">Work Experience</span>
      </div>

      <div class="exp-card">
        <div class="exp-card-head">
          <span class="exp-role-name">MERN Stack Developer</span>
          <span class="exp-period">May 2024 — Present</span>
        </div>
        <div class="exp-card-body">
          <p class="exp-co">Astonish Info-Tech Private Limited</p>
          <ul class="exp-ul">
            <li>Designed and built websites and applications for various platforms including a responsive e-commerce site.</li>
            <li>Developed and maintained web services and APIs for social media platforms.</li>
            <li>Contributed to both front-end and back-end development for user interfaces and project management tools.</li>
          </ul>
        </div>
      </div>

      <div class="exp-card">
        <div class="exp-card-head muted">
          <span class="exp-role-name">Customer Service Associate</span>
          <span class="exp-period past">Nov 2015 — Dec 2016</span>
        </div>
        <div class="exp-card-body">
          <p class="exp-co">Minacs Pvt Ltd, Bangalore, India</p>
          <ul class="exp-ul">
            <li>Maintained accurate daily and monthly financial records, invoices, and ledgers via voice and non-voice processes.</li>
            <li>Managed branch operations and supervised staff in the manager's absence.</li>
            <li>Ensured precise financial reporting through proficient bookkeeping and documentation practices.</li>
          </ul>
        </div>
      </div>

      <div class="exp-card">
        <div class="exp-card-head muted">
          <span class="exp-role-name">Customer Service Associate</span>
          <span class="exp-period past">Oct 2013 — May 2014</span>
        </div>
        <div class="exp-card-body">
          <p class="exp-co">Muthoot Fincorp Ltd, Trichy, India</p>
          <ul class="exp-ul">
            <li>Prepared daily and monthly account statements, bills, and ledgers; verified jewellery for loan calculations.</li>
            <li>Delivered quality customer service through voice and non-voice channels.</li>
            <li>Managed branch operations and ensured smooth workflow in the manager's absence.</li>
          </ul>
        </div>
      </div>
    </div>

    <div class="ms" id="projects">
      <div class="sec-hdr">
        <span class="sec-eye">Portfolio</span>
        <span class="sec-title">Projects</span>
      </div>
      <div class="proj-grid">
        <div class="proj-card">
          <div class="proj-top-bar"></div>
          <p class="proj-num">01 ——</p>
          <p class="proj-name">The School Cool</p>
          <p class="proj-desc">School management system for student and staff activities, attendance tracking, and stock updates.</p>
          <div class="proj-stack"><span class="ptag">React</span><span class="ptag">MongoDB</span></div>
        </div>
        <div class="proj-card">
          <div class="proj-top-bar"></div>
          <p class="proj-num">02 ——</p>
          <p class="proj-name">Pay-Roll Process</p>
          <p class="proj-desc">Admin-controlled payroll generation system for managing employee compensation workflows.</p>
          <div class="proj-stack"><span class="ptag">PHP</span><span class="ptag">MySQL</span></div>
        </div>
        <div class="proj-card">
          <div class="proj-top-bar"></div>
          <p class="proj-num">03 ——</p>
          <p class="proj-name">Matrimony Portal</p>
          <p class="proj-desc">Match-finding platform to help users discover and connect with compatible partners for marriage.</p>
          <div class="proj-stack"><span class="ptag">PHP</span><span class="ptag">MySQL</span></div>
        </div>
        <div class="proj-card">
          <div class="proj-top-bar"></div>
          <p class="proj-num">04 ——</p>
          <p class="proj-name">Max Home Tuition</p>
          <p class="proj-desc">Coaching center management for attendance, timetable updates, and staff-student coordination.</p>
          <div class="proj-stack"><span class="ptag">PHP</span><span class="ptag">MySQL</span></div>
        </div>
      </div>
    </div>

    <div class="ms">
      <div class="sec-hdr">
        <span class="sec-eye">Focus</span>
        <span class="sec-title">Interests</span>
      </div>
      <div class="interest-row">
        <div class="int-cell"><span class="int-mark">01</span>Web Application Development</div>
        <div class="int-cell"><span class="int-mark">02</span>UI / UX Improvement</div>
        <div class="int-cell"><span class="int-mark">03</span>Learning New Technologies</div>
        <div class="int-cell"><span class="int-mark">04</span>Technical Environment Work</div>
      </div>
    </div>

  </main>
</div>

<!-- FOOTER — DARK -->
<footer>
  <p>© 2024 <span>Evangelin Sofia F</span> — MERN Stack Developer</p>
  <p>Trichy, Tamil Nadu &nbsp;·&nbsp; <span>evangelin.sofia24@gmail.com</span></p>
</footer>

</body>
</html>
