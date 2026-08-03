<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no,viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<title>SALAD DAYS</title>
<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@12..96,800&family=Space+Grotesk:wght@400;500;700&display=swap" rel="stylesheet">
<style>
:root{--bg:#241A12;--pale:#F6ECD9;--dim:#A08A6E;--gold:#F2B33D;--red:#E2503B;--blue:#7FC24B;--green:#9FD86B;--line:#FFFFFF1E}
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;-webkit-user-select:none;user-select:none}
html,body{height:100%;overflow:hidden;background:var(--bg);color:var(--pale);
  font-family:"Space Grotesk",system-ui,sans-serif;touch-action:none;overscroll-behavior:none}
canvas{display:block;position:fixed;inset:0}
#hud{position:fixed;inset:0;pointer-events:none;z-index:3}
.tag{font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--dim)}
#top{position:absolute;top:max(10px,env(safe-area-inset-top));left:12px;right:12px}
#waveRow{display:flex;justify-content:space-between;align-items:baseline}
#waveN{font-family:"Bricolage Grotesque",sans-serif;font-size:26px;line-height:1;letter-spacing:-.03em}
#left{font-family:"Bricolage Grotesque",sans-serif;font-size:18px;color:var(--red)}
#towers{display:flex;gap:5px;margin-top:6px}
.tw{flex:1;height:6px;background:#FFFFFF14;border:1px solid var(--line);border-radius:3px;overflow:hidden}
.tw i{display:block;height:100%;background:var(--blue);transition:width .15s}
.tw.dead i{background:var(--red);width:0!important}
#hpWrap{position:absolute;bottom:calc(max(10px,env(safe-area-inset-bottom)) + 84px);left:12px;right:12px}
#hpBar{height:9px;background:#FFFFFF14;border:1px solid var(--line);border-radius:3px;overflow:hidden}
#hpBar i{display:block;height:100%;background:linear-gradient(90deg,#5FD08A,#F2B33D);transition:width .12s}
#perks{position:absolute;bottom:calc(max(10px,env(safe-area-inset-bottom)) + 100px);left:12px;right:12px;
  display:flex;gap:3px;flex-wrap:wrap}
