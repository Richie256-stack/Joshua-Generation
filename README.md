<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Joshua Generation International Network — TJG Profile 2026</title>
<style>
:root{
  --forest:#144d34;
  --forest-dark:#0b2f1f;
  --gold:#e8b430;
  --gold-deep:#c9930f;
  --cream:#f7f2e4;
  --ink:#16241c;
  --paper:#fffdf7;
  --line: rgba(20,77,52,0.16);
  --serif: "Iowan Old Style", "Palatino Linotype", Palatino, Georgia, serif;
  --sans: "Avenir Next", "Segoe UI", system-ui, -apple-system, sans-serif;
  --mono: "JetBrains Mono", "SFMono-Regular", Menlo, monospace;
}
*{box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  margin:0;
  font-family:var(--sans);
  background:var(--cream);
  color:var(--ink);
  -webkit-font-smoothing:antialiased;
}
::selection{background:var(--gold);color:var(--forest-dark);}

/* ---------- Texture backdrop ---------- */
body::before{
  content:"";
  position:fixed;inset:0;
  background-image:
    radial-gradient(circle at 15% 20%, rgba(232,180,48,0.08), transparent 40%),
    radial-gradient(circle at 85% 80%, rgba(20,77,52,0.06), transparent 45%);
  pointer-events:none;
  z-index:0;
}

/* ---------- Top bar ---------- */
header.top{
  position:sticky;top:0;z-index:50;
  background:var(--forest);
  color:var(--cream);
  border-bottom:3px solid var(--gold);
}
.top-inner{
  max-width:1200px;margin:0 auto;
  display:flex;align-items:center;justify-content:space-between;
  padding:14px 24px;gap:20px;
}
.brand{display:flex;align-items:center;gap:12px;cursor:pointer;}
.brand-mark{
  width:38px;height:38px;border-radius:6px;
  background:linear-gradient(160deg,var(--gold),var(--gold-deep));
  display:flex;align-items:center;justify-content:center;
  font-family:var(--serif);font-weight:700;color:var(--forest-dark);font-size:18px;
  flex:none;
}
.brand-text{font-family:var(--serif);line-height:1.1;}
.brand-text b{font-size:16px;letter-spacing:0.02em;display:block;}
.brand-text span{font-size:11px;letter-spacing:0.14em;text-transform:uppercase;opacity:0.75;}
nav.top-nav{display:flex;gap:2px;flex-wrap:wrap;}
nav.top-nav a{
  color:var(--cream);text-decoration:none;font-size:13px;
  padding:8px 12px;border-radius:20px;opacity:0.82;
  transition:background .18s, opacity .18s;
  white-space:nowrap;
}
nav.top-nav a:hover{background:rgba(232,180,48,0.16);opacity:1;}

