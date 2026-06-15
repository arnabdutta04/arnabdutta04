
<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=JetBrains+Mono:wght@300;400;500&display=swap');
*{margin:0;padding:0;box-sizing:border-box}
body{background:#f6f8fa;color:#1a1a2e;font-family:'Space Grotesk',sans-serif;min-height:100vh}
.page{max-width:760px;margin:0 auto;padding:32px 24px 56px}

/* ── HERO ── */
.hero{padding:8px 0 36px;text-align:center}
.hero-badge{
  display:inline-flex;align-items:center;gap:7px;
  font-family:'JetBrains Mono',monospace;font-size:10px;letter-spacing:.14em;text-transform:uppercase;
  color:#5c40cc;background:#ede9fe;border:1px solid #c4b5fd;border-radius:20px;padding:5px 14px;margin-bottom:20px
}
.hero-badge .dot{width:6px;height:6px;border-radius:50%;background:#7c3aed;animation:pulse 2s ease-in-out infinite}
@keyframes pulse{0%,100%{opacity:1;transform:scale(1)}50%{opacity:.4;transform:scale(.7)}}

.avatar-ring{
  width:88px;height:88px;border-radius:50%;margin:0 auto 18px;
  background:linear-gradient(135deg,#7c3aed 0%,#2dd4bf 100%);
  display:flex;align-items:center;justify-content:center;
  font-family:'Space Grotesk',sans-serif;font-size:28px;font-weight:700;color:#fff;letter-spacing:-1px
}

.hero-name{font-size:40px;font-weight:700;letter-spacing:-0.03em;color:#0f0f1a;line-height:1;margin-bottom:4px}
.hero-name .acc{color:#7c3aed}
.hero-name .dim{color:#94a3b8}

.hero-role{
  font-family:'JetBrains Mono',monospace;font-size:13px;color:#64748b;
  margin-top:12px;height:20px;display:flex;align-items:center;justify-content:center;gap:4px
}
.hero-role .cursor{display:inline-block;width:2px;height:14px;background:#7c3aed;animation:blink 1s step-end infinite;border-radius:1px}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}

/* ── RULE ── */
.rule{height:1px;margin:28px 0;background:linear-gradient(90deg,#7c3aed,#2dd4bf 40%,transparent 80%);opacity:.25}

/* ── EYEBROW ── */
.eyebrow{
  font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:.22em;text-transform:uppercase;
  color:#94a3b8;margin-bottom:16px;display:flex;align-items:center;gap:10px
}
.eyebrow::after{content:'';flex:1;height:1px;background:#e2e8f0}

/* ── INFO GRID ── */
.info-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:32px}
.info-card{
  background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:14px 16px;
  display:flex;align-items:flex-start;gap:12px;
  transition:border-color .2s,transform .2s,box-shadow .2s
}
.info-card:hover{border-color:#a78bfa;transform:translateY(-2px);box-shadow:0 4px 16px rgba(124,58,237,.08)}
.ic-glyph{
  font-family:'JetBrains Mono',monospace;font-size:14px;color:#7c3aed;
  background:#f5f3ff;border:1px solid #ede9fe;border-radius:8px;
  padding:6px 8px;flex-shrink:0;min-width:34px;text-align:center;line-height:1
}
.ic-label{font-size:9px;letter-spacing:.12em;text-transform:uppercase;color:#94a3b8;margin-bottom:3px}
.ic-val{font-size:12.5px;color:#334155;line-height:1.4}

/* ── SKILL BARS ── */
.skill-section{margin-bottom:32px}
.skill-row{display:flex;align-items:center;gap:12px;margin-bottom:10px}
.skill-name{font-family:'JetBrains Mono',monospace;font-size:11px;color:#475569;width:110px;flex-shrink:0}
.skill-track{flex:1;height:4px;background:#e2e8f0;border-radius:4px;overflow:hidden}
.skill-fill{height:100%;border-radius:4px;transform:scaleX(0);transform-origin:left;transition:transform 1.1s cubic-bezier(.16,1,.3,1)}
.skill-fill.go{transform:scaleX(1)}
.skill-pct{font-family:'JetBrains Mono',monospace;font-size:10px;color:#94a3b8;width:34px;text-align:right;flex-shrink:0}

/* ── TAG PILLS ── */
.tags-section{margin-bottom:32px}
.tag-group{margin-bottom:16px}
.tag-group-label{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:.15em;text-transform:uppercase;color:#94a3b8;margin-bottom:9px}
.tag-wrap{display:flex;flex-wrap:wrap;gap:7px}
.tag{
  font-family:'JetBrains Mono',monospace;font-size:11px;
  padding:4px 12px;border-radius:6px;border:1px solid;
  transition:all .18s;cursor:default
}
.tag:hover{transform:translateY(-2px)}
.tp{color:#5c40cc;border-color:#c4b5fd;background:#f5f3ff}.tp:hover{background:#ede9fe}
.tt{color:#0f766e;border-color:#99f6e4;background:#f0fdfa}.tt:hover{background:#ccfbf1}
.tg{color:#475569;border-color:#cbd5e1;background:#f8fafc}.tg:hover{background:#f1f5f9}

/* ── STATS ── */
.stats-section{margin-bottom:32px}
.stats-row{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.stat-card{
  background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:20px 12px 16px;
  text-align:center;transition:border-color .2s,transform .2s,box-shadow .2s
}
.stat-card:hover{border-color:#a78bfa;transform:translateY(-2px);box-shadow:0 4px 16px rgba(124,58,237,.08)}
.stat-num{
  font-family:'Space Grotesk',sans-serif;font-size:32px;font-weight:700;
  letter-spacing:-0.05em;line-height:1;margin-bottom:6px
}
.stat-lbl{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:.14em;text-transform:uppercase;color:#94a3b8}

/* ── CONNECT ── */
.connect-section{margin-bottom:32px}
.connect-row{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
.cc{
  background:#fff;border:1px solid #e2e8f0;border-radius:12px;padding:14px 16px;
  display:flex;flex-direction:column;gap:8px;cursor:pointer;
  transition:all .2s;text-decoration:none
}
.cc:hover{transform:translateY(-3px)}
.cc[data-c="gh"]:hover{border-color:#334155;box-shadow:0 4px 16px rgba(51,65,85,.1)}
.cc[data-c="li"]:hover{border-color:#3b82f6;box-shadow:0 4px 16px rgba(59,130,246,.1)}
.cc[data-c="em"]:hover{border-color:#ec4899;box-shadow:0 4px 16px rgba(236,72,153,.1)}
.cc-icon{width:28px;height:28px;border-radius:8px;display:flex;align-items:center;justify-content:center}
.cc[data-c="gh"] .cc-icon{background:#f1f5f9}
.cc[data-c="li"] .cc-icon{background:#eff6ff}
.cc[data-c="em"] .cc-icon{background:#fdf2f8}
.cc-plat{font-family:'JetBrains Mono',monospace;font-size:9px;letter-spacing:.14em;text-transform:uppercase;color:#94a3b8}
.cc-handle{font-family:'JetBrains Mono',monospace;font-size:11px;color:#334155;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}

/* ── QUOTE ── */
.quote{
  margin-top:32px;padding:16px 20px;
  background:#f5f3ff;border-left:3px solid #7c3aed;border-radius:0 10px 10px 0
}
.quote-text{font-family:'JetBrains Mono',monospace;font-size:12px;color:#64748b;line-height:1.75}
.quote-text em{color:#7c3aed;font-style:normal}

/* ── FADE IN ── */
.fi{opacity:0;transform:translateY(14px);transition:opacity .5s ease,transform .5s ease}
.fi.vis{opacity:1;transform:translateY(0)}
</style>

<div class="page">
  <h2 style="position:absolute;width:1px;height:1px;overflow:hidden">Arnab Dutta GitHub profile readme</h2>

  <!-- HERO -->
  <section class="hero fi">
    <div class="hero-badge"><span class="dot"></span>Open to Work · Batch 2027</div>
    <div class="avatar-ring">AD</div>
    <div class="hero-name"><span class="dim">~/</span>arnab<span class="acc">.</span>dutta</div>
    <div class="hero-role"><span id="typed"></span><span class="cursor"></span></div>
  </section>

  <div class="rule fi"></div>

  <!-- INFO -->
  <section class="fi">
    <div class="eyebrow">About</div>
    <div class="info-grid">
      <div class="info-card">
        <div class="ic-glyph">▸</div>
        <div><div class="ic-label">Education</div><div class="ic-val">B.Tech CSE · IEM Kolkata · 2027</div></div>
      </div>
      <div class="info-card">
        <div class="ic-glyph">▸</div>
        <div><div class="ic-label">Focus</div><div class="ic-val">AI / ML · Data Science · Full Stack</div></div>
      </div>
      <div class="info-card">
        <div class="ic-glyph">▸</div>
        <div><div class="ic-label">Contributions</div><div class="ic-val">442+ commits last year</div></div>
      </div>
      <div class="info-card">
        <div class="ic-glyph">▸</div>
        <div><div class="ic-label">Location</div><div class="ic-val">Kolkata, West Bengal, India</div></div>
      </div>
    </div>
  </section>

  <!-- SKILLS -->
  <section class="skill-section fi" id="skillSec">
    <div class="eyebrow">Proficiency</div>
    <div class="skill-row"><span class="skill-name">Python</span><div class="skill-track"><div class="skill-fill" style="background:#7c3aed;width:90%"></div></div><span class="skill-pct">90%</span></div>
    <div class="skill-row"><span class="skill-name">ML / AI</span><div class="skill-track"><div class="skill-fill" style="background:#6d28d9;width:82%"></div></div><span class="skill-pct">82%</span></div>
    <div class="skill-row"><span class="skill-name">JavaScript</span><div class="skill-track"><div class="skill-fill" style="background:#0d9488;width:78%"></div></div><span class="skill-pct">78%</span></div>
    <div class="skill-row"><span class="skill-name">Data Science</span><div class="skill-track"><div class="skill-fill" style="background:#0f766e;width:75%"></div></div><span class="skill-pct">75%</span></div>
    <div class="skill-row"><span class="skill-name">HTML / CSS</span><div class="skill-track"><div class="skill-fill" style="background:#0d9488;width:80%"></div></div><span class="skill-pct">80%</span></div>
    <div class="skill-row"><span class="skill-name">Java</span><div class="skill-track"><div class="skill-fill" style="background:#7c3aed;width:65%"></div></div><span class="skill-pct">65%</span></div>
  </section>

  <!-- TAGS -->
  <section class="tags-section fi">
    <div class="eyebrow">Stack</div>
    <div class="tag-group">
      <div class="tag-group-label">Languages</div>
      <div class="tag-wrap">
        <span class="tag tp">Python</span><span class="tag tp">JavaScript</span><span class="tag tp">Java</span><span class="tag tp">HTML5</span><span class="tag tp">CSS3</span>
      </div>
    </div>
    <div class="tag-group">
      <div class="tag-group-label">AI · ML · Data Science</div>
      <div class="tag-wrap">
        <span class="tag tt">TensorFlow</span><span class="tag tt">Scikit-Learn</span><span class="tag tt">Pandas</span><span class="tag tt">NumPy</span><span class="tag tt">Matplotlib</span><span class="tag tt">Jupyter</span>
      </div>
    </div>
    <div class="tag-group">
      <div class="tag-group-label">Tools</div>
      <div class="tag-wrap">
        <span class="tag tg">Git</span><span class="tag tg">GitHub</span><span class="tag tg">VS Code</span><span class="tag tg">Postman</span>
      </div>
    </div>
  </section>

  <!-- STATS -->
  <section class="stats-section fi" id="statSec">
    <div class="eyebrow">Numbers</div>
    <div class="stats-row">
      <div class="stat-card"><div class="stat-num" id="s1" style="color:#7c3aed">0</div><div class="stat-lbl">Contributions</div></div>
      <div class="stat-card"><div class="stat-num" id="s2" style="color:#0d9488">0</div><div class="stat-lbl">Repositories</div></div>
      <div class="stat-card"><div class="stat-num" id="s3" style="color:#6d28d9">0</div><div class="stat-lbl">Years Active</div></div>
    </div>
  </section>

  <!-- CONNECT -->
  <section class="connect-section fi">
    <div class="eyebrow">Connect</div>
    <div class="connect-row">
      <div class="cc" data-c="gh">
        <div class="cc-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="#334155"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z"/></svg></div>
        <div><div class="cc-plat">GitHub</div><div class="cc-handle">arnabdutta04</div></div>
      </div>
      <div class="cc" data-c="li">
        <div class="cc-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="#2563eb"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg></div>
        <div><div class="cc-plat">LinkedIn</div><div class="cc-handle">arnabdutta04</div></div>
      </div>
      <div class="cc" data-c="em">
        <div class="cc-icon"><svg width="16" height="16" viewBox="0 0 24 24" fill="#db2777"><path d="M24 5.457v13.909c0 .904-.732 1.636-1.636 1.636h-3.819V11.73L12 16.64l-6.545-4.91v9.273H1.636A1.636 1.636 0 0 1 0 19.366V5.457c0-2.023 2.309-3.178 3.927-1.964L5.455 4.64 12 9.548l6.545-4.91 1.528-1.145C21.69 2.28 24 3.434 24 5.457z"/></svg></div>
        <div><div class="cc-plat">Email</div><div class="cc-handle">arnabdutta453@gmail</div></div>
      </div>
    </div>
  </section>

  <!-- QUOTE -->
  <div class="quote fi">
    <div class="quote-text">"The best way to predict the future is to <em>build it.</em>"</div>
  </div>
</div>

<script>
const lines=['AI / ML Engineer in Making','Full Stack Developer','Data Science Enthusiast','Building the future, one commit at a time'];
let li=0,ci=0,del=false;
const el=document.getElementById('typed');
function type(){
  const cur=lines[li];
  if(!del){el.textContent=cur.slice(0,++ci);if(ci===cur.length){del=true;setTimeout(type,1600);return}setTimeout(type,50);}
  else{el.textContent=cur.slice(0,--ci);if(ci===0){del=false;li=(li+1)%lines.length;setTimeout(type,300);return}setTimeout(type,25);}
}
setTimeout(type,700);

function countUp(id,target,dur){
  const e=document.getElementById(id),t0=Date.now();
  const tick=()=>{const p=Math.min((Date.now()-t0)/dur,1);const ease=1-Math.pow(1-p,3);e.textContent=Math.round(ease*target)+(id==='s1'?'+':'');if(p<1)requestAnimationFrame(tick);};
  tick();
}

let counted=false,barsAnimated=false;
const io=new IntersectionObserver(entries=>{
  entries.forEach(en=>{
    if(en.isIntersecting){
      en.target.classList.add('vis');
      if(en.target.id==='statSec'&&!counted){counted=true;setTimeout(()=>{countUp('s1',442,1200);countUp('s2',12,900);countUp('s3',3,700);},200);}
      if(en.target.id==='skillSec'&&!barsAnimated){barsAnimated=true;setTimeout(()=>{en.target.querySelectorAll('.skill-fill').forEach((b,i)=>setTimeout(()=>b.classList.add('go'),i*90));},150);}
    }
  });
},{threshold:.15});
document.querySelectorAll('.fi').forEach(e=>io.observe(e));
</script>