.perk{font-size:8px;letter-spacing:.06em;text-transform:uppercase;color:var(--gold);
  border:1px solid #F2B33D44;border-radius:5px;padding:2px 5px;background:#F2B33D14}
.perk b{font-weight:700;opacity:.7}
.perk.dying{color:var(--red);border-color:#E8574C66;background:#E8574C1A;animation:pulse .9s infinite}
.perk.anchored{color:var(--blue);border-color:#5B9BD588;background:#5B9BD51F}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:.45}}
#stickZone{position:absolute;inset:0;pointer-events:auto}
#msg{position:absolute;top:38%;left:0;right:0;text-align:center;font-family:"Bricolage Grotesque",sans-serif;
  font-size:clamp(20px,7vw,34px);text-transform:uppercase;letter-spacing:-.02em;opacity:0;
  transition:opacity .2s;color:var(--gold)}
.screen{position:fixed;inset:0;z-index:6;display:flex;flex-direction:column;align-items:center;
  justify-content:center;gap:12px;padding:20px;background:#0B0D14F5;backdrop-filter:blur(9px);
  text-align:center;overflow-y:auto}
.screen.hide{display:none}
h1{font-family:"Bricolage Grotesque",sans-serif;font-weight:800;font-size:clamp(46px,15vw,84px);
  line-height:.84;letter-spacing:-.05em;text-transform:uppercase}
h1 em{font-style:normal;color:var(--red)}
.kicker{font-size:9px;letter-spacing:.3em;text-transform:uppercase;color:var(--dim)}
.rules{font-size:11.5px;line-height:1.75;color:#AFB6C8;max-width:330px}
.rules b{color:var(--pale);font-weight:700}
button{font:inherit;font-size:13px;font-weight:700;letter-spacing:.12em;text-transform:uppercase;
  color:var(--pale);background:#FFFFFF0E;border:1px solid var(--line);border-radius:10px;
  padding:14px 12px;cursor:pointer;width:100%;max-width:330px}
button:active{transform:scale(.98)}
.go{background:var(--red);border-color:var(--red);color:#180608;font-size:16px;padding:16px}
#threat{border:1px solid #E8574C55;background:#E8574C12;border-radius:10px;padding:9px 13px;max-width:330px}
#threat .t1{font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--red)}
#threat .t2{font-family:"Bricolage Grotesque",sans-serif;font-size:17px;margin-top:2px}
#threat .t3{font-size:10.5px;color:#AFB6C8;margin-top:3px;line-height:1.4}
#cards{display:flex;flex-direction:column;gap:8px;width:100%;max-width:330px}
#rig{display:flex;flex-direction:column;gap:5px;width:100%;max-width:330px}
.rigrow{display:flex;justify-content:space-between;align-items:center;gap:8px;
  border:1px solid var(--line);border-radius:8px;padding:7px 10px;font-size:11px}
.rigrow.anc{border-color:#5B9BD588;background:#5B9BD514}
.rigrow .rn{font-weight:700}
.rigrow .rt{font-size:9px;letter-spacing:.14em;text-transform:uppercase;color:var(--dim)}
.rigrow .rt.inf{color:var(--blue)}
.ancbtn{font-size:9px;letter-spacing:.14em;text-transform:uppercase;font-weight:700;
  color:var(--gold);border:1px solid #F2B33D66;border-radius:6px;padding:5px 9px;white-space:nowrap}
.ancbtn:active{background:#F2B33D33}
.card{border:1px solid var(--line);background:#FFFFFF08;border-radius:11px;padding:11px 13px;text-align:left}
.card:active{background:#FFFFFF14}
.card.up{border-color:#F2B33D88;background:#F2B33D12}
.card .n{font-weight:700;font-size:13.5px;display:flex;justify-content:space-between;align-items:center}
.card .n em{font-style:normal;font-size:8.5px;letter-spacing:.14em;text-transform:uppercase;color:var(--gold)}
.card .d{font-size:11px;color:#AFB6C8;margin-top:3px;line-height:1.45}
#endN{font-family:"Bricolage Grotesque",sans-serif;font-size:64px;line-height:1;letter-spacing:-.04em}
#rot{position:fixed;inset:0;z-index:9;display:none;flex-direction:column;align-items:center;justify-content:center;
  gap:16px;background:var(--bg);text-align:center;padding:28px}
#rot.show{display:flex}
#rot .ph{width:52px;height:88px;border:3px solid var(--pale);border-radius:11px;animation:tn 2.4s ease-in-out infinite}
@keyframes tn{0%,28%{transform:rotate(0)}55%,100%{transform:rotate(-90deg)}}
#err{position:fixed;left:0;right:0;bottom:0;z-index:12;background:#7A0C18;color:#fff;font-size:10px;
  padding:7px 11px;display:none;font-family:ui-monospace,monospace}
</style>
</head>
<body>

<div id="hud">
  <div id="top">
    <div id="waveRow">
      <div><div class="tag">Course</div><div id="waveN">1</div></div>
      <div style="text-align:right"><div class="tag">On the field</div><div id="left">0</div></div>
    </div>
    <div id="towers"><div class="tw"><i></i></div><div class="tw"><i></i></div><div class="tw"><i></i></div></div>
  </div>
  <div id="perks"></div>
  <div id="hpWrap"><div class="tag">Chef</div><div id="hpBar"><i></i></div></div>
  <div id="stickZone"></div>
  <div id="msg"></div>
</div>

<div class="screen" id="title">
  <div class="kicker">The vegetables have had enough</div>
  <h1>Salad<em>Days</em></h1>
  <div class="rules">
    <b>Drag anywhere</b> to move. You fire constantly, in whatever direction you're facing — so movement is aiming.<br>
    Protect the <b>three diners</b>. Let one get eaten and the veg start crawling out from under the chair.<br>
    Every wave you take <b>one power from three</b>. You can only run <b>five at once</b>, and each one <b>burns out after five waves</b>.<br>
    Levelling a power resets its clock — so keeping a favourite alive means passing on something new.<br>
    You start with <b>five slots and two anchors</b>. An anchored power never expires.<br>
    You earn <b>+1 slot every 5 waves</b> and <b>+1 anchor every 10</b> — so survive long enough and the rig grows with you.
  </div>
  <button class="go" id="startBtn">Begin</button>
</div>

<div class="screen hide" id="draft">
  <div id="threat"><div class="t1">Incoming</div><div class="t2" id="thName">—</div><div class="t3" id="thDesc">—</div></div>
  <div class="kicker" id="slotLine">Choose one</div>
  <div id="cards"></div>
  <div class="kicker" id="anchorLine" style="margin-top:4px">Anchors</div>
  <div id="rig"></div>
</div>

<div class="screen hide" id="swap">
  <div class="kicker">Kit is full — drop one to make room</div>
  <div class="kicker" id="pendName" style="color:var(--gold);font-size:12px;letter-spacing:.1em"></div>
  <div id="swapCards" style="display:flex;flex-direction:column;gap:8px;width:100%;max-width:330px"></div>
</div>

<div class="screen hide" id="over">
  <div class="kicker" id="endWhy">They ate everyone</div>
  <div id="endN">0</div>
  <div class="kicker">courses served · best <span id="endBest">0</span></div>
  <button class="go" id="againBtn">Again</button>
</div>

<div id="rot"><div class="ph"></div><div style="font-family:'Bricolage Grotesque';font-size:24px;text-transform:uppercase">Hold it upright</div><div class="kicker">Salad Days is played in portrait</div></div>
<div id="err"></div>

<script>
let _lastTap=0;
document.addEventListener('touchend',e=>{
  const now=Date.now();
  if(now-_lastTap<360) e.preventDefault();     // kills double-tap-to-zoom
  _lastTap=now;
},{passive:false});
['gesturestart','gesturechange','gestureend'].forEach(g=>
  document.addEventListener(g,e=>e.preventDefault(),{passive:false}));
document.addEventListener('dblclick',e=>e.preventDefault(),{passive:false});

window.onerror=function(m,s,l){var e=document.getElementById('err');
  e.style.display='block'; e.textContent='ERROR: '+m+' ('+l+')';};
const $=id=>document.getElementById(id);
const clamp=(v,a,b)=>Math.max(a,Math.min(b,v));
const rnd=(a,b)=>a+Math.random()*(b-a);
const TAU=Math.PI*2;

/* ================= canvas ================= */
const cv=document.createElement('canvas'); document.body.appendChild(cv);
const ctx=cv.getContext('2d');
let W=0,H=0,DPR=1;
function resize(){
  DPR=Math.min(devicePixelRatio,2); W=innerWidth; H=innerHeight;
  cv.width=W*DPR; cv.height=H*DPR; cv.style.width=W+'px'; cv.style.height=H+'px';
  ctx.setTransform(DPR,0,0,DPR,0,0);
  if(G) placeTowers();
}

/* ================= audio ================= */
let AC=null;
function aInit(){ if(AC) return; try{ AC=new (window.AudioContext||window.webkitAudioContext)(); }catch(e){} }
function blip(hz,dur,vol,type){
  if(!AC) return;
  const o=AC.createOscillator(), g=AC.createGain();
  o.type=type||'square'; o.frequency.value=hz; g.gain.value=vol;
  g.gain.exponentialRampToValueAtTime(.0001,AC.currentTime+dur);
  o.connect(g); g.connect(AC.destination); o.start(); o.stop(AC.currentTime+dur);
}
function boom(dur,freq,vol){
  if(!AC) return;
  const len=Math.floor(AC.sampleRate*dur), buf=AC.createBuffer(1,len,AC.sampleRate), d=buf.getChannelData(0);
  for(let i=0;i<len;i++) d[i]=(Math.random()*2-1)*(1-i/len);
  const n=AC.createBufferSource(); n.buffer=buf;
  const f=AC.createBiquadFilter(); f.type='lowpass'; f.frequency.value=freq;
  const g=AC.createGain(); g.gain.value=vol;
  g.gain.exponentialRampToValueAtTime(.0001,AC.currentTime+dur);
  n.connect(f); f.connect(g); g.connect(AC.destination); n.start();
}
const buzz=p=>{ try{navigator.vibrate&&navigator.vibrate(p);}catch(e){} };

/* ================= powers ================= */
const BASE={
  dmg:11, count:1, spread:.12, bounce:0, pierce:0, explode:0, blast:56,
  fireCd:.30, bspeed:560, bsize:4.2, homing:0, crit:0, splitBounce:0,
  aura:0, auraR:78, orbit:0, thorns:0, shockwave:0,
  maxhp:100, speed:178, regen:0, lifesteal:0, slow:0,
  towerDmg:9, towerRange:200, towerCd:.85, towerHpMul:1, chain:0
};
const POWERS=[
  {id:'twin',   n:'Twin Grinders',    d:'+1 bullet per shot. Spread widens a touch.',      f:(S,l)=>{S.count+=l; S.spread+=.05*l;}},
  {id:'scatter',n:'Peppercorn Spray',    d:'+3 bullets in a wide fan. Hard to miss, weaker per pellet.', f:(S,l)=>{S.count+=3*l; S.spread+=.30*l; S.dmg-=2*l;}},
  {id:'punch',  n:'Rock Salt',   d:'+6 damage per bullet, per level.',                f:(S,l)=>{S.dmg+=6*l;}},
  {id:'rate',   n:'Fast Hands',  d:'Fire 18% faster per level.',                      f:(S,l)=>{S.fireCd*=Math.pow(.82,l);}},
  {id:'bounce', n:'Bank Shot',       d:'Bullets ricochet off walls AND off enemies, +1 bounce per level. Each ricochet seeks a new target.', f:(S,l)=>{S.bounce+=l;}},
  {id:'pierce', n:'Skewer',  d:'Bullets pass through +1 enemy per level.',        f:(S,l)=>{S.pierce+=l;}},
  {id:'boom',   n:'Popping Kernels',d:'Rounds pop like corn on impact. Bigger blast each level.',f:(S,l)=>{S.explode=1; S.blast+=24*(l-1);}},
  {id:'split',  n:'Splatter',    d:'Every bounce splits the bullet in two.',          f:(S,l)=>{S.splitBounce+=l;}},
  {id:'home',   n:'Homing Seeds',  d:'Bullets curve toward enemies.',                   f:(S,l)=>{S.homing+=1.9*l;}},
  {id:'crit',   n:'Sharp Knife',       d:'18% chance per level for a bullet to hit triple.', f:(S,l)=>{S.crit+=.18*l;}},
  {id:'vel',    n:'Searing Heat',      d:'Bullets fly 25% faster and hit slightly harder.', f:(S,l)=>{S.bspeed*=1+.25*l; S.dmg+=2*l;}},
  {id:'big',    n:'Meatballs',    d:'Much bigger bullets, +4 damage.',                 f:(S,l)=>{S.bsize+=2.2*l; S.dmg+=4*l;}},
  {id:'aura',   n:'Blender',      d:'A blender strapped to your back. Purees anything close.',        f:(S,l)=>{S.aura+=26*l;}},
  {id:'auraR',  n:'Wide Blades',     d:'Blender radius +38%. Needs the Blender to matter.',f:(S,l)=>{S.auraR*=1+.38*l;}},
  {id:'orbit',  n:'Rolling Pins',       d:'+1 blade circling you, shredding what it touches.',f:(S,l)=>{S.orbit+=l;}},
  {id:'shock',  n:'Pan Slam',      d:'Every reload knocks back and damages nearby.',    f:(S,l)=>{S.shockwave+=1*l;}},
  {id:'thorn',  n:'Cheese Grater',   d:'Anything that bumps into you gets shredded.',   f:(S,l)=>{S.thorns+=34*l;}},
  {id:'hp',     n:'Big Appetite',     d:'+35 max health, and heal that much now.',         f:(S,l)=>{S.maxhp+=35*l;}},
  {id:'spd',    n:'Non-Slip Shoes',    d:'+16% movement speed.',                            f:(S,l)=>{S.speed*=1+.16*l;}},
  {id:'regen',  n:'Hot Soup',      d:'Regenerate 3 health per second, per level.',      f:(S,l)=>{S.regen+=3*l;}},
  {id:'leech',  n:'Juicer',         d:'Heal 4% of the damage you deal.',                 f:(S,l)=>{S.lifesteal+=.04*l;}},
  {id:'slow',   n:'Syrup Rounds',     d:'Hits slow enemies by 22% for a moment.',          f:(S,l)=>{S.slow+=.22*l;}},
  {id:'twdmg',  n:'Give Them Forks',     d:'Diners fight back harder — +7 damage, 12% faster.',      f:(S,l)=>{S.towerDmg+=7*l; S.towerCd*=Math.pow(.88,l);}},
  {id:'twrng',  n:'Reading Glasses',       d:'Diners spot them sooner. +30% range.',                               f:(S,l)=>{S.towerRange*=1+.30*l;}},
  {id:'twhp',   n:'Second Helping',      d:'Diners get +40% health and tuck in right now.',f:(S,l)=>{S.towerHpMul+=.40*l;}},
  {id:'chain',  n:'Pass The Salt',      d:'Diner shots chain to +1 extra vegetable.',            f:(S,l)=>{S.chain+=l;}}
];
const byId=id=>POWERS.find(p=>p.id===id);
const SLOTS=5, LIFE=5, ANCHORS=2;
/* the rig grows: +1 slot every 5 waves, +1 permanent anchor every 15 */
const slotCap  =()=>SLOTS  +Math.floor(G.wave/5);
const anchorCap=()=>ANCHORS+Math.floor(G.wave/10);
const onScreen=e=>e.x>10&&e.x<W-10&&e.y>10&&e.y<H-10;
const anchorsLeft=()=>anchorCap()-G.anchorsUsed;

/* ================= enemies ================= */
const TYPES={
  rusher: {cost:1,  hp:16,  spd:118, r:7,  dmg:6,  col:'#7FC24B', out:'#CFF0A0'},
  grunt:  {cost:2,  hp:34,  spd:74,  r:9,  dmg:10, col:'#E8862E', out:'#FFC98E'},
  tank:   {cost:7,  hp:180, spd:38,  r:16, dmg:22, col:'#3E7A34', out:'#8FD86B'},
  ranged: {cost:4,  hp:28,  spd:56,  r:8,  dmg:8,  col:'#C4342A', out:'#FF8B72', shoots:1, range:210},
  splitter:{cost:4, hp:44,  spd:66,  r:11, dmg:10, col:'#E2503B', out:'#FF9C86', splits:2},
  bomber: {cost:5,  hp:30,  spd:104, r:10, dmg:38, col:'#E7D6B8', out:'#FFF3DC', suicide:1, towerOnly:1},
  hive:   {cost:11, hp:150, spd:26,  r:15, dmg:12, col:'#F0C33C', out:'#FFE894', spawns:1}
};
const MODS={
  armored:{n:'Pickled',  d:'takes 45% less damage',   mul:2.0, f:e=>{e.armor=.55;}},
  hasted: {n:'Fresh',    d:'moves 55% faster',        mul:1.7, f:e=>{e.spd*=1.55;}},
  volatile:{n:'Overripe',d:'bursts when it dies',   mul:1.6, f:e=>{e.volatile=1;}},
  vast:   {n:'Jumbo',    d:'double health',           mul:1.9, f:e=>{e.hp*=2; e.maxhp*=2; e.r*=1.2;}}
};
function unlocked(wave){
  const l=['rusher'];
  if(wave>=2) l.push('grunt');
  if(wave>=4) l.push('ranged');
  if(wave>=5) l.push('splitter');
  if(wave>=6) l.push('bomber');
  if(wave>=8) l.push('tank');
  if(wave>=11) l.push('hive');
  return l;
}

/* ================= state ================= */
let G=null, running=false, best=0;
try{ best=parseInt(localStorage.getItem('salad:best')||'0')||0; }catch(e){}

function placeTowers(){
  if(!G) return;
  const pts=[[W*0.22,H*0.52],[W*0.78,H*0.52],[W*0.50,H*0.80]];
  G.towers.forEach((t,i)=>{ t.x=pts[i][0]; t.y=pts[i][1]; });
}
function newGame(){
  G={ wave:0, S:Object.assign({},BASE), owned:{}, anchorsUsed:0,
      player:{x:W/2,y:H*0.68,a:-Math.PI/2,hp:100,fireT:0,orbA:0,shockT:0,inv:0},
      enemies:[], bullets:[], ebullets:[], parts:[], rings:[],
      towers:[0,1,2].map(i=>({x:0,y:0,hp:260,max:260,alive:true,cd:0})),
      shake:0, budget:9, lastClear:0, waveT:0, spawnQ:[], spawnT:0, threat:null, over:false };
  placeTowers(); recalc(true); paintPerks(); paintTowers();
}
function recalc(full){
  const S=Object.assign({},BASE);
  for(const id in G.owned) byId(id).f(S,G.owned[id].l);
  const oldMax=G.S?G.S.maxhp:S.maxhp;
  G.S=S;
  G.towers.forEach(t=>{ const nm=260*S.towerHpMul; if(nm>t.max){ t.hp+=nm-t.max; } t.max=nm; });
  if(full) G.player.hp=S.maxhp;
  else G.player.hp=Math.min(S.maxhp,G.player.hp+Math.max(0,S.maxhp-oldMax));
}
function paintPerks(){
  $('perks').innerHTML=Object.keys(G.owned).map(id=>{
    const p=byId(id), o=G.owned[id];
    const cls = o.a ? 'perk anchored' : (o.t<=1 ? 'perk dying' : 'perk');
    return `<div class="${cls}">${p.n}${o.l>1?' '+o.l:''} <b>${o.a?'\u221e':o.t+'w'}</b></div>`;
  }).join('');
}
/* every draft, the clock ticks and anything at zero falls off your rig */
function expireTick(){
  const gone=[];
  for(const id in G.owned){
    if(G.owned[id].a) continue;                 // anchored: no clock
    G.owned[id].t--;
    if(G.owned[id].t<=0){ gone.push(byId(id).n); delete G.owned[id]; }
  }
  if(gone.length){ recalc(false); paintPerks(); }
  return gone;
}
function paintTowers(){
  const els=document.querySelectorAll('#towers .tw');
  G.towers.forEach((t,i)=>{
    els[i].classList.toggle('dead',!t.alive);
    els[i].firstElementChild.style.width=Math.max(0,t.hp/t.max*100)+'%';
  });
}
let msgT=0;
function say(t){ const m=$('msg'); m.textContent=t; m.style.opacity=1; msgT=1.1; }

/* ================= wave building ================= */
function buildWave(){
  G.wave++;
  const w=G.wave;
  // budget grows, then flexes against how the player actually did
  let growth=1.28;
  if(w>1){
    if(G.lastClear<14 && G.towerDmgTaken<40) growth=1.42;      // crushed it
    else if(G.towerDmgTaken>180) growth=1.10;                   // nearly lost a tower
  }
  G.budget=w===1?9:G.budget*growth;
  G.towerDmgTaken=0;

  // one visible threat modifier from wave 3 on, two from wave 12
  const keys=Object.keys(MODS);
  const nMods=w<3?0:(w<12?1:2);
  const picked=[];
  while(picked.length<nMods){
    const k=keys[Math.floor(Math.random()*keys.length)];
    if(picked.indexOf(k)<0) picked.push(k);
  }
  G.threat=picked;
  const avail=unlocked(w);
  let budget=G.budget, q=[];
  let guard=0;
  while(budget>0 && guard++<900){
    const t=avail[Math.floor(Math.random()*avail.length)];
    let cost=TYPES[t].cost;
    const useMod = picked.length && Math.random()<.55 ? picked[Math.floor(Math.random()*picked.length)] : null;
    if(useMod) cost*=MODS[useMod].mul;
    if(cost>budget){ if(TYPES[t].cost>budget) continue; }
    budget-=cost;
    q.push({t,mod:useMod});
  }
  G.spawnQ=q.sort(()=>Math.random()-.5);
  G.waveT=0; G.spawnT=0;
  $('waveN').textContent=w;
  $('thName').textContent = picked.length ? picked.map(k=>MODS[k].n).join(' + ') : 'Unmodified';
  $('thDesc').textContent = picked.length ? picked.map(k=>MODS[k].d).join(' · ')
    : 'Nothing special. Enjoy it.';
}
function spawnPoints(){
  const pts=[];
  for(const t of G.towers) if(!t.alive) pts.push({x:t.x,y:t.y,ruin:1});   // fallen towers leak enemies
  pts.push({x:rnd(20,W-20),y:-24});
  if(G.wave>=6) pts.push({x:-24,y:rnd(H*.15,H*.6)},{x:W+24,y:rnd(H*.15,H*.6)});
  return pts;
}
function spawnOne(spec){
  const T=TYPES[spec.t], pts=spawnPoints();
  const p=pts[Math.floor(Math.random()*pts.length)];
  const scale=1+G.wave*0.045;                       // HP creeps, damage barely moves
  const e={ t:spec.t, x:p.x+rnd(-14,14), y:p.y+rnd(-14,14),
    hp:T.hp*scale, maxhp:T.hp*scale, spd:T.spd, r:T.r, dmg:T.dmg*(1+G.wave*0.012),
    col:T.col, out:T.out, armor:0, volatile:0, hit:0, slowT:0, cd:rnd(0,1.2),
    shoots:T.shoots||0, range:T.range||0, splits:T.splits||0, suicide:T.suicide||0,
    towerOnly:T.towerOnly||0, spawns:T.spawns||0, target:null };
  if(spec.mod) MODS[spec.mod].f(e);
  G.enemies.push(e);
}

/* ================= input ================= */
const stick={active:false,ox:0,oy:0,x:0,y:0,id:null};
$('stickZone').addEventListener('pointerdown',e=>{
  stick.active=true; stick.id=e.pointerId; stick.ox=e.clientX; stick.oy=e.clientY;
  stick.x=0; stick.y=0;
});
addEventListener('pointermove',e=>{
  if(stick.active&&e.pointerId===stick.id){
    let dx=e.clientX-stick.ox, dy=e.clientY-stick.oy;
    const d=Math.hypot(dx,dy), max=52;
    if(d>max){ dx=dx/d*max; dy=dy/d*max; }
    stick.x=dx/max; stick.y=dy/max;
  }
});
addEventListener('pointerup',e=>{ if(e.pointerId===stick.id){ stick.active=false; stick.x=0; stick.y=0; } });
addEventListener('pointercancel',()=>{ stick.active=false; stick.x=0; stick.y=0; });

function tryFire(){
  if(!running||!G||G.over) return;
  const P=G.player, S=G.S;
  if(P.fireT>0) return;
  P.fireT=S.fireCd;
  // nudge toward anything already close to your facing — invisible, but it's why you hit
  let aim=P.a, bestDa=null, bd=1e9;
  for(const e of G.enemies){
    if(e.dead) continue;
    const d=Math.hypot(e.x-P.x,e.y-P.y);
    if(d>440) continue;
    let da=Math.atan2(e.y-P.y,e.x-P.x)-P.a;
    while(da>Math.PI)da-=TAU; while(da<-Math.PI)da+=TAU;
    if(Math.abs(da)<.45&&d<bd){ bd=d; bestDa=da; }
  }
  if(bestDa!==null) aim=P.a+clamp(bestDa,-.24,.24);
  const n=S.count;
  for(let i=0;i<n;i++){
    const off=(n===1)?0:(i-(n-1)/2)*S.spread;
    const a=aim+off+rnd(-.02,.02);
    G.bullets.push({x:P.x+Math.cos(a)*16,y:P.y+Math.sin(a)*16,
      vx:Math.cos(a)*S.bspeed, vy:Math.sin(a)*S.bspeed,
      dmg:S.dmg*(Math.random()<S.crit?3:1), b:S.bounce, p:S.pierce, life:2.2, hitList:[]});
  }
  blip(430,.05,.05,'square');
  G.shake=Math.max(G.shake,2);
  if(S.shockwave>0){                                 // reload knocks the crowd back
    P.shockT=.12;
    G.rings.push({x:P.x,y:P.y,r:10,max:120,col:'#8FD3F2'});
    for(const e of G.enemies){
      const d=Math.hypot(e.x-P.x,e.y-P.y);
      if(d<120){ hurt(e,16*S.shockwave); const a=Math.atan2(e.y-P.y,e.x-P.x);
        e.x+=Math.cos(a)*26; e.y+=Math.sin(a)*26; }
    }
  }
}

/* ================= combat helpers ================= */
function hurt(e,dmg){
  const d=dmg*(1-(e.armor||0));
  e.hp-=d; e.hit=.09;
  if(G.S.lifesteal) G.player.hp=Math.min(G.S.maxhp,G.player.hp+d*G.S.lifesteal);
  if(e.hp<=0) kill(e);
}
function kill(e){
  if(e.dead) return;
  e.dead=true;
  for(let i=0;i<5;i++) G.parts.push({x:e.x,y:e.y,vx:rnd(-90,90),vy:rnd(-90,90),life:.4,col:e.col});
  if(e.volatile){ explode(e.x,e.y,64,26,'#FF9A90'); }
  if(e.splits){
    for(let i=0;i<e.splits;i++){
      const T=TYPES.rusher, scale=1+G.wave*0.045;
      G.enemies.push({t:'rusher',x:e.x+rnd(-10,10),y:e.y+rnd(-10,10),
        hp:T.hp*scale*.7,maxhp:T.hp*scale*.7,spd:T.spd*1.15,r:5.5,dmg:T.dmg,
        col:'#E2503B',out:'#FF9C86',armor:e.armor,volatile:0,hit:0,slowT:0,cd:0,
        shoots:0,range:0,splits:0,suicide:0,towerOnly:0,spawns:0});
    }
  }
}
function explode(x,y,r,dmg,col){
  G.rings.push({x,y,r:6,max:r,col:col||'#FFC24B'});
  boom(.22,700,.16); G.shake=Math.max(G.shake,6);
  for(const e of G.enemies){
    if(e.dead) continue;
    const d=Math.hypot(e.x-x,e.y-y);
    if(d<r) hurt(e,dmg*(1-d/r*.5));
  }
}

/* ================= step ================= */
function step(dt){
  const P=G.player, S=G.S;
  G.waveT+=dt;

  /* spawn drip */
  if(G.spawnQ.length){
    G.spawnT-=dt;
    if(G.spawnT<=0){
      const burst=1+Math.floor(G.wave/4);
      for(let i=0;i<burst&&G.spawnQ.length;i++) spawnOne(G.spawnQ.pop());
      G.spawnT=Math.max(.12,.62-G.wave*.02);
    }
  }

  /* player */
  const sp=Math.hypot(stick.x,stick.y);
  if(sp>.12){
    P.a=Math.atan2(stick.y,stick.x);
    P.x=clamp(P.x+stick.x*S.speed*dt,14,W-14);
    P.y=clamp(P.y+stick.y*S.speed*dt,14,H-14);
  }
  if(P.fireT>0) P.fireT-=dt;
  tryFire();                              // the gun never stops
  if(S.regen) P.hp=Math.min(S.maxhp,P.hp+S.regen*dt);
  if(P.inv>0) P.inv-=dt;
  P.orbA+=dt*2.6;

  /* aura + orbiters */
  if(S.aura>0||S.orbit>0){
    for(const e of G.enemies){
      if(e.dead) continue;
      const d=Math.hypot(e.x-P.x,e.y-P.y);
      if(S.aura>0&&d<S.auraR) hurt(e,S.aura*dt);
      if(S.orbit>0){
        for(let i=0;i<S.orbit;i++){
          const a=P.orbA+i*TAU/S.orbit;
          const ox=P.x+Math.cos(a)*66, oy=P.y+Math.sin(a)*66;
          if(Math.hypot(e.x-ox,e.y-oy)<e.r+9) hurt(e,120*dt);
        }
      }
    }
  }

  /* bullets */
  for(const b of G.bullets){
    if(b.dead) continue;
    b.life-=dt;
    if(S.homing){
      let best=null,bd=1e9;
      for(const e of G.enemies){ if(e.dead) continue;
        const d=(e.x-b.x)**2+(e.y-b.y)**2; if(d<bd&&d<220*220){bd=d;best=e;} }
      if(best){
        const a=Math.atan2(best.y-b.y,best.x-b.x), ca=Math.atan2(b.vy,b.vx);
        let da=a-ca; while(da>Math.PI)da-=TAU; while(da<-Math.PI)da+=TAU;
        const na=ca+clamp(da,-S.homing*dt,S.homing*dt), sp2=Math.hypot(b.vx,b.vy);
        b.vx=Math.cos(na)*sp2; b.vy=Math.sin(na)*sp2;
      }
    }
    b.x+=b.vx*dt; b.y+=b.vy*dt;
    let bounced=false;
    if(b.x<4||b.x>W-4){ if(b.b>0){ b.vx*=-1; b.b--; bounced=true; b.x=clamp(b.x,5,W-5); } else b.dead=true; }
    if(b.y<4||b.y>H-4){ if(b.b>0){ b.vy*=-1; b.b--; bounced=true; b.y=clamp(b.y,5,H-5); } else b.dead=true; }
    if(bounced&&S.splitBounce&&!b.noSplit){
      for(let i=0;i<S.splitBounce;i++){
        const a=Math.atan2(b.vy,b.vx)+rnd(-.8,.8), sp2=Math.hypot(b.vx,b.vy);
        G.bullets.push({x:b.x,y:b.y,vx:Math.cos(a)*sp2,vy:Math.sin(a)*sp2,
          dmg:b.dmg*.62,b:Math.max(0,b.b-1),p:b.p,life:1.4,hitList:[],noSplit:1});
      }
    }
    if(b.life<=0) b.dead=true;
    if(b.dead) continue;
    for(const e of G.enemies){
      if(e.dead||b.dead) continue;
      if(b.hitList.indexOf(e)>=0) continue;
      if(Math.hypot(e.x-b.x,e.y-b.y)<e.r+S.bsize+3){        // a touch more forgiving
        hurt(e,b.dmg);
        if(S.slow){ e.slowT=.9; }
        if(S.explode) explode(b.x,b.y,S.blast,b.dmg*.55);
        b.hitList.push(e);
        if(b.p>0){ b.p--; }
        else if(b.b>0){                                     // ricochet off the body
          b.b--;
          let nx=null,nd=1e9;
          for(const o of G.enemies){
            if(o.dead||o===e||b.hitList.indexOf(o)>=0) continue;
            const d2=Math.hypot(o.x-b.x,o.y-b.y);
            if(d2<300&&d2<nd){ nd=d2; nx=o; }
          }
          const sp2=Math.hypot(b.vx,b.vy);
          let na;
          if(nx) na=Math.atan2(nx.y-b.y,nx.x-b.x);           // seek the next one
          else   na=Math.atan2(b.vy,b.vx)+Math.PI+rnd(-.7,.7);
          b.vx=Math.cos(na)*sp2; b.vy=Math.sin(na)*sp2;
          b.dmg*=.85;
          if(S.splitBounce&&!b.noSplit){
            for(let k=0;k<S.splitBounce;k++){
              const a2=na+rnd(-.9,.9);
              G.bullets.push({x:b.x,y:b.y,vx:Math.cos(a2)*sp2,vy:Math.sin(a2)*sp2,
                dmg:b.dmg*.62,b:Math.max(0,b.b-1),p:b.p,life:1.4,hitList:[e],noSplit:1});
            }
          }
        }
        else b.dead=true;
        break;
      }
    }
  }
  G.bullets=G.bullets.filter(b=>!b.dead);
  if(G.bullets.length>700) G.bullets.splice(0,G.bullets.length-700);

  /* enemies */
  for(const e of G.enemies){
    if(e.dead) continue;
    if(e.hit>0) e.hit-=dt;
    if(e.slowT>0) e.slowT-=dt;
    // pick a target: bombers only ever want towers
    let tx,ty,isTower=false;
    const live=G.towers.filter(t=>t.alive);
    let bt=null,bd=1e9;
    for(const t of live){ const d=(t.x-e.x)**2+(t.y-e.y)**2; if(d<bd){bd=d;bt=t;} }
    const pd=Math.hypot(P.x-e.x,P.y-e.y);
    if(e.towerOnly&&bt){ tx=bt.x; ty=bt.y; isTower=true; }
    else if(!bt || pd<150){ tx=P.x; ty=P.y; }
    else { tx=bt.x; ty=bt.y; isTower=true; }

    const dx=tx-e.x, dy=ty-e.y, d=Math.hypot(dx,dy)||1;
    const spd=e.spd*(e.slowT>0?(1-S.slow):1);
    // a shooter off the edge keeps walking in — it only sets up once you can see it
    const stopAt=(e.shoots&&onScreen(e))?e.range:(isTower?26:e.r+13);
    if(d>stopAt){ e.x+=dx/d*spd*dt; e.y+=dy/d*spd*dt; }
    else {
      e.cd-=dt;
      if(e.shoots){
        if(e.cd<=0&&onScreen(e)){ e.cd=1.5;
          const a=Math.atan2(dy,dx);
          G.ebullets.push({x:e.x,y:e.y,vx:Math.cos(a)*210,vy:Math.sin(a)*210,dmg:e.dmg,life:3,tw:isTower?bt:null});
        }
      } else if(e.suicide){
        explode(e.x,e.y,74,0,'#FF9CBC');
        if(isTower&&bt){ bt.hp-=e.dmg; G.towerDmgTaken+=e.dmg; }
        if(Math.hypot(P.x-e.x,P.y-e.y)<74&&P.inv<=0){ P.hp-=e.dmg*.6; P.inv=.35; G.shake=10; }
        kill(e); continue;
      } else if(e.cd<=0){
        e.cd=.75;
        if(isTower&&bt){ bt.hp-=e.dmg; G.towerDmgTaken+=e.dmg; G.shake=Math.max(G.shake,3); }
        else if(P.inv<=0){ P.hp-=e.dmg; P.inv=.28; G.shake=6; buzz(25);
          if(S.thorns) hurt(e,S.thorns); }
      }
    }
    if(e.spawns){
      e.sp=(e.sp||0)-dt;
      if(e.sp<=0){ e.sp=2.2;
        const T=TYPES.rusher, sc=1+G.wave*.045;
        G.enemies.push({t:'rusher',x:e.x+rnd(-16,16),y:e.y+rnd(-16,16),hp:T.hp*sc,maxhp:T.hp*sc,
          spd:T.spd,r:6.5,dmg:T.dmg,col:'#F0C33C',out:'#FFE894',armor:0,volatile:0,hit:0,slowT:0,cd:0,
          shoots:0,range:0,splits:0,suicide:0,towerOnly:0,spawns:0});
      }
    }
    // soft separation keeps the horde a horde, not one dot
    for(const o of G.enemies){
      if(o===e||o.dead) continue;
      const ox=e.x-o.x, oy=e.y-o.y, od=Math.hypot(ox,oy);
      const want=e.r+o.r;
      if(od>0.01&&od<want){ e.x+=ox/od*(want-od)*.5; e.y+=oy/od*(want-od)*.5; }
    }
  }
  G.enemies=G.enemies.filter(e=>!e.dead);

  /* enemy bullets */
  for(const b of G.ebullets){
    b.life-=dt; b.x+=b.vx*dt; b.y+=b.vy*dt;
    if(b.life<=0){ b.dead=true; continue; }
    if(Math.hypot(P.x-b.x,P.y-b.y)<12&&P.inv<=0){ P.hp-=b.dmg; P.inv=.25; b.dead=true; G.shake=5; buzz(20); }
    for(const t of G.towers){
      if(!t.alive) continue;
      if(Math.hypot(t.x-b.x,t.y-b.y)<22){ t.hp-=b.dmg; G.towerDmgTaken+=b.dmg; b.dead=true; }
    }
  }
  G.ebullets=G.ebullets.filter(b=>!b.dead);

  /* towers shoot */
  for(const t of G.towers){
    if(!t.alive) continue;
    t.cd-=dt;
    if(t.cd<=0){
      let best=null,bd=1e9;
      for(const e of G.enemies){ if(e.dead) continue;
        const d=Math.hypot(e.x-t.x,e.y-t.y); if(d<S.towerRange&&d<bd){bd=d;best=e;} }
      if(best){
        t.cd=S.towerCd;
        hurt(best,S.towerDmg);
        G.rings.push({x:t.x,y:t.y,r:4,max:14,col:'#5B9BD5',fast:1,to:{x:best.x,y:best.y}});
        let last=best;
        for(let c=0;c<S.chain;c++){
          let n=null,nd=1e9;
          for(const e of G.enemies){ if(e.dead||e===last) continue;
            const d=Math.hypot(e.x-last.x,e.y-last.y); if(d<110&&d<nd){nd=d;n=e;} }
          if(!n) break;
          hurt(n,S.towerDmg*.7);
          G.rings.push({x:last.x,y:last.y,r:4,max:10,col:'#8FD3F2',fast:1,to:{x:n.x,y:n.y}});
          last=n;
        }
      }
    }
    if(t.hp<=0){ t.alive=false; t.hp=0; explode(t.x,t.y,120,0,'#E8574C');
      say('they got one'); buzz([60,40,120]); G.shake=14; }
  }
  paintTowers();

  /* particles */
  for(const p of G.parts){ p.life-=dt; p.x+=p.vx*dt; p.y+=p.vy*dt; p.vx*=.94; p.vy*=.94; }
  G.parts=G.parts.filter(p=>p.life>0);
  for(const r of G.rings){ r.r+=(r.max-r.r)*(r.fast?.5:.16); }
  G.rings=G.rings.filter(r=>r.max-r.r>1.2);

  if(G.shake>0) G.shake=Math.max(0,G.shake-dt*26);

  /* end conditions */
  if(P.hp<=0 || G.towers.every(t=>!t.alive)) endRun();
  if(!G.spawnQ.length && !G.enemies.length && !G.over){
    G.lastClear=G.waveT;
    running=false; openDraft();
  }
  $('left').textContent=G.enemies.length+G.spawnQ.length;
  $('hpBar').firstElementChild.style.width=clamp(P.hp/S.maxhp*100,0,100)+'%';
}

/* ================= draw ================= */
let TT=0;
function box(x,y,w,h,r){
  if(ctx.roundRect){ ctx.beginPath(); ctx.roundRect(x,y,w,h,r); }
  else { ctx.beginPath(); ctx.rect(x,y,w,h); }
}
function leafy(x,y,r,col,n,ph){
  ctx.fillStyle=col;
  for(let i=0;i<n;i++){
    const a=ph+i*TAU/n;
    ctx.beginPath();
    ctx.ellipse(x+Math.cos(a)*r*.55,y+Math.sin(a)*r*.55,r*.62,r*.5,a,0,TAU);
    ctx.fill();
  }
}
function drawVeg(e){
  ctx.save(); ctx.translate(e.x,e.y); ctx.rotate(Math.sin(TT*6+e.x*.05)*.10);
  const r=e.r;
  ctx.lineWidth=2; ctx.strokeStyle=e.out; ctx.lineJoin='round';
  if(e.t==='rusher'){                                   // pea
    ctx.fillStyle=e.col; ctx.beginPath(); ctx.arc(0,0,r,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#CFF0A0'; ctx.beginPath(); ctx.arc(-r*.3,-r*.3,r*.28,0,TAU); ctx.fill();
  } else if(e.t==='grunt'){                             // carrot, point first
    ctx.fillStyle=e.col;
    ctx.beginPath(); ctx.moveTo(0,-r*1.9); ctx.lineTo(r*.85,r*.7);
    ctx.lineTo(-r*.85,r*.7); ctx.closePath(); ctx.fill(); ctx.stroke();
    ctx.strokeStyle='#B4611E'; ctx.lineWidth=1.3;
    for(let i=-1;i<2;i++){ ctx.beginPath(); ctx.moveTo(-r*.55,i*r*.5); ctx.lineTo(r*.55,i*r*.5-r*.2); ctx.stroke(); }
    leafy(0,r*.95,r*.55,'#5FA83C',3,TT*2);
  } else if(e.t==='tank'){                              // broccoli
    ctx.fillStyle='#B8D98F'; ctx.strokeStyle=e.out;
    ctx.fillRect(-r*.26,r*.2,r*.52,r*.95); ctx.strokeRect(-r*.26,r*.2,r*.52,r*.95);
    leafy(0,-r*.15,r,e.col,6,TT*1.2);
    ctx.beginPath(); ctx.arc(0,-r*.15,r*.94,0,TAU); ctx.stroke();
  } else if(e.t==='ranged'){                            // chilli
    ctx.fillStyle=e.col;
    ctx.beginPath(); ctx.ellipse(0,0,r*.72,r*1.35,.35,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#4E9A3A';
    ctx.beginPath(); ctx.ellipse(r*.25,-r*1.2,r*.3,r*.5,.5,0,TAU); ctx.fill();
  } else if(e.t==='splitter'){                          // tomato
    ctx.fillStyle=e.col; ctx.beginPath(); ctx.arc(0,r*.1,r,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#FF9C86'; ctx.beginPath(); ctx.arc(-r*.35,-r*.25,r*.24,0,TAU); ctx.fill();
    leafy(0,-r*.75,r*.42,'#4E9A3A',5,0);
  } else if(e.t==='bomber'){                            // onion
    ctx.fillStyle=e.col;
    ctx.beginPath(); ctx.ellipse(0,r*.15,r*.95,r*1.05,0,0,TAU); ctx.fill(); ctx.stroke();
    ctx.strokeStyle='#C9B08A'; ctx.lineWidth=1.1;
    for(let i=-1;i<2;i++){ ctx.beginPath(); ctx.ellipse(i*r*.3,r*.15,r*.26,r*.92,0,0,TAU); ctx.stroke(); }
    ctx.strokeStyle='#7FC24B'; ctx.lineWidth=2.2;
    ctx.beginPath(); ctx.moveTo(0,-r*.9); ctx.lineTo(Math.sin(TT*4)*r*.4,-r*1.8); ctx.stroke();
  } else {                                              // corn
    ctx.fillStyle=e.col;
    ctx.beginPath(); ctx.ellipse(0,0,r*.72,r*1.15,0,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#C99B1E';
    for(let a=-2;a<3;a++) for(let b=-3;b<4;b++) ctx.fillRect(a*r*.26-r*.07,b*r*.28-r*.07,r*.15,r*.15);
    ctx.fillStyle='#6FA83C';
    ctx.beginPath(); ctx.ellipse(-r*.8,r*.3,r*.28,r*.85,-.4,0,TAU); ctx.fill();
    ctx.beginPath(); ctx.ellipse(r*.8,r*.3,r*.28,r*.85,.4,0,TAU); ctx.fill();
  }
  if(e.armor){ ctx.strokeStyle='#B9E3FF'; ctx.lineWidth=1.4; ctx.setLineDash([3,3]);
    ctx.beginPath(); ctx.arc(0,0,r+4,0,TAU); ctx.stroke(); ctx.setLineDash([]); }
  if(e.hit>0){ ctx.globalAlpha=.72; ctx.fillStyle='#FFF';
    ctx.beginPath(); ctx.arc(0,0,r+1,0,TAU); ctx.fill(); ctx.globalAlpha=1; }
  ctx.restore();
  if(e.hp<e.maxhp){
    ctx.fillStyle='#0007'; ctx.fillRect(e.x-e.r,e.y-e.r-9,e.r*2,3);
    ctx.fillStyle='#9FD86B'; ctx.fillRect(e.x-e.r,e.y-e.r-9,e.r*2*(e.hp/e.maxhp),3);
  }
}
function drawDiner(t,S){
  if(t.alive){
    ctx.strokeStyle='rgba(127,194,75,.10)'; ctx.lineWidth=1;
    ctx.beginPath(); ctx.arc(t.x,t.y,S.towerRange,0,TAU); ctx.stroke();
    ctx.fillStyle='#4A3623'; ctx.strokeStyle='#6B5033'; ctx.lineWidth=2;
    ctx.beginPath(); ctx.ellipse(t.x,t.y+17,27,9,0,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#F6ECD9'; ctx.strokeStyle='#B79B77'; ctx.lineWidth=2;
    box(t.x-11,t.y-5,22,22,6); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#E8C39A';
    ctx.beginPath(); ctx.arc(t.x,t.y-14,10,0,TAU); ctx.fill(); ctx.stroke();
    ctx.fillStyle='#3A2A1C';
    ctx.beginPath(); ctx.arc(t.x-3.5,t.y-15,1.6,0,TAU); ctx.fill();
    ctx.beginPath(); ctx.arc(t.x+3.5,t.y-15,1.6,0,TAU); ctx.fill();
    ctx.strokeStyle='#D8DCE2'; ctx.lineWidth=2.6; ctx.lineCap='round';
    const fa=Math.sin(TT*3+t.x)*.5;
    ctx.beginPath(); ctx.moveTo(t.x+10,t.y+3);
    ctx.lineTo(t.x+10+Math.cos(fa-1.1)*14,t.y+3+Math.sin(fa-1.1)*14); ctx.stroke();
    ctx.fillStyle='#9FD86B'; ctx.fillRect(t.x-13,t.y+28,26*(t.hp/t.max),3);
    ctx.strokeStyle='#00000055'; ctx.lineWidth=1; ctx.strokeRect(t.x-13,t.y+28,26,3);
  } else {
    ctx.fillStyle='#2A1A12'; ctx.strokeStyle='#E2503B'; ctx.lineWidth=2; ctx.setLineDash([4,4]);
    ctx.beginPath(); ctx.ellipse(t.x,t.y+10,25,9,0,0,TAU); ctx.fill(); ctx.stroke();
    ctx.setLineDash([]);
    ctx.fillStyle='#E2503B'; ctx.font='700 10px Space Grotesk,sans-serif'; ctx.textAlign='center';
    ctx.fillText('EATEN',t.x,t.y-6); ctx.textAlign='left';
  }
}
function draw(){
  const sh=G?G.shake:0;
  ctx.save();
  ctx.translate(rnd(-sh,sh),rnd(-sh,sh));
  ctx.fillStyle='#3B2A1B'; ctx.fillRect(-20,-20,W+40,H+40);
  ctx.strokeStyle='rgba(49,34,21,.55)'; ctx.lineWidth=6;
  for(let y=-10;y<H+20;y+=27){
    ctx.beginPath(); ctx.moveTo(-20,y);
    ctx.bezierCurveTo(W*.3,y+7,W*.7,y-7,W+20,y+3); ctx.stroke();
  }
  ctx.strokeStyle='#2A1C11'; ctx.lineWidth=2;
  for(let y=-10;y<H+20;y+=81){ ctx.beginPath(); ctx.moveTo(-20,y); ctx.lineTo(W+20,y); ctx.stroke(); }
  if(!G){ ctx.restore(); return; }
  const P=G.player, S=G.S;

  // aura
  if(S.aura>0){
    ctx.fillStyle='rgba(143,211,242,.06)'; ctx.beginPath();
    ctx.arc(P.x,P.y,S.auraR,0,TAU); ctx.fill();
    ctx.strokeStyle='rgba(143,211,242,.22)'; ctx.lineWidth=1.5; ctx.stroke();
  }

  for(const t of G.towers) drawDiner(t,S);

  // rings / tracers
  for(const r of G.rings){
    if(r.to){ ctx.strokeStyle=r.col; ctx.lineWidth=1.6; ctx.globalAlpha=.7;
      ctx.beginPath(); ctx.moveTo(r.x,r.y); ctx.lineTo(r.to.x,r.to.y); ctx.stroke(); ctx.globalAlpha=1; }
    else { ctx.strokeStyle=r.col; ctx.lineWidth=2.4; ctx.globalAlpha=clamp(1-r.r/r.max,0,1);
      ctx.beginPath(); ctx.arc(r.x,r.y,r.r,0,TAU); ctx.stroke(); ctx.globalAlpha=1; }
  }

  // particles
  for(const p of G.parts){ ctx.globalAlpha=clamp(p.life*2.5,0,1); ctx.fillStyle=p.col;
    ctx.fillRect(p.x-1.5,p.y-1.5,3,3); }
  ctx.globalAlpha=1;

  for(const e of G.enemies) drawVeg(e);

  ctx.fillStyle='#FFD2A0'; ctx.strokeStyle='#C4342A'; ctx.lineWidth=1;
  for(const b of G.ebullets){
    ctx.beginPath(); ctx.ellipse(b.x,b.y,3.8,2.4,Math.atan2(b.vy,b.vx),0,TAU); ctx.fill(); ctx.stroke();
  }
  ctx.fillStyle='#FFFDF5'; ctx.strokeStyle='#C9B08A'; ctx.lineWidth=1;
  for(const b of G.bullets){
    ctx.save(); ctx.translate(b.x,b.y); ctx.rotate(b.x*.09+TT*7);
    ctx.fillRect(-S.bsize,-S.bsize,S.bsize*2,S.bsize*2);
    ctx.strokeRect(-S.bsize,-S.bsize,S.bsize*2,S.bsize*2);
    ctx.restore();
  }

  // orbiters
  if(S.orbit>0){
    for(let i=0;i<S.orbit;i++){
      const a=P.orbA+i*TAU/S.orbit;
      ctx.fillStyle='#8FD3F2';
      ctx.beginPath(); ctx.arc(P.x+Math.cos(a)*66,P.y+Math.sin(a)*66,6,0,TAU); ctx.fill();
    }
  }

  ctx.save(); ctx.translate(P.x,P.y);
  ctx.fillStyle='#241A12'; ctx.globalAlpha=.35;
  ctx.beginPath(); ctx.ellipse(0,10,13,5,0,0,TAU); ctx.fill(); ctx.globalAlpha=1;
  ctx.save(); ctx.rotate(P.a);
  ctx.fillStyle='#5A3E28'; ctx.strokeStyle='#2E1E12'; ctx.lineWidth=2;
  box(8,-5,18,10,3); ctx.fill(); ctx.stroke();
  ctx.fillStyle='#C9B08A'; ctx.fillRect(24,-3.5,5,7);
  ctx.restore();
  ctx.fillStyle=P.inv>0?'#FFFFFF':'#F6ECD9'; ctx.strokeStyle='#B79B77'; ctx.lineWidth=2;
  ctx.beginPath(); ctx.arc(0,0,11,0,TAU); ctx.fill(); ctx.stroke();
  ctx.fillStyle='#E8C39A'; ctx.beginPath(); ctx.arc(0,-3,6.5,0,TAU); ctx.fill();
  ctx.fillStyle='#FFFDF5'; ctx.strokeStyle='#CFC0A4';
  ctx.beginPath(); ctx.ellipse(0,-12,8,5.5,0,0,TAU); ctx.fill(); ctx.stroke();
  ctx.fillRect(-6,-11,12,4);
  ctx.restore();

  ctx.restore();

  // joystick
  if(stick.active){
    ctx.globalAlpha=.3; ctx.strokeStyle='#EDE9E2'; ctx.lineWidth=2;
    ctx.beginPath(); ctx.arc(stick.ox,stick.oy,52,0,TAU); ctx.stroke();
    ctx.fillStyle='#EDE9E2'; ctx.beginPath();
    ctx.arc(stick.ox+stick.x*52,stick.oy+stick.y*52,18,0,TAU); ctx.fill();
    ctx.globalAlpha=1;
  }
}

/* ================= draft ================= */
let pending=null;
function openDraft(){
  const gone=expireTick();
  buildWave();
  const n=Object.keys(G.owned).length;
  let unlock='';
  if(G.wave>1&&G.wave%5===0)  unlock+='+1 SLOT · ';
  if(G.wave>1&&G.wave%10===0) unlock+='+1 ANCHOR · ';
  $('slotLine').textContent = unlock + (gone.length? gone.join(' + ')+' burned out · ' : '')
    + 'Kit '+n+'/'+slotCap();
  // weight toward what you already own, so builds actually come together
  const pool=[];
  for(const p of POWERS){
    const lvl=G.owned[p.id]?G.owned[p.id].l:0;
    let w=1;
    if(lvl>0) w=2.4;
    if(lvl>=5) w=.6;
    if(p.id==='auraR'&&!G.owned.aura) w=.15;
    for(let i=0;i<Math.round(w*10);i++) pool.push(p);
  }
  const picks=[];
  let guard=0;
  while(picks.length<3&&guard++<400){
    const p=pool[Math.floor(Math.random()*pool.length)];
    if(!picks.find(x=>x.id===p.id)) picks.push(p);
  }
  $('cards').innerHTML=picks.map(p=>{
    const o=G.owned[p.id];
    const tag = o ? `<em>lvl ${o.l} → ${o.l+1} · clock resets</em>`
                  : (Object.keys(G.owned).length>=slotCap() ? '<em style="color:#E8574C">needs a slot</em>' : '');
    return `<div class="card ${o?'up':''}" data-p="${p.id}">
      <div class="n">${p.n}${tag}</div>
      <div class="d">${p.d}</div></div>`;
  }).join('');
  paintRig();
  $('draft').classList.remove('hide');
}
function paintRig(){
  const ids=Object.keys(G.owned);
  $('anchorLine').textContent = 'Anchors left · '+anchorsLeft()+' of '+anchorCap()
    +'   ·   next slot at wave '+((Math.floor(G.wave/5)+1)*5);
  if(!ids.length){ $('rig').innerHTML=''; return; }
  $('rig').innerHTML=ids.map(id=>{
    const p=byId(id), o=G.owned[id];
    const btn = o.a ? '' : (anchorsLeft()>0 ? `<div class="ancbtn" data-a="${id}">Anchor</div>` : '');
    return `<div class="rigrow ${o.a?'anc':''}">
      <div><div class="rn">${p.n} ${o.l}</div>
        <div class="rt ${o.a?'inf':''}">${o.a?'anchored \u2014 never expires':o.t+' waves left'}</div></div>
      ${btn}</div>`;
  }).join('');
}
$('rig').addEventListener('click',e=>{
  const b=e.target.closest('.ancbtn'); if(!b) return;
  const id=b.dataset.a;
  if(anchorsLeft()<=0||!G.owned[id]||G.owned[id].a) return;
  G.owned[id].a=1; G.anchorsUsed++;
  paintRig(); paintPerks(); blip(520,.3,.13,'triangle'); buzz(40);
});
function equip(id){
  if(G.owned[id]){ G.owned[id].l++; if(!G.owned[id].a) G.owned[id].t=LIFE; }
  else G.owned[id]={l:1,t:LIFE,a:0};
  recalc(false); paintPerks();
  if(id==='hp') G.player.hp=Math.min(G.S.maxhp,G.player.hp+35);
  if(id==='twhp') G.towers.forEach(t=>{ if(t.alive) t.hp=t.max; });
  $('draft').classList.add('hide'); $('swap').classList.add('hide');
  running=true; blip(760,.16,.1,'triangle');
}
$('cards').addEventListener('click',e=>{
  const c=e.target.closest('.card'); if(!c) return;
  const id=c.dataset.p;
  if(!G.owned[id] && Object.keys(G.owned).length>=slotCap()){ openSwap(id); return; }
  equip(id);
});
function openSwap(id){
  pending=id;
  $('pendName').textContent='Coming in: '+byId(id).n;
  $('swapCards').innerHTML=Object.keys(G.owned).map(k=>{
    const p=byId(k), o=G.owned[k];
    return `<div class="card" data-s="${k}">
      <div class="n">${p.n}<em>lvl ${o.l} · ${o.a?'anchored':o.t+'w left'}</em></div>
      <div class="d">${p.d}${o.a?' <span style="color:#5B9BD5">Dropping this returns the anchor.</span>':''}</div></div>`;
  }).join('');
  $('draft').classList.add('hide');
  $('swap').classList.remove('hide');
}
$('swapCards').addEventListener('click',e=>{
  const c=e.target.closest('.card'); if(!c||!pending) return;
  if(G.owned[c.dataset.s].a) G.anchorsUsed--;   // the anchor comes back with it
  delete G.owned[c.dataset.s];
  const id=pending; pending=null;
  equip(id);
});

/* ================= flow ================= */
function startRun(){
  aInit(); if(AC&&AC.state==='suspended') AC.resume();
  try{ const el=document.documentElement;
    (el.requestFullscreen||el.webkitRequestFullscreen||function(){}).call(el); }catch(e){}
  newGame();
  $('title').classList.add('hide'); $('over').classList.add('hide');
  openDraft();
}
function endRun(){
  if(G.over) return;
  G.over=true; running=false;
  const w=Math.max(0,G.wave-1);
  if(w>best){ best=w; try{ localStorage.setItem('salad:best',String(best)); }catch(e){} }
  $('endWhy').textContent = G.player.hp<=0 ? 'The chef was eaten' : 'They ate everyone';
  $('endN').textContent=w; $('endBest').textContent=best;
  $('over').classList.remove('hide'); $('draft').classList.add('hide');
  boom(.9,500,.3); buzz([80,60,180]);
}
$('startBtn').addEventListener('click',startRun);
$('againBtn').addEventListener('click',startRun);

let last=performance.now();
function frame(now){
  requestAnimationFrame(frame);
  const dt=Math.min((now-last)/1000,.045); last=now; TT+=dt;
  if(running&&G&&!G.over) step(dt);
  if(msgT>0){ msgT-=dt; if(msgT<=0) $('msg').style.opacity=0; }
  draw();
}
function checkOrient(){
  const land=innerWidth>innerHeight;
  $('rot').classList.toggle('show',land);
  if(land&&running) running=false;
}
addEventListener('resize',()=>{ resize(); checkOrient(); });
addEventListener('orientationchange',()=>setTimeout(()=>{resize();checkOrient();},300));
resize(); checkOrient(); frame(performance.now());
</script>
</body>
</html>