/* ---------- Hero ---------- */
.hero{
  position:relative;z-index:1;
  padding:90px 24px 70px;
  max-width:1200px;margin:0 auto;
  display:grid;grid-template-columns:1.15fr 0.85fr;gap:50px;align-items:center;
}
.hero-eyebrow{
  font-family:var(--mono);font-size:12px;letter-spacing:0.2em;
  text-transform:uppercase;color:var(--gold-deep);
  display:flex;align-items:center;gap:10px;margin-bottom:18px;
}
.hero-eyebrow::before{content:"";width:26px;height:1px;background:var(--gold-deep);display:inline-block;}
.hero h1{
  font-family:var(--serif);font-size:clamp(2.4rem,4.6vw,4rem);
  line-height:1.02;margin:0 0 22px;color:var(--forest-dark);
  letter-spacing:-0.01em;
}
.hero h1 em{font-style:italic;color:var(--gold-deep);}
.hero p.lede{font-size:17px;line-height:1.65;color:#33463a;max-width:52ch;margin:0 0 30px;}
.hero-stats{display:flex;gap:28px;flex-wrap:wrap;margin-bottom:8px;}
.stat b{
  display:block;font-family:var(--serif);font-size:2rem;color:var(--forest);
  line-height:1;
}
.stat span{font-size:11px;text-transform:uppercase;letter-spacing:0.1em;color:#6b7a70;}
.hero-cta{display:flex;gap:14px;margin-top:28px;flex-wrap:wrap;}
.btn{
  font-family:var(--sans);font-weight:600;font-size:14px;
  padding:13px 26px;border-radius:3px;border:none;cursor:pointer;
  text-decoration:none;display:inline-flex;align-items:center;gap:8px;
  transition:transform .15s, box-shadow .15s;
}
.btn:hover{transform:translateY(-2px);}
.btn-primary{background:var(--forest);color:var(--cream);box-shadow:0 6px 0 var(--forest-dark);}
.btn-primary:hover{box-shadow:0 8px 0 var(--forest-dark);}
.btn-ghost{background:transparent;color:var(--forest);border:1.5px solid var(--forest);}

/* Hero map/flag mosaic */
.hero-visual{
  position:relative;
  aspect-ratio:1/1;
  border-radius:6px;
  background:var(--forest-dark);
  overflow:hidden;
  box-shadow:0 20px 50px rgba(11,47,31,0.35);
}
.flag-grid{
  position:absolute;inset:0;
  display:grid;grid-template-columns:repeat(9,1fr);grid-auto-rows:1fr;
  opacity:0.9;
}
.flag-grid div{background-size:cover;}
.hero-visual .overlay{
  position:absolute;inset:0;
  background:linear-gradient(160deg, rgba(11,47,31,0.15), rgba(11,47,31,0.85));
  display:flex;align-items:flex-end;padding:26px;
}
.hero-visual .overlay-text{
  font-family:var(--serif);color:var(--cream);font-size:1.15rem;line-height:1.4;
}
.hero-visual .overlay-text b{color:var(--gold);display:block;font-size:1.5rem;}

/* ---------- Section shell ---------- */
section{position:relative;z-index:1;padding:70px 24px;max-width:1200px;margin:0 auto;scroll-margin-top:76px;}
.section-head{margin-bottom:38px;max-width:70ch;}
.eyebrow{
  font-family:var(--mono);font-size:11px;letter-spacing:0.2em;text-transform:uppercase;
  color:var(--gold-deep);margin-bottom:10px;display:block;
}
.section-head h2{
  font-family:var(--serif);font-size:clamp(1.8rem,3vw,2.6rem);
  margin:0 0 14px;color:var(--forest-dark);
}
.section-head p{font-size:15.5px;line-height:1.65;color:#41544a;margin:0;}
.divider{
  height:1px;background:var(--line);max-width:1200px;margin:0 auto;
}

/* ---------- Pillars grid ---------- */
.pillars{display:grid;grid-template-columns:repeat(5,1fr);gap:1px;background:var(--line);border:1px solid var(--line);margin-top:10px;}
.pillar{
  background:var(--paper);padding:26px 20px;min-height:170px;
  display:flex;flex-direction:column;justify-content:space-between;
}
.pillar .num{font-family:var(--mono);color:var(--gold-deep);font-size:12px;}
.pillar h3{font-family:var(--serif);font-size:1.15rem;margin:14px 0 8px;color:var(--forest-dark);}
.pillar p{font-size:13px;color:#586a5f;line-height:1.5;margin:0;}

/* ---------- Region tabs + country directory ---------- */
.region-tabs{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:26px;}
.region-tab{
  font-family:var(--sans);font-size:13px;font-weight:600;
  padding:9px 16px;border-radius:20px;border:1.5px solid var(--line);
  background:var(--paper);color:var(--forest);cursor:pointer;
  transition:all .15s;
}
.region-tab:hover{border-color:var(--forest);}
.region-tab.active{background:var(--forest);color:var(--cream);border-color:var(--forest);}

.search-row{display:flex;gap:12px;margin-bottom:26px;flex-wrap:wrap;}
.search-box{
  flex:1;min-width:220px;
  font-family:var(--sans);font-size:14px;
  padding:12px 16px;border-radius:3px;border:1.5px solid var(--line);
  background:var(--paper);color:var(--ink);
}
.search-box:focus{outline:none;border-color:var(--gold-deep);}
.count-badge{
  font-family:var(--mono);font-size:12px;color:#6b7a70;
  display:flex;align-items:center;padding:0 4px;
}

.country-grid{
  display:grid;grid-template-columns:repeat(auto-fill,minmax(210px,1fr));gap:14px;
}
.country-card{
  background:var(--paper);border:1px solid var(--line);border-radius:4px;
  padding:18px;cursor:pointer;text-align:left;
  transition:border-color .15s, transform .15s, box-shadow .15s;
  display:flex;flex-direction:column;gap:10px;
  font-family:var(--sans);
}
.country-card:hover{border-color:var(--gold-deep);transform:translateY(-3px);box-shadow:0 10px 22px rgba(20,77,52,0.1);}
.country-card .flagbox{
  width:100%;height:64px;border-radius:3px;overflow:hidden;
  background:linear-gradient(135deg,var(--forest),var(--forest-dark));
  display:flex;align-items:center;justify-content:center;
  font-family:var(--serif);color:var(--gold);font-size:1.4rem;font-weight:700;
}
.country-card .cc-name{font-weight:700;font-size:14.5px;color:var(--forest-dark);}
.country-card .cc-meta{font-size:11.5px;color:#7a8a7f;font-family:var(--mono);display:flex;justify-content:space-between;}
.country-card .cc-region{
  font-size:10px;text-transform:uppercase;letter-spacing:0.08em;
  color:var(--gold-deep);font-weight:700;
}

/* ---------- Modal / mini-app ---------- */
.modal-backdrop{
  position:fixed;inset:0;background:rgba(11,20,15,0.6);
  z-index:100;display:none;align-items:flex-start;justify-content:center;
  padding:30px 16px;overflow-y:auto;backdrop-filter: blur(2px);
}
.modal-backdrop.open{display:flex;}
.modal{
  background:var(--paper);max-width:760px;width:100%;
  border-radius:6px;overflow:hidden;
  box-shadow:0 30px 80px rgba(0,0,0,0.4);
  animation:pop .22s ease;
  margin-bottom:30px;
}
@keyframes pop{from{opacity:0;transform:translateY(14px) scale(0.98);}to{opacity:1;transform:none;}}
.modal-head{
  background:linear-gradient(135deg,var(--forest),var(--forest-dark));
  color:var(--cream);padding:30px 32px;position:relative;
}
.modal-head .close-x{
  position:absolute;top:18px;right:20px;
  background:rgba(255,255,255,0.12);border:none;color:var(--cream);
  width:32px;height:32px;border-radius:50%;cursor:pointer;font-size:16px;
  display:flex;align-items:center;justify-content:center;
  transition:background .15s;
}
.modal-head .close-x:hover{background:rgba(255,255,255,0.28);}
.modal-head .mh-flag{font-family:var(--serif);font-size:2.6rem;color:var(--gold);margin-bottom:6px;}
.modal-head h2{font-family:var(--serif);font-size:1.9rem;margin:0 0 6px;}
.modal-head .mh-region{font-family:var(--mono);font-size:11.5px;letter-spacing:0.14em;text-transform:uppercase;color:var(--gold);opacity:0.9;}
.modal-head .mh-code{font-family:var(--mono);font-size:13px;opacity:0.8;margin-top:4px;}

.modal-body{padding:28px 32px 34px;}
.mb-tabs{display:flex;gap:6px;border-bottom:1px solid var(--line);margin-bottom:22px;flex-wrap:wrap;}
.mb-tab{
  font-family:var(--sans);font-size:13px;font-weight:600;
  padding:9px 4px;background:none;border:none;cursor:pointer;
  color:#7a8a7f;position:relative;margin-right:18px;
}
.mb-tab.active{color:var(--forest-dark);}
.mb-tab.active::after{
  content:"";position:absolute;left:0;right:0;bottom:-1px;height:2px;background:var(--gold-deep);
}
.mb-panel{display:none;}
.mb-panel.active{display:block;animation:fadein .2s ease;}
@keyframes fadein{from{opacity:0;}to{opacity:1;}}

.info-row{display:flex;gap:14px;padding:12px 0;border-bottom:1px dashed var(--line);}
.info-row:last-child{border-bottom:none;}
.info-row .ir-label{
  flex:0 0 120px;font-family:var(--mono);font-size:11px;text-transform:uppercase;
  letter-spacing:0.06em;color:var(--gold-deep);padding-top:2px;
}
.info-row .ir-value{flex:1;font-size:14.5px;line-height:1.6;color:var(--ink);}
.info-row .ir-value a{color:var(--forest);font-weight:600;text-decoration:none;border-bottom:1px solid var(--line);}
.info-row .ir-value a:hover{border-color:var(--forest);}

.tool-panel{
  background:var(--cream);border:1px solid var(--line);border-radius:4px;padding:20px;
}
.tool-panel h4{font-family:var(--serif);margin:0 0 6px;font-size:1.05rem;color:var(--forest-dark);}
.tool-panel p{font-size:13px;color:#586a5f;margin:0 0 16px;line-height:1.5;}
.calc-row{display:flex;gap:10px;margin-bottom:12px;flex-wrap:wrap;}
.calc-row input, .calc-row select{
  font-family:var(--sans);padding:10px 12px;border-radius:3px;border:1.5px solid var(--line);
  font-size:13.5px;background:var(--paper);flex:1;min-width:120px;
}
.calc-out{
  font-family:var(--mono);font-size:14px;background:var(--forest);color:var(--cream);
  padding:14px 16px;border-radius:3px;margin-top:8px;
}
.copy-btn{
  font-family:var(--sans);font-size:12.5px;font-weight:600;
  background:var(--forest);color:var(--cream);border:none;border-radius:3px;
  padding:9px 14px;cursor:pointer;margin-top:10px;
}
.copy-btn:hover{background:var(--forest-dark);}
.badge-list{display:flex;gap:8px;flex-wrap:wrap;margin-top:10px;}
.badge{
  font-family:var(--mono);font-size:11px;background:var(--forest);color:var(--cream);
  padding:4px 10px;border-radius:12px;
}
.note-box{
  background:#fff8e6;border:1px solid #e8d9a8;border-radius:4px;padding:14px 16px;
  font-size:12.5px;color:#5c4a10;line-height:1.5;margin-top:14px;
}
.progress-wrap{background:var(--line);height:8px;border-radius:6px;overflow:hidden;margin:8px 0 4px;}
.progress-bar{height:100%;background:linear-gradient(90deg,var(--gold-deep),var(--gold));border-radius:6px;transition:width .3s;}

/* Checklist tool */
.checklist{list-style:none;margin:0;padding:0;display:flex;flex-direction:column;gap:8px;}
.checklist li{
  display:flex;align-items:center;gap:10px;font-size:13.5px;
  background:var(--paper);border:1px solid var(--line);padding:10px 12px;border-radius:3px;
  cursor:pointer;user-select:none;
}
.checklist li.done{opacity:0.5;text-decoration:line-through;}
.checklist li .chk{
  width:18px;height:18px;border-radius:4px;border:1.5px solid var(--forest);flex:none;
  display:flex;align-items:center;justify-content:center;font-size:11px;color:var(--cream);
}
.checklist li.done .chk{background:var(--forest);}

/* ---------- Photo gallery ---------- */
.gallery-grid{
  display:grid;grid-template-columns:repeat(auto-fill,minmax(180px,1fr));gap:14px;
}
.gallery-item{
  background:var(--paper);border:1px solid var(--line);border-radius:4px;overflow:hidden;
  cursor:pointer;transition:transform .15s, box-shadow .15s, border-color .15s;
  display:flex;flex-direction:column;
}
.gallery-item:hover{transform:translateY(-3px);box-shadow:0 12px 26px rgba(20,77,52,0.14);border-color:var(--gold-deep);}
.gallery-item .gi-imgwrap{
  width:100%;aspect-ratio:210/297;overflow:hidden;background:var(--cream);
  display:flex;align-items:center;justify-content:center;position:relative;
}
.gallery-item img{width:100%;height:100%;object-fit:cover;display:block;}
.gallery-item .gi-num{
  position:absolute;top:8px;left:8px;background:rgba(11,47,31,0.82);color:var(--gold);
  font-family:var(--mono);font-size:10.5px;padding:2px 7px;border-radius:10px;
}
.gallery-item .gi-caption{
  padding:10px 12px;font-size:12px;color:var(--forest-dark);line-height:1.4;font-weight:600;
}

.lightbox-backdrop{
  position:fixed;inset:0;background:rgba(6,14,10,0.92);z-index:200;
  display:none;align-items:center;justify-content:center;flex-direction:column;
  padding:24px;
}
.lightbox-backdrop.open{display:flex;}
.lightbox-img-wrap{
  max-width:min(90vw,700px);max-height:78vh;display:flex;align-items:center;justify-content:center;
}
.lightbox-img-wrap img{max-width:100%;max-height:78vh;border-radius:4px;box-shadow:0 20px 60px rgba(0,0,0,0.5);}
.lightbox-caption{
  color:var(--cream);font-family:var(--sans);font-size:13.5px;margin-top:16px;text-align:center;
  display:flex;align-items:center;gap:16px;
}
.lightbox-caption b{color:var(--gold);}
.lb-nav-btn{
  background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.25);color:var(--cream);
  width:40px;height:40px;border-radius:50%;cursor:pointer;font-size:16px;
  display:flex;align-items:center;justify-content:center;transition:background .15s;
}
.lb-nav-btn:hover{background:rgba(255,255,255,0.25);}
.lb-close{
  position:absolute;top:20px;right:24px;background:rgba(255,255,255,0.1);
  border:1px solid rgba(255,255,255,0.25);color:var(--cream);width:38px;height:38px;
  border-radius:50%;cursor:pointer;font-size:16px;
}
.lb-close:hover{background:rgba(255,255,255,0.25);}
.lb-controls{display:flex;align-items:center;gap:18px;margin-top:18px;}

/* ---------- Org / programme cards ---------- */
.prog-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:18px;}
.prog-card{
  background:var(--paper);border:1px solid var(--line);border-radius:4px;padding:24px;
  border-top:3px solid var(--gold-deep);
}
.prog-card .pc-n{font-family:var(--mono);color:var(--gold-deep);font-size:12px;margin-bottom:10px;display:block;}
.prog-card h3{font-family:var(--serif);font-size:1.2rem;margin:0 0 10px;color:var(--forest-dark);}
.prog-card p{font-size:13.5px;color:#586a5f;line-height:1.55;margin:0;}

/* People strip */
.people-strip{
  display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:16px;
}
.person{text-align:center;}
.person .pv{
  width:78px;height:78px;border-radius:50%;margin:0 auto 10px;
  background:linear-gradient(135deg,var(--forest),var(--forest-dark));
  display:flex;align-items:center;justify-content:center;
  font-family:var(--serif);color:var(--gold);font-size:1.3rem;font-weight:700;
}
.person b{display:block;font-size:12.5px;color:var(--forest-dark);line-height:1.35;}
.person span{display:block;font-size:11px;color:#8a9890;margin-top:2px;}

footer{
  background:var(--forest-dark);color:var(--cream);padding:50px 24px 30px;
  position:relative;z-index:1;
}
.footer-inner{max-width:1200px;margin:0 auto;display:flex;justify-content:space-between;flex-wrap:wrap;gap:30px;}
.footer-inner h4{font-family:var(--serif);font-size:1.1rem;margin:0 0 12px;color:var(--gold);}
.footer-inner p, .footer-inner a{font-size:13px;color:rgba(247,242,228,0.75);line-height:1.7;text-decoration:none;}
.footer-inner a:hover{color:var(--gold);}
.footer-bottom{
  max-width:1200px;margin:36px auto 0;padding-top:20px;border-top:1px solid rgba(247,242,228,0.15);
  font-size:12px;color:rgba(247,242,228,0.5);text-align:center;font-family:var(--mono);
}

@media (max-width:820px){
  .hero{grid-template-columns:1fr;padding-top:50px;}
  .hero-visual{max-width:340px;margin:0 auto;}
  nav.top-nav{display:none;}
  .pillars{grid-template-columns:repeat(2,1fr);}
}
@media (max-width:480px){
  .pillars{grid-template-columns:1fr;}
}
</style>
</head>
<body>

<header class="top">
  <div class="top-inner">
    <div class="brand" onclick="window.scrollTo({top:0,behavior:'smooth'})">
      <div class="brand-mark">TJG</div>
      <div class="brand-text"><b>Joshua Generation</b><span>International Network</span></div>
    </div>
    <nav class="top-nav">
      <a href="#overview">Overview</a>
      <a href="#programmes">Programmes</a>
      <a href="#network">Africa Network</a>
      <a href="#countries">Countries</a>
      <a href="#gallery">Photos</a>
      <a href="#leadership">Leadership</a>
      <a href="#calendar">Calendar</a>
    </nav>
  </div>
</header>

<div class="hero">
  <div>
    <span class="hero-eyebrow">TJG Profile · 2026 Edition</span>
    <h1>Raising a generation that will <em>disciple all nations.</em></h1>
    <p class="lede">The Joshua Generation International Network coordinates awareness, relief, empowerment, missions, sports and music programmes across 234 nations — built on a seven-member committee model that stretches from International to Cell level.</p>
    <div class="hero-stats">
      <div class="stat"><b>54</b><span>Nations in Africa</span></div>
      <div class="stat"><b>5</b><span>African Regions</span></div>
      <div class="stat"><b>50,000+</b><span>Appointed Leaders</span></div>
      <div class="stat"><b>1988</b><span>Founding Year</span></div>
    </div>
    <div class="hero-cta">
      <a href="#countries" class="btn btn-primary">Open Country Directory ↓</a>
      <a href="#overview" class="btn btn-ghost">Read the Vision</a>
    </div>
  </div>
  <div class="hero-visual">
    <div class="flag-grid" id="heroFlagGrid"></div>
    <div class="overlay">
      <div class="overlay-text"><b>#DiscipleAllNations</b>Southern · East · Central · West · North Africa</div>
    </div>
  </div>
</div>

<div class="divider"></div>

<section id="overview">
  <div class="section-head">
    <span class="eyebrow">1.0 Introduction</span>
    <h2>Vision, mission &amp; the twelve words</h2>
    <p>To raise a generation that will collectively and cooperatively pursue and turn their dreams into tangible reality — coordinating members and the corporate sector around Awareness, Relief, Empowerment, Missions, and Sports programmes that would otherwise be difficult to pursue alone.</p>
  </div>
  <div class="pillars">
    <div class="pillar"><span class="num">Values</span><h3>Love &amp; Order</h3><p>Love, Order, Unity, Voluntary Mutual Submission, Honesty, Quality and Excellence, Transparency, Connectivity, Societal Sustainability.</p></div>
    <div class="pillar"><span class="num">Motto</span><h3>#DiscipleAllNations</h3><p>The rallying call carried into every national launch, crusade, and regional summit since inception.</p></div>
    <div class="pillar"><span class="num">12 Words</span><h3>Modern · Online · Network</h3><p>Intercessory, Evangelical, Discipleship, Christian, Youth, Business, Consortium, Leadership, Movement.</p></div>
    <div class="pillar"><span class="num">Founded</span><h3>1988</h3><p>Instituted under Dr. Jose V. Pascua's Board of Directors, with roots in monthly all-night prayer meetings from 2011.</p></div>
    <div class="pillar"><span class="num">Structure</span><h3>7-Member Committees</h3><p>Replicated from International, Continental, Regional, National, down to State, County, Ward, Branch and Cell level.</p></div>
  </div>
</section>

<div class="divider"></div>

<section id="programmes">
  <div class="section-head">
    <span class="eyebrow">4.0 Programmes</span>
    <h2>Five pillars of service delivery</h2>
    <p>Every national chapter is built on the same five-phase engine — each phase unlocking the next.</p>
  </div>
  <div class="prog-grid">
    <div class="prog-card"><span class="pc-n">01</span><h3>Awareness</h3><p>Leadership seminars, revivals, crusades, official launches, conferences and summits — plus School, University and Church Clubs.</p></div>
    <div class="prog-card"><span class="pc-n">02</span><h3>Relief</h3><p>Humanitarian and recreational support for orphans, widows and the elderly, including food hampers and healthcare coordination.</p></div>
    <div class="prog-card"><span class="pc-n">03</span><h3>Empowerment</h3><p>SACCOs and Micro-Finance, Brand Ambassador and Distributor networks, and business development units.</p></div>
    <div class="prog-card"><span class="pc-n">04</span><h3>Missions</h3><p>Continental and Regional missions directors pushing to set foot in all 54 African nations and beyond.</p></div>
    <div class="prog-card"><span class="pc-n">05</span><h3>CSRM Sports</h3><p>Partnership with Church Sports and Recreation Ministries — sport as a modern form of evangelism.</p></div>
  </div>
</section>

<div class="divider"></div>

<section id="network"><a id="countries"></a>
  <div class="section-head">
    <span class="eyebrow">7.0 Africa Network</span>
    <h2>Five regions, fifty-four nations</h2>
    <p>Search or filter the directory below, then open any country to launch its own mini profile — leadership contacts, a WhatsApp-message generator, a conference countdown, and a launch-readiness checklist.</p>
  </div>

  <div class="region-tabs" id="regionTabs"></div>
  <div class="search-row">
    <input type="text" class="search-box" id="searchBox" placeholder="Search by country name, code, or leader…">
    <div class="count-badge" id="countBadge"></div>
  </div>
  <div class="country-grid" id="countryGrid"></div>
</section>

<div class="divider"></div>

<section id="gallery">
  <div class="section-head">
    <span class="eyebrow">9.0 &amp; 10.0 Photos &amp; News Bulletin</span>
    <h2>Every page, as it appeared</h2>
    <p>All 97 pages of the TJG Profile 2026 — cover, directors' columns, photo galleries, calendar, and continued stories — reproduced here exactly as laid out in the original document. Filter by section or open any page full-size.</p>
  </div>
  <div class="region-tabs" id="galleryTabs"></div>
  <div class="search-row">
    <input type="text" class="search-box" id="gallerySearch" placeholder="Search page titles… e.g. 'Gallery', 'Director', 'Congo'">
    <div class="count-badge" id="galleryCount"></div>
  </div>
  <div class="gallery-grid" id="galleryGrid"></div>
</section>

<div class="divider"></div>

<section id="leadership">
  <div class="section-head">
    <span class="eyebrow">11.0 Coordination</span>
    <h2>International executive</h2>
    <p>The presidium sits above five networks (Africa, Asia, Europe, the Americas, Australia/Oceania) each mirroring the same seven-member committee model.</p>
  </div>
  <div class="people-strip">
    <div class="person"><div class="pv">JP</div><b>Dr. Jose V. Pascua</b><span>Founder / President</span></div>
    <div class="person"><div class="pv">AH</div><b>Prophetess Ann Hubbard</b><span>Founder / CEO</span></div>
    <div class="person"><div class="pv">XM</div><b>Apostle Dr. Xavier Mzembi</b><span>Founder / Chairperson</span></div>
    <div class="person"><div class="pv">WO</div><b>Bishop Dr. Walter Ogwada</b><span>Patron</span></div>
    <div class="person"><div class="pv">PW</div><b>Bishop Patrick W. Wataka</b><span>Executive Director</span></div>
    <div class="person"><div class="pv">AI</div><b>Apostle Albert Itoumbou</b><span>Africa President</span></div>
    <div class="person"><div class="pv">HB</div><b>Prof. Habonimana Baptiste</b><span>Africa Chairperson</span></div>
    <div class="person"><div class="pv">WS</div><b>Dr. William Ssekyanzi</b><span>Africa Executive Director</span></div>
  </div>
</section>

<div class="divider"></div>

<section id="calendar">
  <div class="section-head">
    <span class="eyebrow">13.0 Calendar Tool</span>
    <h2>Countdown to your national conference</h2>
    <p>Pick a country in the directory above to see its scheduled conference date and a live countdown — or use the quick picker here.</p>
  </div>
  <div class="tool-panel" style="max-width:480px;">
    <h4>Quick countdown</h4>
    <div class="calc-row">
      <select id="quickPick"></select>
    </div>
    <div class="calc-out" id="quickOut">Select a nation above.</div>
  </div>
</section>

<footer>
  <div class="footer-inner">
    <div>
      <h4>The Joshua Generation International Network</h4>
      <p>info@tjgint.org<br>www.tjgint.org<br>www.thejoshuageneration.org</p>
    </div>
    <div>
      <h4>Headquarters</h4>
      <p>Houston, Texas, USA (HQ)<br>Kent, United Kingdom (Int'l Executive)<br>Nairobi, Kenya (African Secretariat)</p>
    </div>
    <div>
      <h4>Site</h4>
      <p><a href="#overview">Overview</a><br><a href="#programmes">Programmes</a><br><a href="#countries">Country Directory</a></p>
    </div>
  </div>
  <div class="footer-bottom">#DiscipleAllNations — TJG Profile 2026, rebuilt as an interactive directory.</div>
</footer>

<div class="modal-backdrop" id="modalBackdrop">
  <div class="modal" id="modalContent"></div>
</div>

<div class="lightbox-backdrop" id="lightboxBackdrop">
  <button class="lb-close" onclick="closeLightbox()">✕</button>
  <div class="lightbox-img-wrap"><img id="lightboxImg" src="" alt=""></div>
  <div class="lb-controls">
    <button class="lb-nav-btn" onclick="lbNav(-1)">‹</button>
    <div class="lightbox-caption"><b id="lightboxPageNum"></b><span id="lightboxLabel"></span></div>
    <button class="lb-nav-btn" onclick="lbNav(1)">›</button>
  </div>
</div>

<script>
const TJG_PAGES = [
{"n":1,"label":"Cover — TJG Profile 2026","src":"data:image/jpeg;base64,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
