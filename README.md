:root { --navy:#123a63; --blue:#1769aa; --sky:#e9f4fb; --ink:#172536; --muted:#607083; --line:#d9e3ec; --white:#fff; --paper:#f7f9fb; }
* { box-sizing:border-box; }
html { scroll-behavior:smooth; scroll-padding-top:84px; }
body { margin:0; color:var(--ink); background:var(--white); font-family:"Pretendard","Noto Sans KR","Malgun Gothic",Arial,sans-serif; word-break:keep-all; }
a { color:inherit; text-decoration:none; }
.progress { position:fixed; z-index:100; top:0; left:0; width:0; height:4px; background:#3aa7db; transition:width .1s linear; }
.site-header { position:sticky; z-index:50; top:0; background:rgba(255,255,255,.95); border-bottom:1px solid var(--line); backdrop-filter:blur(10px); }
.header-inner,.section-inner,.hero-inner { width:min(1120px,calc(100% - 40px)); margin:0 auto; }
.header-inner { min-height:72px; display:flex; align-items:center; justify-content:space-between; gap:24px; }
.brand { font-weight:800; color:var(--navy); letter-spacing:-.03em; }
nav { display:flex; gap:28px; font-size:15px; font-weight:700; color:#40546b; }
nav a:hover,nav a:focus-visible { color:var(--blue); }
.hero { position:relative; overflow:hidden; color:white; background:linear-gradient(125deg,#102f51 0%,#165b8d 65%,#2087b5 100%); }
.hero::after { content:""; position:absolute; width:440px; height:440px; right:-100px; top:-180px; border:80px solid rgba(255,255,255,.07); border-radius:50%; }
.hero-inner { position:relative; z-index:1; padding:92px 0 80px; }
.eyebrow,.section-kicker { margin:0 0 14px; color:#5db5e3; font-size:14px; font-weight:800; letter-spacing:.08em; text-transform:uppercase; }
h1 { max-width:840px; margin:0; font-size:clamp(38px,6vw,66px); line-height:1.17; letter-spacing:-.055em; }
.lead { max-width:780px; margin:28px 0 34px; color:#deedf7; font-size:19px; line-height:1.8; }
.period { display:inline-flex; align-items:center; gap:14px; padding:12px 18px; border:1px solid rgba(255,255,255,.32); border-radius:9px; background:rgba(255,255,255,.08); }
.period span { color:#a9d8ef; font-size:13px; font-weight:800; }.period strong{font-size:16px;letter-spacing:.02em}
.summary { background:var(--paper); padding:80px 0; }
h2 { margin:0; color:var(--navy); font-size:clamp(30px,4vw,44px); letter-spacing:-.045em; line-height:1.25; }
.summary-grid { display:grid; grid-template-columns:repeat(3,1fr); gap:16px; margin-top:36px; }
.summary-grid article { display:flex; min-height:150px; flex-direction:column; justify-content:center; padding:28px; border:1px solid var(--line); border-top:4px solid var(--blue); background:white; box-shadow:0 12px 30px rgba(20,54,84,.05); }
.summary-grid strong { color:var(--blue); font-size:30px; letter-spacing:-.04em; }.summary-grid span{margin-top:8px;color:#536579;font-size:16px}
.policy-section { padding:104px 0; }.policy-section.alternate{background:#f2f7fa}
.split { display:grid; grid-template-columns:minmax(260px,.75fr) minmax(0,1.25fr); gap:80px; align-items:start; }
.section-heading { position:sticky; top:112px; }.number{display:block;margin-bottom:24px;color:#a5c8dc;font-size:20px;font-weight:800}
.section-heading>p:last-child { margin:22px 0 0; color:var(--muted); font-size:17px; line-height:1.8; }
.policy-list { display:grid; gap:12px; margin:0; padding:0; list-style:none; }
.policy-list li { display:flex; gap:18px; padding:26px; border:1px solid var(--line); border-radius:12px; background:white; }
.check { display:grid; width:30px; height:30px; flex:none; place-items:center; border-radius:50%; color:white; background:var(--blue); font-weight:900; }
.policy-list h3 { margin:2px 0 9px; color:var(--navy); font-size:20px; }.policy-list p{margin:0;color:#526477;line-height:1.75}
.schedule { padding:96px 0; }.schedule-card{padding:48px;border-radius:16px;color:white;background:var(--navy)}
.schedule-card .section-kicker{color:#71c5ea}.schedule-card h2{max-width:730px;color:white}
.schedule-card ol { display:grid; grid-template-columns:repeat(3,1fr); gap:1px; margin:38px 0 0; padding:0; list-style:none; background:rgba(255,255,255,.2); }
.schedule-card li { display:flex; min-height:125px; flex-direction:column; gap:10px; padding:24px; background:var(--navy); }.schedule-card li strong{color:#74c9ed}.schedule-card li span{line-height:1.5}
.note { margin:24px 0 0; color:#ccdfed; font-size:14px; }.quote-section{padding:100px 0;background:var(--sky);text-align:center}
blockquote { max-width:920px; margin:0 auto; color:var(--navy); font-family:Georgia,"Noto Serif KR",serif; font-size:clamp(23px,3vw,34px); font-weight:700; line-height:1.65; letter-spacing:-.025em; }
.attribution { margin:26px 0 0; color:#62778b; }.attribution strong{color:var(--navy)}
footer { padding:30px 0; color:#b6c7d5; background:#0d2945; font-size:14px; }footer .section-inner{display:flex;align-items:center;justify-content:space-between;gap:20px}footer div div{display:flex;align-items:center;gap:12px}footer strong{color:white;font-size:17px}footer p{margin:0}
.top-button { position:fixed; z-index:40; right:24px; bottom:24px; width:48px; height:48px; border:0; border-radius:50%; color:white; background:var(--blue); box-shadow:0 8px 24px rgba(17,62,99,.28); font-size:22px; cursor:pointer; opacity:0; pointer-events:none; transform:translateY(8px); transition:.2s; }.top-button.visible{opacity:1;pointer-events:auto;transform:none}
:focus-visible { outline:3px solid #f7b731; outline-offset:4px; }
@media (max-width:800px){nav{display:none}.hero-inner{padding:68px 0 64px}.desktop-break{display:none}.summary,.policy-section,.schedule,.quote-section{padding:68px 0}.summary-grid{grid-template-columns:1fr}.summary-grid article{min-height:120px}.split{grid-template-columns:1fr;gap:36px}.section-heading{position:static}.schedule-card{padding:32px 24px}.schedule-card ol{grid-template-columns:1fr}.schedule-card li{min-height:auto}.header-inner,.section-inner,.hero-inner{width:min(100% - 28px,1120px)}footer .section-inner{align-items:flex-start;flex-direction:column}.lead{font-size:17px}.period{align-items:flex-start;flex-direction:column;gap:4px}}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}.top-button{transition:none}}
