DAG-L&D Program
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>DAG — Learning & Development Program 2025–2027</title>
<link href="https://fonts.googleapis.com/css2?family=Lexend+Exa:wght@300;400;700&family=Noto+Serif:ital,wght@0,400;0,700;1,400&family=Overpass+Mono:wght@400;600&display=swap" rel="stylesheet"/>
<style>
:root {
  --gold: #c9a84c;
  --gold-light: #e8c97a;
  --gold-dim: rgba(201,168,76,0.12);
  --red: #c0392b;
  --blue: #1a5276;
  --bg: #f7f4ef;
  --white: #ffffff;
  --ink: #1c1c1c;
  --muted: #7a7165;
  --border: #e0d9cd;
  --surface: #faf8f4;
  --kh-red: #032ea1;
  --kh-blue: #e00025;
}
*{box-sizing:border-box;margin:0;padding:0;}
html{scroll-behavior:smooth;}
body{
  background:var(--bg);
  color:var(--ink);
  font-family:'Noto Serif',serif;
  font-size:15px;
  line-height:1.8;
}

/* ─── COVER ─── */
.cover{
  background: linear-gradient(160deg, #0a0f1e 0%, #0d1b3e 55%, #1a0a08 100%);
  min-height:100vh;
  display:flex;flex-direction:column;
  position:relative;overflow:hidden;
  padding:60px 80px;
}
.cover-grid{
  position:absolute;inset:0;
  background-image:
    linear-gradient(rgba(201,168,76,0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(201,168,76,0.06) 1px, transparent 1px);
  background-size:60px 60px;
}
.cover-glow{
  position:absolute;
  width:700px;height:700px;
  background:radial-gradient(ellipse, rgba(201,168,76,0.15) 0%, transparent 70%);
  top:-100px;right:-100px;
  pointer-events:none;
}
.cover-glow2{
  position:absolute;
  width:400px;height:400px;
  background:radial-gradient(ellipse, rgba(192,57,43,0.12) 0%, transparent 70%);
  bottom:0;left:100px;
  pointer-events:none;
}
.cover-top{
  display:flex;justify-content:space-between;align-items:flex-start;
  position:relative;z-index:2;
  margin-bottom:auto;
}
.dag-badge{
  display:flex;align-items:center;gap:14px;
}
.dag-logo{
  width:56px;height:56px;
  background:var(--gold);
  border-radius:4px;
  display:flex;align-items:center;justify-content:center;
  font-family:'Lexend Exa',sans-serif;
  font-size:18px;font-weight:700;
  color:#0a0f1e;
  letter-spacing:-0.02em;
  flex-shrink:0;
}
.dag-name{
  font-family:'Lexend Exa',sans-serif;
  font-size:13px;font-weight:300;
  color:rgba(255,255,255,0.6);
  letter-spacing:0.15em;
  text-transform:uppercase;
  line-height:1.4;
}
.dag-name strong{color:var(--gold-light);font-weight:400;}
.cover-doc-num{
  font-family:'Overpass Mono',monospace;
  font-size:11px;
  color:rgba(255,255,255,0.3);
  letter-spacing:0.1em;
  text-align:right;
  line-height:1.8;
}
.cover-body{
  position:relative;z-index:2;
  margin-top:auto;
  padding-top:80px;
}
.cover-kicker{
  font-family:'Overpass Mono',monospace;
  font-size:11px;
  letter-spacing:0.25em;
  text-transform:uppercase;
  color:var(--gold);
  margin-bottom:24px;
  display:flex;align-items:center;gap:14px;
}
.cover-kicker::before{content:'';display:block;width:40px;height:1px;background:var(--gold);}
.cover h1{
  font-family:'Lexend Exa',sans-serif;
  font-size:clamp(36px,5vw,68px);
  font-weight:700;
  color:#fff;
  line-height:1.05;
  letter-spacing:-0.02em;
  margin-bottom:8px;
}
.cover h1 span{color:var(--gold-light);}
.cover-subtitle{
  font-size:18px;
  color:rgba(255,255,255,0.5);
  font-style:italic;
  margin-bottom:48px;
  font-family:'Noto Serif',serif;
}
.cover-meta{
  display:flex;gap:48px;flex-wrap:wrap;
  border-top:1px solid rgba(201,168,76,0.2);
  padding-top:32px;
}
.cover-meta-item .label{
  font-family:'Overpass Mono',monospace;
  font-size:10px;letter-spacing:0.15em;
  text-transform:uppercase;
  color:rgba(255,255,255,0.3);
  margin-bottom:4px;
}
.cover-meta-item .value{
  font-family:'Lexend Exa',sans-serif;
  font-size:14px;font-weight:300;
  color:var(--gold-light);
}
.cover-pillars{
  display:flex;gap:12px;flex-wrap:wrap;
  margin-top:40px;
}
.cover-pillar{
  border:1px solid rgba(201,168,76,0.25);
  border-radius:3px;
  padding:6px 16px;
  font-family:'Overpass Mono',monospace;
  font-size:10px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  color:rgba(255,255,255,0.5);
}

/* ─── NAV ─── */
nav{
  background:#0d1b3e;
  position:sticky;top:0;z-index:100;
  display:flex;align-items:center;
  overflow-x:auto;scrollbar-width:none;
  border-bottom:2px solid var(--gold);
  padding:0 40px;
}
nav::-webkit-scrollbar{display:none;}
.nav-brand{
  font-family:'Lexend Exa',sans-serif;
  font-size:13px;font-weight:700;
  color:var(--gold);
  letter-spacing:0.05em;
  padding:14px 24px 14px 0;
  border-right:1px solid rgba(255,255,255,0.1);
  margin-right:16px;
  white-space:nowrap;
  flex-shrink:0;
}
nav a{
  color:rgba(255,255,255,0.5);
  text-decoration:none;
  font-family:'Overpass Mono',monospace;
  font-size:10px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  padding:18px 14px;
  white-space:nowrap;
  border-bottom:2px solid transparent;
  transition:all 0.2s;
  margin-bottom:-2px;
}
nav a:hover{color:var(--gold-light);border-bottom-color:var(--gold);}

/* ─── PAGE LAYOUT ─── */
.page{max-width:1080px;margin:0 auto;padding:80px 60px;}
@media(max-width:700px){.page{padding:40px 20px;}}

/* ─── SECTION HEADER ─── */
.sec-header{
  display:flex;align-items:baseline;gap:20px;
  margin-bottom:40px;
  padding-bottom:20px;
  border-bottom:1px solid var(--border);
}
.sec-num{
  font-family:'Overpass Mono',monospace;
  font-size:11px;color:var(--muted);
  letter-spacing:0.1em;flex-shrink:0;
}
.sec-title{
  font-family:'Lexend Exa',sans-serif;
  font-size:28px;font-weight:700;
  color:#0d1b3e;
  letter-spacing:-0.01em;
}
.sec-tag{
  font-family:'Overpass Mono',monospace;
  font-size:10px;letter-spacing:0.12em;
  text-transform:uppercase;
  padding:3px 12px;border-radius:2px;
  margin-left:auto;flex-shrink:0;
}
.tag-gold{background:rgba(201,168,76,0.15);color:var(--gold);}
.tag-blue{background:rgba(26,82,118,0.12);color:var(--blue);}
.tag-red{background:rgba(192,57,43,0.1);color:var(--red);}
.tag-green{background:rgba(39,174,96,0.1);color:#27ae60;}

/* ─── PROSE ─── */
.prose{font-size:15px;line-height:1.85;color:#2c2c2c;margin-bottom:20px;}
.prose strong{color:var(--ink);font-weight:700;}

/* ─── VISION BOX ─── */
.vision-box{
  background:linear-gradient(135deg,#0d1b3e,#1a0a08);
  border-radius:8px;
  padding:48px 52px;
  margin:32px 0;
  position:relative;overflow:hidden;
}
.vision-box::before{
  content:'"';
  position:absolute;top:-20px;left:32px;
  font-size:200px;color:rgba(201,168,76,0.08);
  font-family:'Noto Serif',serif;
  line-height:1;
}
.vision-box p{
  font-size:22px;font-style:italic;
  color:#fff;line-height:1.6;
  position:relative;z-index:1;
  font-family:'Noto Serif',serif;
}
.vision-box .attrib{
  font-style:normal;font-size:12px;
  color:var(--gold);font-family:'Overpass Mono',monospace;
  letter-spacing:0.1em;text-transform:uppercase;
  margin-top:20px;
}

/* ─── PILLAR CARDS ─── */
.pillar-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:16px;margin:24px 0;}
.pillar-card{
  border:1px solid var(--border);
  border-radius:6px;
  padding:28px 24px;
  background:var(--white);
  position:relative;
  transition:box-shadow 0.2s,transform 0.2s;
}
.pillar-card:hover{box-shadow:0 8px 32px rgba(0,0,0,0.08);transform:translateY(-3px);}
.pillar-card::before{
  content:'';
  position:absolute;top:0;left:0;right:0;
  height:4px;border-radius:6px 6px 0 0;
}
.pc-gold::before{background:var(--gold);}
.pc-blue::before{background:var(--blue);}
.pc-red::before{background:var(--red);}
.pc-green::before{background:#27ae60;}
.pc-teal::before{background:#16a085;}
.pc-purple::before{background:#8e44ad;}
.pillar-icon{font-size:28px;margin-bottom:14px;}
.pillar-card h3{
  font-family:'Lexend Exa',sans-serif;
  font-size:13px;font-weight:700;
  letter-spacing:0.04em;
  color:#0d1b3e;margin-bottom:10px;
}
.pillar-card p{font-size:12.5px;color:var(--muted);line-height:1.65;}

/* ─── TRACK TABLE ─── */
.tbl-wrap{overflow-x:auto;border-radius:8px;border:1px solid var(--border);margin:24px 0;}
table{width:100%;border-collapse:collapse;font-size:13px;}
thead{background:#0d1b3e;}
th{
  padding:13px 16px;
  font-family:'Overpass Mono',monospace;
  font-size:10px;letter-spacing:0.12em;
  text-transform:uppercase;
  color:rgba(255,255,255,0.7);
  text-align:left;
  border-bottom:2px solid var(--gold);
}
td{
  padding:12px 16px;
  border-bottom:1px solid var(--border);
  vertical-align:top;
  line-height:1.6;
}
tr:last-child td{border-bottom:none;}
tr:nth-child(even) td{background:var(--surface);}
td.bold{font-weight:700;color:#0d1b3e;}
td.gold{color:var(--gold);font-weight:600;font-family:'Overpass Mono',monospace;}
td.blue{color:var(--blue);}

/* ─── MODULE CARDS ─── */
.module-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:20px;margin:24px 0;}
.module-card{
  background:var(--white);
  border:1px solid var(--border);
  border-radius:8px;
  overflow:hidden;
  transition:box-shadow 0.2s;
}
.module-card:hover{box-shadow:0 6px 24px rgba(0,0,0,0.08);}
.module-card-header{
  padding:18px 20px;
  display:flex;justify-content:space-between;align-items:center;
}
.mch-gold{background:#0d1b3e;}
.mch-blue{background:#1a5276;}
.mch-red{background:#922b21;}
.mch-green{background:#1e8449;}
.module-card-header h4{
  font-family:'Lexend Exa',sans-serif;
  font-size:12px;font-weight:700;
  color:#fff;letter-spacing:0.04em;
}
.module-badge{
  font-family:'Overpass Mono',monospace;
  font-size:10px;
  background:rgba(255,255,255,0.15);
  color:#fff;
  padding:3px 10px;border-radius:100px;
  letter-spacing:0.06em;
}
.module-card-body{padding:20px;}
.module-card-body ul{padding-left:16px;}
.module-card-body li{font-size:13px;color:var(--muted);margin-bottom:5px;line-height:1.5;}
.module-card-body .duration{
  font-family:'Overpass Mono',monospace;font-size:11px;
  color:var(--gold);margin-top:14px;
  border-top:1px solid var(--border);padding-top:10px;
}

/* ─── TIMELINE ─── */
.timeline{margin:32px 0;position:relative;}
.timeline::before{
  content:'';position:absolute;left:28px;top:0;bottom:0;
  width:2px;background:linear-gradient(to bottom,var(--gold),rgba(201,168,76,0.1));
}
.tl-item{display:flex;gap:24px;margin-bottom:32px;position:relative;}
.tl-dot{
  width:56px;height:56px;flex-shrink:0;
  background:#0d1b3e;border:2px solid var(--gold);
  border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  font-family:'Overpass Mono',monospace;font-size:11px;
  color:var(--gold);font-weight:600;
  letter-spacing:0.04em;z-index:1;
}
.tl-content{
  background:var(--white);border:1px solid var(--border);
  border-radius:8px;padding:24px 28px;flex:1;
}
.tl-content h4{
  font-family:'Lexend Exa',sans-serif;font-size:15px;font-weight:700;
  color:#0d1b3e;margin-bottom:8px;
}
.tl-content .phase-tag{
  font-family:'Overpass Mono',monospace;font-size:10px;
  color:var(--gold);letter-spacing:0.1em;text-transform:uppercase;
  margin-bottom:10px;display:block;
}
.tl-content p{font-size:13.5px;color:var(--muted);line-height:1.7;}
.tl-content ul{padding-left:16px;margin-top:8px;}
.tl-content li{font-size:13px;color:var(--muted);margin-bottom:4px;}

/* ─── INFO BOX ─── */
.info-box{
  border-radius:6px;padding:20px 24px;margin:20px 0;
  border-left:4px solid;font-size:13.5px;line-height:1.75;
}
.ib-gold{border-color:var(--gold);background:rgba(201,168,76,0.06);}
.ib-blue{border-color:var(--blue);background:rgba(26,82,118,0.05);}
.ib-red{border-color:var(--red);background:rgba(192,57,43,0.05);}
.ib-green{border-color:#27ae60;background:rgba(39,174,96,0.05);}
.info-box h4{
  font-family:'Lexend Exa',sans-serif;font-size:12px;font-weight:700;
  letter-spacing:0.06em;text-transform:uppercase;margin-bottom:8px;
}
.ib-gold h4{color:var(--gold);}
.ib-blue h4{color:var(--blue);}
.ib-red h4{color:var(--red);}
.ib-green h4{color:#27ae60;}

/* ─── FRAMEWORK BOX ─── */
.framework{
  display:grid;grid-template-columns:repeat(3,1fr);gap:1px;
  background:var(--border);border-radius:8px;overflow:hidden;
  border:1px solid var(--border);margin:24px 0;
}
.fw-cell{
  background:var(--white);padding:24px 20px;
  text-align:center;
}
.fw-cell.header{
  background:#0d1b3e;
  font-family:'Lexend Exa',sans-serif;
  font-size:12px;font-weight:700;
  color:var(--gold-light);letter-spacing:0.08em;
  text-transform:uppercase;padding:14px;
}
.fw-cell .fw-num{
  font-family:'Lexend Exa',sans-serif;font-size:32px;font-weight:700;
  color:var(--gold);line-height:1;margin-bottom:8px;
}
.fw-cell .fw-label{font-size:12px;color:var(--muted);line-height:1.5;}
.fw-cell .fw-title{font-family:'Lexend Exa',sans-serif;font-size:13px;font-weight:700;color:#0d1b3e;margin-bottom:6px;}

/* ─── BUDGET TABLE ─── */
.budget-row{
  display:grid;grid-template-columns:1fr auto auto;gap:0;
  padding:12px 20px;border-bottom:1px solid var(--border);
  align-items:center;font-size:13.5px;
}
.budget-row:last-child{border-bottom:none;}
.budget-row.header{
  background:#0d1b3e;color:var(--gold-light);
  font-family:'Overpass Mono',monospace;font-size:10px;
  letter-spacing:0.1em;text-transform:uppercase;padding:10px 20px;
}
.budget-row.total{
  background:rgba(201,168,76,0.08);
  font-family:'Lexend Exa',sans-serif;font-weight:700;
  font-size:14px;color:#0d1b3e;
}
.budget-amount{
  font-family:'Overpass Mono',monospace;font-size:13px;
  text-align:right;padding-left:32px;color:#0d1b3e;
}
.budget-pct{
  font-family:'Overpass Mono',monospace;font-size:11px;
  color:var(--muted);text-align:right;padding-left:20px;
  width:60px;
}

/* ─── KPI GRID ─── */
.kpi-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(180px,1fr));gap:16px;margin:24px 0;}
.kpi-card{
  background:var(--white);border:1px solid var(--border);
  border-radius:8px;padding:24px 20px;text-align:center;
}
.kpi-num{
  font-family:'Lexend Exa',sans-serif;font-size:36px;font-weight:700;
  color:#0d1b3e;line-height:1;margin-bottom:8px;
}
.kpi-num span{font-size:20px;color:var(--gold);}
.kpi-label{font-size:12px;color:var(--muted);line-height:1.5;}

/* ─── DIVIDER ─── */
hr{border:none;border-top:1px solid var(--border);margin:60px 0;}

/* ─── SECTION BREAK ─── */
.section{padding:80px 0;border-bottom:1px solid var(--border);}
.section:last-child{border-bottom:none;}

/* ─── FOOTER ─── */
footer{
  background:#0d1b3e;
  padding:48px 60px;
  display:flex;justify-content:space-between;align-items:center;
  flex-wrap:wrap;gap:20px;
}
footer .f-brand{
  font-family:'Lexend Exa',sans-serif;font-size:16px;font-weight:700;
  color:var(--gold);
}
footer p{font-size:12px;color:rgba(255,255,255,0.3);font-family:'Overpass Mono',monospace;letter-spacing:0.06em;}

/* ─── ACCORDION ─── */
.accordion{margin:24px 0;}
.acc-item{border:1px solid var(--border);border-radius:6px;margin-bottom:8px;overflow:hidden;}
.acc-header{
  display:flex;justify-content:space-between;align-items:center;
  padding:16px 20px;cursor:pointer;background:var(--white);
  transition:background 0.2s;
}
.acc-header:hover{background:var(--surface);}
.acc-header h4{font-family:'Lexend Exa',sans-serif;font-size:13px;font-weight:700;color:#0d1b3e;}
.acc-arrow{color:var(--gold);font-size:18px;transition:transform 0.3s;flex-shrink:0;}
.acc-body{display:none;padding:0 20px 20px;font-size:13.5px;color:var(--muted);line-height:1.75;}
.acc-body ul{padding-left:16px;margin-top:8px;}
.acc-body li{margin-bottom:6px;}
.acc-item.open .acc-arrow{transform:rotate(180deg);}
.acc-item.open .acc-body{display:block;}
</style>
</head>
<body>

<!-- ══════════════════════ COVER ══════════════════════ -->
<div class="cover">
  <div class="cover-grid"></div>
  <div class="cover-glow"></div>
  <div class="cover-glow2"></div>
  <div class="cover-top">
    <div class="dag-badge">
      <div class="dag-logo">DAG</div>
      <div class="dag-name"><strong>Dynamic Advanced Group</strong><br/>Kingdom of Cambodia</div>
    </div>
    <div class="cover-doc-num">
      Document: DAG-HRD-L&D-2025<br/>
      Classification: Internal<br/>
      Version: 1.0 | 2025–2027
    </div>
  </div>
  <div class="cover-body">
    <div class="cover-kicker">Human Capital Development</div>
    <h1>Learning &<br/><span>Development</span><br/>Program</h1>
    <div class="cover-subtitle">Building Excellence Across Every Level of the Group</div>
    <div class="cover-meta">
      <div class="cover-meta-item">
        <div class="label">Program Period</div>
        <div class="value">2025 – 2027</div>
      </div>
      <div class="cover-meta-item">
        <div class="label">Scope</div>
        <div class="value">All Business Units</div>
      </div>
      <div class="cover-meta-item">
        <div class="label">Audience</div>
        <div class="value">All Employees</div>
      </div>
      <div class="cover-meta-item">
        <div class="label">Issued by</div>
        <div class="value">Group HR & Talent</div>
      </div>
    </div>
    <div class="cover-pillars">
      <span class="cover-pillar">Functional Excellence</span>
      <span class="cover-pillar">Leadership Pipeline</span>
      <span class="cover-pillar">Digital Capability</span>
      <span class="cover-pillar">Culture & Values</span>
      <span class="cover-pillar">Compliance & Ethics</span>
      <span class="cover-pillar">Talent Acceleration</span>
    </div>
  </div>
</div>

<!-- ══════════════════════ NAV ══════════════════════ -->
<nav>
  <div class="nav-brand">DAG L&D</div>
  <a href="#overview">Overview</a>
  <a href="#framework">Framework</a>
  <a href="#tracks">Tracks</a>
  <a href="#modules">Modules</a>
  <a href="#roadmap">Roadmap</a>
  <a href="#delivery">Delivery</a>
  <a href="#kpis">KPIs</a>
  <a href="#budget">Budget</a>
  <a href="#governance">Governance</a>
</nav>

<!-- ══════════════════════ OVERVIEW ══════════════════════ -->
<div id="overview" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">01</span>
    <h2 class="sec-title">Executive Overview</h2>
    <span class="sec-tag tag-gold">Foundation</span>
  </div>

  <p class="prose">Dynamic Advanced Group (DAG) is a diversified Cambodian conglomerate with operations spanning multiple sectors. As DAG accelerates its growth strategy across Cambodia and the region, the quality, capability, and leadership depth of its people is the single most important competitive differentiator.</p>
  <p class="prose">This <strong>Learning & Development (L&D) Program 2025–2027</strong> establishes a unified, structured framework for building human capital across all business units. It is designed to elevate performance at every level — from frontline staff to senior executives — while building a strong Cambodian leadership pipeline aligned with DAG's vision.</p>

  <div class="vision-box">
    <p>To build a world-class workforce rooted in Cambodian excellence — where every employee at Dynamic Advanced Group is empowered to grow, lead, and drive the Group's mission forward.</p>
    <div class="attrib">— DAG L&D Program Vision, 2025–2027</div>
  </div>

  <div class="pillar-grid">
    <div class="pillar-card pc-gold">
      <div class="pillar-icon">🎯</div>
      <h3>Strategic Alignment</h3>
      <p>Every learning initiative is tied directly to DAG's 3-year business strategy and group-level KPIs.</p>
    </div>
    <div class="pillar-card pc-blue">
      <div class="pillar-icon">🏗️</div>
      <h3>Structured Tracks</h3>
      <p>Role-based learning tracks ensure relevance — from fresh graduates to C-suite leaders.</p>
    </div>
    <div class="pillar-card pc-red">
      <div class="pillar-icon">🌏</div>
      <h3>Cambodia-First</h3>
      <p>Programs are designed for the Cambodian context, with bilingual delivery (Khmer & English).</p>
    </div>
    <div class="pillar-card pc-green">
      <div class="pillar-icon">📊</div>
      <h3>Measurable Impact</h3>
      <p>All programs use Kirkpatrick's 4-level model to evaluate effectiveness and business impact.</p>
    </div>
    <div class="pillar-card pc-teal">
      <div class="pillar-icon">💡</div>
      <h3>Blended Learning</h3>
      <p>In-person workshops, digital modules, on-the-job learning, and mentoring — combined.</p>
    </div>
    <div class="pillar-card pc-purple">
      <div class="pillar-icon">🚀</div>
      <h3>Talent Acceleration</h3>
      <p>Fast-track programs identify and develop high-potential talent for critical Group roles.</p>
    </div>
  </div>
</div>
</div>

<!-- ══════════════════════ FRAMEWORK ══════════════════════ -->
<div id="framework" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">02</span>
    <h2 class="sec-title">L&D Framework</h2>
    <span class="sec-tag tag-blue">Architecture</span>
  </div>

  <p class="prose">The DAG L&D Framework is built on three interconnected pillars: <strong>Capability Building</strong> (what people know and can do), <strong>Leadership Development</strong> (how people lead and decide), and <strong>Culture & Values</strong> (who we are as an organization). All three work together to drive performance.</p>

  <div class="framework">
    <div class="fw-cell header">Capability Building</div>
    <div class="fw-cell header">Leadership Development</div>
    <div class="fw-cell header">Culture & Values</div>
    <div class="fw-cell">
      <div class="fw-num">01</div>
      <div class="fw-title">Functional Skills</div>
      <div class="fw-label">Technical expertise specific to each business unit and role</div>
    </div>
    <div class="fw-cell">
      <div class="fw-num">02</div>
      <div class="fw-title">Leadership Pipeline</div>
      <div class="fw-label">Tiered leadership programs from supervisor to Group executive</div>
    </div>
    <div class="fw-cell">
      <div class="fw-num">03</div>
      <div class="fw-title">DAG Way</div>
      <div class="fw-label">Group values, ethics, culture, and Cambodian identity</div>
    </div>
    <div class="fw-cell">
      <div class="fw-num">04</div>
      <div class="fw-title">Digital Literacy</div>
      <div class="fw-label">Technology, data, and digital tools for all levels</div>
    </div>
    <div class="fw-cell">
      <div class="fw-num">05</div>
      <div class="fw-title">Hi-Po Acceleration</div>
      <div class="fw-label">Fast-track programs for identified high-potential employees</div>
    </div>
    <div class="fw-cell">
      <div class="fw-num">06</div>
      <div class="fw-title">Compliance & Ethics</div>
      <div class="fw-label">Mandatory compliance, governance, and safety training</div>
    </div>
  </div>

  <div class="info-box ib-gold">
    <h4>The 70-20-10 Learning Model</h4>
    <p>DAG's L&D program follows the globally proven 70-20-10 framework:<br/>
    <strong>70%</strong> — On-the-job experience: stretch assignments, special projects, job rotations<br/>
    <strong>20%</strong> — Social learning: mentoring, coaching, peer learning, action learning sets<br/>
    <strong>10%</strong> — Formal training: workshops, e-learning, certifications, external programs</p>
  </div>
</div>
</div>

<!-- ══════════════════════ TRACKS ══════════════════════ -->
<div id="tracks" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">03</span>
    <h2 class="sec-title">Learning Tracks by Employee Level</h2>
    <span class="sec-tag tag-blue">Structure</span>
  </div>

  <p class="prose">DAG's L&D program is organized into five distinct learning tracks aligned to career levels. Each track has tailored content, delivery modes, and time commitments — ensuring learning is always relevant and applicable.</p>

  <div class="tbl-wrap">
    <table>
      <thead>
        <tr>
          <th>Track</th>
          <th>Target Group</th>
          <th>Focus Areas</th>
          <th>Hours / Year</th>
          <th>Key Outcome</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="bold">Track 1 — Onboarding & Foundation</td>
          <td>New hires, fresh graduates</td>
          <td>DAG culture, systems, functional basics, compliance</td>
          <td class="gold">80 hrs</td>
          <td>Productive contributor within 90 days</td>
        </tr>
        <tr>
          <td class="bold">Track 2 — Individual Contributor Excellence</td>
          <td>Staff, Officers, Executives</td>
          <td>Functional skills, digital tools, communication, productivity</td>
          <td class="gold">40 hrs</td>
          <td>High performance in current role</td>
        </tr>
        <tr>
          <td class="bold">Track 3 — Emerging Leaders</td>
          <td>Senior officers, Supervisors, Team leads</td>
          <td>People management, project leadership, problem solving</td>
          <td class="gold">50 hrs</td>
          <td>Ready for first management role</td>
        </tr>
        <tr>
          <td class="bold">Track 4 — Mid-Level Management</td>
          <td>Managers, Senior Managers, HODs</td>
          <td>Strategic thinking, business acumen, cross-function leadership</td>
          <td class="gold">60 hrs</td>
          <td>Effective cross-functional leader</td>
        </tr>
        <tr>
          <td class="bold">Track 5 — Senior Leadership</td>
          <td>Directors, GMs, C-Suite, BU Heads</td>
          <td>Group strategy, governance, executive presence, innovation</td>
          <td class="gold">70 hrs</td>
          <td>Drives Group-level growth and transformation</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="info-box ib-blue">
    <h4>High-Potential (Hi-Po) Acceleration Track</h4>
    <p>A select cohort of high-potential employees (top 10–15% identified through performance review and talent calibration) will be enrolled in the <strong>DAG Talent Acceleration Program (DAG-TAP)</strong> — a cross-functional, cross-track program involving executive mentoring, stretch projects, external benchmarking, and leadership exposure over 18 months.</p>
  </div>
</div>
</div>

<!-- ══════════════════════ MODULES ══════════════════════ -->
<div id="modules" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">04</span>
    <h2 class="sec-title">Core Learning Modules</h2>
    <span class="sec-tag tag-gold">Content</span>
  </div>

  <p class="prose">The following modules form the core curriculum of the DAG L&D program. Modules are delivered as standalone workshops, blended programs, or digital self-paced courses depending on content type and audience.</p>

  <h3 style="font-family:'Lexend Exa',sans-serif;font-size:16px;color:#0d1b3e;margin:32px 0 16px;">🧭 Culture, Onboarding & Compliance</h3>
  <div class="module-grid">
    <div class="module-card">
      <div class="module-card-header mch-gold">
        <h4>DAG Orientation & Culture</h4>
        <span class="module-badge">All Staff</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>DAG history, vision, values, and group structure</li>
          <li>Business units overview and synergies</li>
          <li>HR policies, benefits, and expectations</li>
          <li>Workplace code of conduct</li>
        </ul>
        <div class="duration">⏱ 2 days | Classroom + Digital</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-gold">
        <h4>Compliance, Ethics & Anti-Corruption</h4>
        <span class="module-badge">Mandatory</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Cambodia labor law fundamentals</li>
          <li>Anti-corruption and whistleblower policy</li>
          <li>Data privacy and information security</li>
          <li>Health, safety & environment (HSE)</li>
        </ul>
        <div class="duration">⏱ 1 day + Annual e-learning | Digital</div>
      </div>
    </div>
  </div>

  <h3 style="font-family:'Lexend Exa',sans-serif;font-size:16px;color:#0d1b3e;margin:32px 0 16px;">⚙️ Functional & Technical Skills</h3>
  <div class="module-grid">
    <div class="module-card">
      <div class="module-card-header mch-blue">
        <h4>Finance for Non-Finance Managers</h4>
        <span class="module-badge">Track 3–4</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Reading financial statements</li>
          <li>Budgeting and cost management</li>
          <li>Financial KPIs and business performance</li>
          <li>Capex vs. Opex decision making</li>
        </ul>
        <div class="duration">⏱ 3 days | Classroom + Case studies</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-blue">
        <h4>Sales, Negotiation & CRM</h4>
        <span class="module-badge">Track 2–3</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Consultative selling techniques</li>
          <li>Negotiation strategies and closing</li>
          <li>Customer relationship management</li>
          <li>Key account management</li>
        </ul>
        <div class="duration">⏱ 2 days | Workshop + Role-play</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-blue">
        <h4>Project Management Essentials</h4>
        <span class="module-badge">Track 2–4</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Project planning, scope and scheduling</li>
          <li>Risk management and issue escalation</li>
          <li>Stakeholder communication</li>
          <li>Agile and traditional PM methodologies</li>
        </ul>
        <div class="duration">⏱ 3 days | Blended</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-blue">
        <h4>Digital Skills & Productivity Tools</h4>
        <span class="module-badge">All Staff</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Excel, PowerPoint, and data tools (advanced)</li>
          <li>ERP and business system navigation</li>
          <li>AI tools and productivity automation</li>
          <li>Cybersecurity awareness</li>
        </ul>
        <div class="duration">⏱ 2 days | Digital + Lab</div>
      </div>
    </div>
  </div>

  <h3 style="font-family:'Lexend Exa',sans-serif;font-size:16px;color:#0d1b3e;margin:32px 0 16px;">👥 Leadership & People Development</h3>
  <div class="module-grid">
    <div class="module-card">
      <div class="module-card-header mch-red">
        <h4>Supervisory & Team Leadership</h4>
        <span class="module-badge">Track 3</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Role of a first-time manager</li>
          <li>Goal setting and performance management</li>
          <li>Giving effective feedback and coaching</li>
          <li>Conflict resolution and team dynamics</li>
        </ul>
        <div class="duration">⏱ 4 days | Workshop over 2 months</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-red">
        <h4>Strategic Leadership for Managers</h4>
        <span class="module-badge">Track 4</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Business strategy and competitive analysis</li>
          <li>Cross-functional leadership</li>
          <li>Change management and organizational agility</li>
          <li>Influencing without authority</li>
        </ul>
        <div class="duration">⏱ 5 days | Modular program (3 months)</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-red">
        <h4>Executive Leadership Program</h4>
        <span class="module-badge">Track 5</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Group governance and board dynamics</li>
          <li>Leading enterprise transformation</li>
          <li>Executive communication and stakeholder management</li>
          <li>Succession planning and talent stewardship</li>
        </ul>
        <div class="duration">⏱ 6 days | Residential + Coaching</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-red">
        <h4>Coaching & Mentoring Skills</h4>
        <span class="module-badge">Track 3–5</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>GROW coaching model</li>
          <li>Active listening and powerful questions</li>
          <li>Mentoring relationships and structure</li>
          <li>Developing others as a strategic habit</li>
        </ul>
        <div class="duration">⏱ 2 days | Workshop + Practice pairs</div>
      </div>
    </div>
  </div>

  <h3 style="font-family:'Lexend Exa',sans-serif;font-size:16px;color:#0d1b3e;margin:32px 0 16px;">🌐 Professional & Soft Skills</h3>
  <div class="module-grid">
    <div class="module-card">
      <div class="module-card-header mch-green">
        <h4>Business Communication & Presentation</h4>
        <span class="module-badge">Track 2–4</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Professional writing (email, reports, proposals)</li>
          <li>Presentation structure and storytelling</li>
          <li>Executive-level communication</li>
          <li>Bilingual business communication (Khmer/English)</li>
        </ul>
        <div class="duration">⏱ 2 days | Workshop + Practice</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-green">
        <h4>Critical Thinking & Problem Solving</h4>
        <span class="module-badge">Track 2–4</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Structured problem-solving frameworks (MECE, 5-Why, fishbone)</li>
          <li>Data-driven decision making</li>
          <li>Creative and design thinking</li>
          <li>Business case development</li>
        </ul>
        <div class="duration">⏱ 2 days | Workshop + Case studies</div>
      </div>
    </div>
    <div class="module-card">
      <div class="module-card-header mch-green">
        <h4>Emotional Intelligence & Resilience</h4>
        <span class="module-badge">All Levels</span>
      </div>
      <div class="module-card-body">
        <ul>
          <li>Self-awareness and self-regulation</li>
          <li>Empathy, social skills, and motivation</li>
          <li>Managing stress and workplace resilience</li>
          <li>Mental wellness at work</li>
        </ul>
        <div class="duration">⏱ 1 day | Workshop + Reflection</div>
      </div>
    </div>
  </div>
</div>
</div>

<!-- ══════════════════════ ROADMAP ══════════════════════ -->
<div id="roadmap" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">05</span>
    <h2 class="sec-title">3-Year Implementation Roadmap</h2>
    <span class="sec-tag tag-red">Execution</span>
  </div>

  <div class="timeline">
    <div class="tl-item">
      <div class="tl-dot">2025<br/>Q1–Q2</div>
      <div class="tl-content">
        <span class="phase-tag">Phase 1 — Foundation</span>
        <h4>Build the Infrastructure</h4>
        <p>Establish the L&D function, systems, and baseline programs.</p>
        <ul>
          <li>Appoint Group L&D Manager and BU L&D Coordinators</li>
          <li>Conduct Training Needs Analysis (TNA) across all BUs</li>
          <li>Design and launch the DAG Learning Management System (LMS)</li>
          <li>Develop and roll out Onboarding & Compliance programs (all staff)</li>
          <li>Launch Track 1 Foundation modules for all new hires</li>
          <li>Establish mentoring pilot program (Track 5 mentors → Track 3 mentees)</li>
        </ul>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot">2025<br/>Q3–Q4</div>
      <div class="tl-content">
        <span class="phase-tag">Phase 2 — Core Rollout</span>
        <h4>Launch Core Curriculum Across Tracks</h4>
        <ul>
          <li>Roll out Track 2 & 3 programs (Individual Contributors & Emerging Leaders)</li>
          <li>Launch first cohort of DAG Talent Acceleration Program (DAG-TAP)</li>
          <li>Deliver Digital Skills program group-wide</li>
          <li>Begin bi-annual performance–learning integration (link IDP to L&D calendar)</li>
          <li>Establish external partnerships: local universities, regional training providers</li>
        </ul>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot">2026<br/>Q1–Q2</div>
      <div class="tl-content">
        <span class="phase-tag">Phase 3 — Leadership & Management Development</span>
        <h4>Build the Leadership Pipeline</h4>
        <ul>
          <li>Launch Track 4 Strategic Leadership Program (Managers & HODs)</li>
          <li>Deliver Executive Leadership Program for Track 5 (Directors, GMs)</li>
          <li>Introduce 360-degree feedback for all management levels</li>
          <li>Implement job rotation program across BUs for Hi-Po cohort</li>
          <li>First DAG-TAP cohort graduation and placement</li>
        </ul>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot">2026<br/>Q3–Q4</div>
      <div class="tl-content">
        <span class="phase-tag">Phase 4 — Optimize & Scale</span>
        <h4>Measure, Refine and Scale</h4>
        <ul>
          <li>Full Kirkpatrick Level 3 & 4 evaluation of all programs</li>
          <li>Launch second cohort of DAG-TAP with refined curriculum</li>
          <li>Introduce internal faculty program (senior leaders as trainers)</li>
          <li>Expand digital content library on LMS</li>
          <li>Benchmark DAG L&D against regional group company best practices</li>
        </ul>
      </div>
    </div>
    <div class="tl-item">
      <div class="tl-dot">2027</div>
      <div class="tl-content">
        <span class="phase-tag">Phase 5 — Sustainability & Excellence</span>
        <h4>Institutionalize Learning Culture</h4>
        <ul>
          <li>Launch DAG Learning Academy — a branded internal learning institution</li>
          <li>Develop DAG-branded certifications recognized across BUs</li>
          <li>Implement succession planning integrated with L&D outcomes</li>
          <li>Target 90%+ of management roles filled internally</li>
          <li>Evaluate ROI of 3-year L&D investment against business outcomes</li>
        </ul>
      </div>
    </div>
  </div>
</div>
</div>

<!-- ══════════════════════ DELIVERY ══════════════════════ -->
<div id="delivery" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">06</span>
    <h2 class="sec-title">Delivery Methods & Learning Experience</h2>
    <span class="sec-tag tag-blue">Approach</span>
  </div>

  <div class="accordion">
    <div class="acc-item open">
      <div class="acc-header" onclick="toggle(this)">
        <h4>🏫 Classroom & Workshop-Based Learning</h4>
        <span class="acc-arrow">▾</span>
      </div>
      <div class="acc-body">
        <p>Instructor-led training (ILT) remains a core delivery method for complex, interpersonal, and leadership topics. DAG workshops are facilitated in Khmer and English, using experiential methods:</p>
        <ul>
          <li>Case studies from Cambodia and ASEAN business contexts</li>
          <li>Role-play, simulation, and group exercises</li>
          <li>Guest speakers from industry and academia</li>
          <li>Action learning sets (post-workshop peer groups)</li>
        </ul>
      </div>
    </div>
    <div class="acc-item">
      <div class="acc-header" onclick="toggle(this)">
        <h4>💻 Digital & E-Learning (LMS)</h4>
        <span class="acc-arrow">▾</span>
      </div>
      <div class="acc-body">
        <p>DAG will deploy a Learning Management System (LMS) to deliver and track digital learning across all BUs. The LMS will host:</p>
        <ul>
          <li>Mandatory compliance e-learning modules (annual certification)</li>
          <li>Short-form microlearning videos (5–15 minutes) for on-demand learning</li>
          <li>Pre-work and post-workshop reinforcement materials</li>
          <li>Learning progress dashboards for employees and managers</li>
          <li>External content subscriptions (LinkedIn Learning, Coursera for Business)</li>
        </ul>
      </div>
    </div>
    <div class="acc-item">
      <div class="acc-header" onclick="toggle(this)">
        <h4>🤝 Mentoring & Coaching Programs</h4>
        <span class="acc-arrow">▾</span>
      </div>
      <div class="acc-body">
        <p>Structured mentoring is one of the highest-impact development tools. DAG will implement a formal Group Mentoring Program:</p>
        <ul>
          <li>Senior leaders (Track 5) paired with emerging talents (Track 3)</li>
          <li>Monthly structured mentoring sessions with guided conversation frameworks</li>
          <li>External executive coaching for Directors and GMs (quarterly)</li>
          <li>Peer coaching circles for mid-management cohorts</li>
          <li>Dedicated HR Business Partner coaching support</li>
        </ul>
      </div>
    </div>
    <div class="acc-item">
      <div class="acc-header" onclick="toggle(this)">
        <h4>🔄 On-the-Job Learning & Stretch Assignments</h4>
        <span class="acc-arrow">▾</span>
      </div>
      <div class="acc-body">
        <p>The most powerful development happens on the job. DAG formalizes OJL through:</p>
        <ul>
          <li>Stretch assignments: cross-BU projects beyond current job scope</li>
          <li>Job shadowing and cross-functional exposure visits</li>
          <li>Secondments to other business units (3–6 months for Hi-Po)</li>
          <li>Project leadership opportunities for emerging managers</li>
          <li>Structured reflection and debrief with line manager after each assignment</li>
        </ul>
      </div>
    </div>
    <div class="acc-item">
      <div class="acc-header" onclick="toggle(this)">
        <h4>🌐 External Programs & Certifications</h4>
        <span class="acc-arrow">▾</span>
      </div>
      <div class="acc-body">
        <p>Selected employees will access external development for specialized skills or advanced qualifications:</p>
        <ul>
          <li>Professional certifications: CPA, CMA, PMP, SHRM, CIPS, CFA</li>
          <li>MBA / Executive MBA sponsorship for senior talent (bond agreement)</li>
          <li>ASEAN and international leadership programs (Singapore, Thailand)</li>
          <li>Industry conferences and professional association memberships</li>
          <li>Government and ASEAN training partnerships (ILO, ADB, GIZ)</li>
        </ul>
      </div>
    </div>
  </div>

  <div class="info-box ib-green">
    <h4>Individual Development Plan (IDP)</h4>
    <p>Every employee completes an <strong>Individual Development Plan</strong> annually, co-created with their line manager during the performance appraisal cycle. The IDP maps current competency gaps to specific learning interventions — formal training, OJL, mentoring, or external programs — with timelines, resources, and success measures. IDPs are reviewed mid-year and tracked on the LMS.</p>
  </div>
</div>
</div>

<!-- ══════════════════════ KPIs ══════════════════════ -->
<div id="kpis" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">07</span>
    <h2 class="sec-title">Measurement & KPIs</h2>
    <span class="sec-tag tag-gold">Impact</span>
  </div>

  <p class="prose">DAG evaluates L&D effectiveness using <strong>Kirkpatrick's Four-Level Model</strong> — measuring reaction, learning, behavior change, and business results. The following KPIs will be tracked quarterly and reported to Group HR leadership and the Board.</p>

  <div class="kpi-grid">
    <div class="kpi-card">
      <div class="kpi-num">40<span>hrs</span></div>
      <div class="kpi-label">Minimum training hours per employee per year</div>
    </div>
    <div class="kpi-card">
      <div class="kpi-num">85<span>%</span></div>
      <div class="kpi-label">Target post-training satisfaction score</div>
    </div>
    <div class="kpi-card">
      <div class="kpi-num">90<span>%</span></div>
      <div class="kpi-label">IDP completion rate across all staff</div>
    </div>
    <div class="kpi-card">
      <div class="kpi-num">70<span>%</span></div>
      <div class="kpi-label">Management roles filled internally by 2027</div>
    </div>
    <div class="kpi-card">
      <div class="kpi-num">100<span>%</span></div>
      <div class="kpi-label">Compliance training completion (mandatory)</div>
    </div>
    <div class="kpi-card">
      <div class="kpi-num">20<span>%</span></div>
      <div class="kpi-label">Reduction in time-to-productivity for new hires</div>
    </div>
  </div>

  <div class="tbl-wrap">
    <table>
      <thead>
        <tr><th>Kirkpatrick Level</th><th>Measurement Method</th><th>Frequency</th><th>Owner</th></tr>
      </thead>
      <tbody>
        <tr>
          <td class="bold">Level 1 — Reaction</td>
          <td>Post-training feedback survey (digital, 5-point scale)</td>
          <td>Every program</td>
          <td class="blue">L&D Team</td>
        </tr>
        <tr>
          <td class="bold">Level 2 — Learning</td>
          <td>Pre/post knowledge assessments, skill demonstrations</td>
          <td>Every program</td>
          <td class="blue">L&D Team + Facilitator</td>
        </tr>
        <tr>
          <td class="bold">Level 3 — Behavior</td>
          <td>360° feedback, manager observation, IDP progress review</td>
          <td>3 & 6 months post-training</td>
          <td class="blue">HRBP + Line Manager</td>
        </tr>
        <tr>
          <td class="bold">Level 4 — Results</td>
          <td>Business KPIs, productivity, retention, internal promotion rate</td>
          <td>Annual</td>
          <td class="blue">Group CHRO + CFO</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>
</div>

<!-- ══════════════════════ BUDGET ══════════════════════ -->
<div id="budget" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">08</span>
    <h2 class="sec-title">Budget & Resource Allocation</h2>
    <span class="sec-tag tag-red">Investment</span>
  </div>

  <p class="prose">DAG commits a dedicated annual L&D budget aligned to industry benchmarks of <strong>1.5–2.5% of total payroll</strong>. The budget is allocated across five categories to ensure balanced investment across all development priorities.</p>

  <div style="border:1px solid var(--border);border-radius:8px;overflow:hidden;margin:24px 0;">
    <div class="budget-row header">
      <span>Budget Category</span>
      <span style="text-align:right">Annual (USD)</span>
      <span style="text-align:right">%</span>
    </div>
    <div class="budget-row">
      <span>Internal Training Delivery (facilitation, materials, venues)</span>
      <span class="budget-amount">$45,000</span>
      <span class="budget-pct">30%</span>
    </div>
    <div class="budget-row">
      <span>External Programs & Certifications</span>
      <span class="budget-amount">$30,000</span>
      <span class="budget-pct">20%</span>
    </div>
    <div class="budget-row">
      <span>LMS Platform & Digital Content</span>
      <span class="budget-amount">$22,500</span>
      <span class="budget-pct">15%</span>
    </div>
    <div class="budget-row">
      <span>Leadership & Executive Development (coaching, residential)</span>
      <span class="budget-amount">$30,000</span>
      <span class="budget-pct">20%</span>
    </div>
    <div class="budget-row">
      <span>L&D Team Capacity & Operations</span>
      <span class="budget-amount">$22,500</span>
      <span class="budget-pct">15%</span>
    </div>
    <div class="budget-row total">
      <span>Total Annual L&D Investment</span>
      <span class="budget-amount" style="color:var(--gold)">$150,000</span>
      <span class="budget-pct" style="color:var(--gold)">100%</span>
    </div>
  </div>

  <div class="info-box ib-gold">
    <h4>Return on Investment Expectation</h4>
    <p>Based on industry studies, every $1 invested in structured employee development yields $4–$6 in productivity gains, reduced turnover, and accelerated business performance. For DAG, the primary ROI metrics are: <strong>internal promotion fill rate</strong>, <strong>employee retention improvement</strong>, <strong>faster time-to-productivity</strong> for new hires, and <strong>measurable competency uplift</strong> aligned to business KPIs.</p>
  </div>
</div>
</div>

<!-- ══════════════════════ GOVERNANCE ══════════════════════ -->
<div id="governance" class="section">
<div class="page">
  <div class="sec-header">
    <span class="sec-num">09</span>
    <h2 class="sec-title">Governance & Roles</h2>
    <span class="sec-tag tag-green">Structure</span>
  </div>

  <div class="tbl-wrap">
    <table>
      <thead>
        <tr><th>Role</th><th>Responsibilities</th></tr>
      </thead>
      <tbody>
        <tr>
          <td class="bold">Group CEO / Board</td>
          <td>Champions learning culture; approves L&D strategy and budget; reviews annual L&D impact report</td>
        </tr>
        <tr>
          <td class="bold">Group CHRO</td>
          <td>Owns L&D strategy; integrates L&D with talent management, succession, and performance systems</td>
        </tr>
        <tr>
          <td class="bold">Group L&D Manager</td>
          <td>Designs and manages the L&D program; vendor management; LMS administration; program evaluation</td>
        </tr>
        <tr>
          <td class="bold">BU HR / L&D Coordinators</td>
          <td>Implement L&D plans within business units; coordinate logistics; track participation and completion</td>
        </tr>
        <tr>
          <td class="bold">Line Managers</td>
          <td>Approve and support employee IDPs; reinforce on-the-job learning; conduct post-training check-ins</td>
        </tr>
        <tr>
          <td class="bold">Employees</td>
          <td>Own their development journey; complete IDP; attend scheduled training; apply learning on the job</td>
        </tr>
        <tr>
          <td class="bold">External Providers</td>
          <td>Deliver specialized training programs; provide certifications; support LMS content</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="info-box ib-blue">
    <h4>L&D Steering Committee</h4>
    <p>A quarterly <strong>L&D Steering Committee</strong> — chaired by the Group CHRO and comprising BU Heads and the Group L&D Manager — reviews program progress, addresses issues, approves curriculum updates, and ensures strategic alignment. Annual results are presented to the Board as part of the Human Capital Report.</p>
  </div>

  <div class="info-box ib-red">
    <h4>Policy: Training Commitment & Bond</h4>
    <p>Employees receiving significant external investment (external certifications, MBA sponsorship, international programs exceeding $3,000) sign a <strong>Training Bond Agreement</strong> committing to remain with DAG for a defined period (typically 1–3 years) proportional to the investment. This protects Group investment while demonstrating commitment to employee growth.</p>
  </div>
</div>
</div>

<!-- ══════════════════════ FOOTER ══════════════════════ -->
<footer>
  <div>
    <div class="f-brand">Dynamic Advanced Group</div>
    <p style="margin-top:6px">Kingdom of Cambodia · Group Human Resources & Talent Development</p>
  </div>
  <div style="text-align:right">
    <p>DAG-HRD-L&D-2025 · Version 1.0</p>
    <p style="margin-top:4px">Learning & Development Program 2025–2027</p>
  </div>
</footer>

<script>
function toggle(header) {
  const item = header.parentElement;
  item.classList.toggle('open');
}
</script>
</body>
</html>
