<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>3D 야구 경기</title>
<link href="https://fonts.googleapis.com/css2?family=Do+Hyeon&display=swap" rel="stylesheet">
<style>
:root{--hud:rgba(8,22,16,.84);--ink:#f3f0e4;--dim:#9db7a6;--lamp:#ffd34d;--red:#ff7262;--line:rgba(243,240,228,.2);color-scheme:dark}
html,body{margin:0;height:100%;background:#0b1a12;overflow:hidden;font-family:"Do Hyeon",system-ui,sans-serif;color:var(--ink);-webkit-user-select:none;user-select:none;touch-action:manipulation}
#c{position:fixed;inset:0;width:100%;height:100%;display:block}
#board{position:fixed;left:10px;top:calc(env(safe-area-inset-top,0px) + 10px);background:var(--hud);border:1px solid var(--line);border-radius:6px;border-left:4px solid #f37321;padding:8px 12px;min-width:150px}
#top{display:flex;justify-content:space-between;gap:12px;color:var(--dim);font-size:14px}
#score{display:flex;align-items:baseline;gap:8px;font-size:15px;margin:2px 0}
#score b{font-size:30px;font-weight:400;color:var(--lamp);line-height:1}
#foot{display:flex;align-items:center;justify-content:space-between;gap:10px}
#cnt{font-size:14px;line-height:1.5;letter-spacing:.06em}
#bs rect{fill:none;stroke:var(--dim);stroke-width:1.5}
#bs rect.on{fill:var(--lamp);stroke:var(--lamp)}
#pinfo{position:fixed;right:10px;top:calc(env(safe-area-inset-top,0px) + 10px);background:var(--hud);border:1px solid var(--line);border-radius:6px;padding:8px 12px;font-size:17px;min-width:120px;text-align:center}
#msg{position:fixed;left:0;right:0;top:30%;text-align:center;font-size:clamp(34px,9vw,68px);opacity:0;transform:scale(.9);transition:opacity .18s,transform .18s;pointer-events:none;text-shadow:0 3px 14px rgba(0,0,0,.7)}
#msg.show{opacity:1;transform:scale(1)}
#msg.gold{color:var(--lamp)}
#msg.red{color:var(--red)}
#sw{position:fixed;right:16px;bottom:calc(env(safe-area-inset-bottom,0px) + 22px);width:104px;height:104px;border-radius:50%;border:3px solid var(--ink);background:var(--hud);color:var(--ink);font:inherit;font-size:26px;cursor:pointer}
#sw:active{background:var(--lamp);color:#10261a;border-color:var(--lamp)}
#hint{position:fixed;left:0;right:0;bottom:calc(env(safe-area-inset-bottom,0px) + 134px);text-align:center;color:var(--ink);font-size:14px;opacity:.75;text-shadow:0 1px 6px #000}
#end{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(6,16,11,.88)}
#end.on{display:flex}
#end div{text-align:center}
#end h1{font-weight:400;font-size:clamp(44px,12vw,84px);margin:0;color:var(--lamp)}
#end p{font-size:22px;margin:8px 0 24px}
#re{font:inherit;font-size:22px;padding:10px 28px;border-radius:6px;border:2px solid var(--ink);background:transparent;color:var(--ink);cursor:pointer}
#pt{position:fixed;left:50%;bottom:calc(env(safe-area-inset-bottom,0px) + 22px);transform:translateX(-50%);display:none;gap:8px}
#pt button{font:inherit;font-size:19px;padding:10px 14px;border-radius:8px;border:2px solid var(--line);background:var(--hud);color:var(--ink);cursor:pointer;min-width:70px}
#pt button small{display:block;font-size:12px;color:var(--dim)}
#pt button.on{border-color:var(--lamp);color:var(--lamp)}
.sub{position:fixed;bottom:calc(env(safe-area-inset-bottom,0px) + 22px);width:72px;height:72px;border-radius:50%;border:2px solid var(--ink);background:var(--hud);color:var(--ink);font:inherit;font-size:18px;cursor:pointer}
#bt{right:128px}#st{right:208px}#po{right:16px;display:none}
#st.on{background:var(--lamp);color:#10261a;border-color:var(--lamp)}
#ph{right:288px}#ib{left:12px;right:auto;display:none}#pc{left:92px;right:auto;display:none}#ib,#pc,#ph{font-size:14px}
#bi{position:fixed;left:50%;transform:translateX(-50%);bottom:calc(env(safe-area-inset-bottom,0px) + 3px);max-width:96vw;background:var(--hud);border:1px solid var(--line);border-radius:6px;padding:3px 10px;font-size:13px;text-align:center;line-height:1.3;pointer-events:none;white-space:nowrap}
#bi b{color:var(--lamp);font-weight:400}
#bi span{color:var(--dim);font-size:12px}
#pa{position:fixed;left:50%;top:44%;transform:translate(-50%,-50%) scale(.95);background:var(--hud);border:1px solid var(--lamp);border-radius:10px;padding:10px 22px;text-align:center;opacity:0;transition:opacity .25s,transform .25s;pointer-events:none;font-size:18px}
#pa.show{opacity:1;transform:translate(-50%,-50%) scale(1)}
#pa b{display:block;font-weight:400;font-size:34px;color:var(--lamp);line-height:1.1}
#pa small{display:block;font-size:13px;color:var(--dim);margin-top:4px}
#ln{position:fixed;inset:0;background:rgba(6,16,11,.95);display:flex;align-items:flex-start;justify-content:center;z-index:5;overflow:auto;padding:12px}
#lnb{max-width:min(720px,96vw);width:100%}
#lnb h2{font-weight:400;font-size:26px;color:var(--lamp);margin:0 0 4px}
#lnb .note{font-size:12.5px;color:var(--dim);margin:0 0 8px;line-height:1.5}
#lnb .note b{color:var(--ink);font-weight:400}
.lr{display:grid;grid-template-columns:22px 1fr auto;gap:8px;align-items:center;padding:5px 8px;border:1px solid var(--line);border-radius:6px;margin-bottom:4px;font-size:14px;cursor:pointer}
.lr.sel{border-color:var(--lamp);background:rgba(255,211,77,.12)}
.lr i{font-style:normal;color:var(--dim);font-size:11.5px;display:block}
.lr b{color:var(--lamp);font-weight:400}
.lr small{color:var(--dim)}
#lnb button{font:inherit;font-size:18px;padding:8px 18px;border-radius:8px;border:2px solid var(--ink);background:transparent;color:var(--ink);cursor:pointer;margin:8px 8px 16px 0}
#lnb #lnGo{border-color:var(--lamp);color:var(--lamp)}
#dfr{margin:0 0 8px;font-size:14px;color:var(--dim)}
#lnb #dfr button{font-size:15px;padding:5px 14px;margin:0 6px 4px 0}
#lnb #dfr button.on{border-color:var(--lamp);color:var(--lamp);background:rgba(255,211,77,.12)}
#dfr small{font-size:12px}
#mdr{margin:0 0 8px;font-size:14px;color:var(--dim)}
#lnb #mdr button{font-size:15px;padding:5px 14px;margin:0 6px 4px 0}
#lnb #mdr button.on{border-color:var(--lamp);color:var(--lamp);background:rgba(255,211,77,.12)}
#dfr button:disabled{opacity:.4;cursor:default}
#fg{position:fixed;inset:0;display:none;flex-direction:column;align-items:center;justify-content:center;gap:10px;background:rgba(0,0,0,.88);z-index:9;padding:8px}
#fgc{width:min(96vw,640px);height:auto;border-radius:10px;border:1px solid var(--line);background:#000;touch-action:none}
#fg{background:transparent!important;justify-content:space-between!important;pointer-events:none;padding:calc(env(safe-area-inset-top,0px) + 10px) 10px calc(env(safe-area-inset-bottom,0px) + 14px)!important}
#fgh{display:flex;align-items:flex-start;justify-content:space-between;gap:10px;width:min(96vw,640px)}
.fb{flex:1;font-size:15px;text-shadow:0 1px 4px #000}
.fb.r{text-align:right}
.fb i{display:block;height:14px;background:rgba(0,0,0,.6);border-radius:7px;overflow:hidden;margin-top:3px}
.fb b{display:block;height:100%;width:100%;background:#f37321}
.fb.r b{background:#c0392b;margin-left:auto}
#fgt{font:400 30px "Do Hyeon",sans-serif;min-width:70px;text-align:center;text-shadow:0 2px 6px #000}
#fgm,#fg small{pointer-events:auto}
#fgm button{background:rgba(0,0,0,.55)}
#fgm{position:fixed!important;left:0;right:0;bottom:0;height:0;display:block!important}
#fgm button{position:fixed;width:86px;height:86px;border-radius:50%;padding:0!important;font-size:19px;bottom:calc(env(safe-area-inset-bottom,0px) + 22px);background:rgba(0,0,0,.5);pointer-events:auto}
#fgm [data-a=L]{left:14px}
#fgm [data-a=R]{left:112px}
#fgm [data-a=P]{right:112px}
#fgm [data-a=K]{right:14px}
#fgm [data-a=B]{right:63px;bottom:calc(env(safe-area-inset-bottom,0px) + 118px)}
body.fighting #sw,body.fighting #bt,body.fighting #st,body.fighting #po,body.fighting #ph,body.fighting #ib,body.fighting #pc,body.fighting #pt,body.fighting #bf,body.fighting #bc,body.fighting #rq,body.fighting #skip,body.fighting #snd,body.fighting #tg,body.fighting #board,body.fighting #pinfo,body.fighting #bi,body.fighting #az,body.fighting #hint,body.fighting #abs,body.fighting #tm,body.fighting #pv,body.fighting #pa,body.fighting #vr,body.fighting #msg{display:none!important}
#fg small{position:fixed;left:0;right:0;bottom:calc(env(safe-area-inset-bottom,0px) + 2px);text-align:center;font-size:11px}
#fgm{display:flex;gap:8px;flex-wrap:wrap;justify-content:center}
#fgm button{font:inherit;font-size:20px;min-width:64px;padding:14px 16px;border-radius:12px;border:2px solid var(--ink);background:rgba(255,255,255,.08);color:var(--ink);touch-action:none}
#fgm button:active{background:var(--lamp);color:#10261a}
#fg small{color:var(--dim)}
#bf{position:fixed;right:16px;bottom:calc(env(safe-area-inset-bottom,0px) + 136px);display:none;font:inherit;font-size:22px;padding:10px 22px;border-radius:12px;border:2px solid #f37321;background:#f37321;color:#fff;cursor:pointer;z-index:3}
#bc{position:fixed;left:50%;transform:translateX(-50%);top:calc(env(safe-area-inset-top,0px) + 8px);display:none;font:inherit;font-size:14px;padding:5px 12px;border-radius:8px;border:1px solid #c0392b;background:rgba(80,14,14,.85);color:#ffd9d4;cursor:pointer;z-index:3}
#rq{position:fixed;left:50%;transform:translateX(-50%);bottom:calc(env(safe-area-inset-bottom,0px) + 150px);display:none;font:inherit;font-size:20px;padding:10px 20px;border-radius:10px;border:2px solid var(--lamp);background:var(--lamp);color:#10261a;cursor:pointer;z-index:3}
#abs{position:fixed;left:10px;top:calc(env(safe-area-inset-top,0px) + 130px);background:var(--hud);border:1px solid var(--line);border-radius:8px;padding:5px;opacity:0;transition:opacity .2s;pointer-events:none;text-align:center}
#abs.show{opacity:1}
#abs canvas{display:block;width:60px;height:80px}
#abs b{display:block;font-weight:400;font-size:13px;margin-top:2px}
#vr{position:fixed;left:50%;top:13%;transform:translateX(-50%);background:var(--hud);border:1px solid var(--ink);border-radius:8px;padding:8px 18px;font-size:20px;color:var(--ink);opacity:0;transition:opacity .2s;pointer-events:none;white-space:nowrap}
#vr.show{opacity:1}
#board{display:flex;align-items:stretch;padding:0;min-width:0;border:0;background:rgba(10,12,16,.84);border-radius:4px;overflow:hidden;left:8px;top:calc(env(safe-area-inset-top,0px) + 8px)}
#foot{display:contents}
#inn{display:flex;flex-direction:column;align-items:center;justify-content:center;width:34px;background:rgba(0,0,0,.5);font-size:22px;line-height:1.05}
#inn b{font-weight:400}
#inn i{font-style:normal;font-size:11px;color:#ffd34d}
#inn small{font-size:9px;color:#9db7a6}
#teams{display:flex;flex-direction:column;min-width:132px}
.tr{display:flex;justify-content:space-between;align-items:center;padding:0 0 0 9px;font-size:15px;height:28px}
.tr b{font-weight:400;font-size:20px;background:#f3f1ea;color:#111;height:100%;display:flex;align-items:center;justify-content:center;min-width:36px}
.tr.hw{background:linear-gradient(90deg,#f37321,#c4561a)}
.tr.op{background:linear-gradient(90deg,#3a1b1b,#9a2a2a)}
#bs{order:1;margin:4px 8px;align-self:center}
#cnt{order:2;display:flex;flex-direction:column;justify-content:center;padding:0 12px;background:rgba(255,255,255,.07);min-width:74px;text-align:center;letter-spacing:0;line-height:1.25}
#cnt .c1{font-size:21px}
#cnt .c2{font-size:13px;color:#ffd34d}
#tg{position:fixed;left:8px;top:calc(env(safe-area-inset-top,0px) + 70px);display:flex;gap:6px;z-index:2}
#tg button{font:inherit;font-size:12px;padding:4px 8px;border-radius:6px;border:1px solid var(--line);background:rgba(10,12,16,.75);color:var(--dim);cursor:pointer}
#tg button.on{border-color:var(--lamp);color:var(--lamp)}
#snd{position:fixed;right:10px;top:calc(env(safe-area-inset-top,0px) + 58px);width:38px;height:34px;border-radius:8px;border:1px solid var(--line);background:var(--hud);color:var(--ink);font-size:16px;cursor:pointer}
#pv{position:fixed;left:50%;top:24%;transform:translateX(-50%);font-size:34px;color:var(--ink);text-shadow:0 2px 12px rgba(0,0,0,.9);opacity:0;transition:opacity .2s;pointer-events:none;white-space:nowrap}
#pv.show{opacity:1}
#pv b{font-weight:400;color:var(--lamp)}
#pv small{font-size:18px;color:var(--dim);margin-left:4px}
#tm{position:fixed;left:50%;top:58%;transform:translate(-50%,0);font-size:30px;opacity:0;transition:opacity .15s;text-shadow:0 2px 10px rgba(0,0,0,.8);pointer-events:none;white-space:nowrap}
#tm.show{opacity:1}
#az{position:fixed;right:12px;bottom:calc(env(safe-area-inset-bottom,0px) + 110px);display:none;background:var(--hud);border:1px solid var(--line);border-radius:8px;padding:6px;touch-action:none}
#az b{display:block;font-weight:400;font-size:13px;color:var(--dim);text-align:center;margin-bottom:3px}
#az canvas{display:block;width:150px;height:180px;border-radius:4px;cursor:crosshair}
#skip{position:fixed;left:12px;bottom:calc(env(safe-area-inset-bottom,0px) + 110px);display:none;font:inherit;font-size:18px;padding:10px 16px;border-radius:8px;border:2px solid var(--ink);background:var(--hud);color:var(--ink);cursor:pointer}
#rp{position:fixed;left:50%;top:18%;transform:translateX(-50%);display:none;background:var(--hud);border:1px solid var(--red);color:var(--red);border-radius:6px;padding:6px 16px;font-size:20px}
</style>
</head>
<body>
<canvas id="c"></canvas>
<div id="board">
  <div id="inn"></div><span id="role" style="display:none"></span><div id="teams"><div class="tr hw"><span>한화</span><b id="sp">0</b></div><div class="tr op"><span>상대</span><b id="sc">0</b></div></div>
  
  <div id="foot">
    <div id="cnt"></div>
    <svg id="bs" viewBox="0 0 40 30" width="52" height="39"><rect id="b2" x="15" y="2" width="8" height="8" transform="rotate(45 19 6)"/><rect id="b3" x="2" y="14" width="8" height="8" transform="rotate(45 6 18)"/><rect id="b1" x="28" y="14" width="8" height="8" transform="rotate(45 32 18)"/></svg>
  </div>
</div>
<div id="pinfo"></div>
<div id="bi"></div><div id="pa"></div><div id="pv"></div><div id="tg"><button id="tgB" class="on">타자 모드 ON</button><button id="tgP" class="on">투구 모드 ON</button></div><button id="snd">🔊</button><div id="tm"></div><div id="vr"></div><button id="rq"></button><button id="bf">빠던</button><button id="bc">벤치 클리어링</button><div id="abs"><canvas id="absc" width="120" height="160"></canvas><b id="abst"></b></div>
<div id="az"><b>조준창 (정면)</b><canvas id="azc" width="300" height="360"></canvas></div>
<div id="msg"></div>
<div id="rp">▶ 리플레이</div>
<button id="skip">건너뛰기 ▶▶</button>
<div id="hint">공이 홈플레이트에 오기 직전에 스윙 (스페이스 / 버튼 / 화면 터치)</div>
<button id="sw">스윙</button>
<button id="bt" class="sub">번트</button><button id="st" class="sub">도루</button><button id="po" class="sub">견제</button><button id="ph" class="sub">대타 3</button><button id="ib" class="sub">고의사구</button><button id="pc" class="sub">투수교체</button>
<div id="pt"><button data-t="직구" class="on">직구<small>130–145</small></button><button data-t="슬라이더">슬라이더<small>110–120</small></button><button data-t="커브">커브<small>100–110</small></button><button data-t="체인지업">체인지업<small>120–130</small></button></div>
<div id="ln"><div id="lnb">
  <h2>한화 이글스 라인업 (KBO 타순 구성)</h2>
  <p class="note">1번 출루·주력 → 2번 컨택 → 3번 최고 타자 → 4번 거포 → 5번 파워 → 6~7번 중간 → 8번 수비형 → 9번 주력. 두 줄을 차례로 누르면 타순이 바뀝니다. DH(지명타자) 제도를 적용하고, 투수는 타석에 들어오지 않습니다.</p>
  <p class="note"><b>경기장</b> 대전 한화생명 볌파크 · 좌 99m · 좌중 115m · 중 122m · 우중 112m · 우 95m · 우측 8m 몬스터월</p>
  <div id="mdr">경기 모드 <button data-m="normal" class="on">일반 (9이닝)</button><button data-m="chal">챌린지 (3이닝 · 익스트림)</button></div>
  <div id="dfr">난이도 <button data-d="easy">쉽음</button><button data-d="normal" class="on">보통</button><button data-d="hard">어려움</button><br><small id="dfd"></small></div>
  <div id="lnU"></div><div id="lnS"></div>
  <p class="note">※ 한화 선수는 실제 선수 이름에 공개 기록을 참고한 추정 능력치이고, 상대는 가상 선수입니다.  능력치 50이 2026 KBO 리그 평균(타율 약 .267, OPS 약 .745)에 해당합니다.</p>
  <button id="lnAuto">자동 구성</button><button id="lnGo">경기 시작</button>
</div></div>
<div id="fg"><div id="fgh"><div class="fb"><span id="fn1"></span><i><b id="fh1"></b></i></div><div id="fgt">40</div><div class="fb r"><span id="fn2"></span><i><b id="fh2"></b></i></div></div><div id="fgm"><button data-a="L">◀</button><button data-a="R">▶</button><button data-a="P">주먹</button><button data-a="K">발차기</button><button data-a="B">방어</button></div><small>키보드: ← → 이동 · J 주먹 · K 발차기 · L 방어</small></div>
<div id="end"><div><h1 id="res"></h1><p id="fin"></p><button id="re">다시 하기</button></div></div>
<div id="md" style="display:none;position:fixed;inset:0;z-index:20;background:rgba(6,16,11,.9);align-items:center;justify-content:center;padding:16px">
  <div id="mdb" style="max-width:420px;width:100%;background:var(--hud);border:1px solid var(--lamp);border-radius:10px;padding:16px 18px;max-height:85vh;overflow:auto">
    <div id="mdc"></div>
    <button id="mdx" style="font:inherit;font-size:16px;padding:6px 16px;margin-top:10px;border-radius:6px;border:1px solid var(--ink);background:transparent;color:var(--ink);cursor:pointer">닫기</button>
  </div>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
let INNINGS=9;const SLOW=1.75, R=122, WH=2.4;
const $=id=>document.getElementById(id);
let TS=1,VT=0,VL=performance.now();const now=()=>{const r=performance.now();VT+=(r-VL)/1000*TS;VL=r;return VT};
function modal(html){$('mdc').innerHTML=html;$('md').style.display='flex'}
function closeModal(){$('md').style.display='none';$('mdc').innerHTML=''}
$('mdx').onclick=closeModal;
$('md').addEventListener('click',e=>{if(e.target.id==='md')closeModal()});

/* ---------- 장면 ---------- */
const ren=new THREE.WebGLRenderer({canvas:$('c'),antialias:true});
ren.shadowMap.enabled=true;ren.shadowMap.type=THREE.PCFSoftShadowMap;
ren.setPixelRatio(Math.min(devicePixelRatio||1,2));
const scene=new THREE.Scene();
function tex(w,h,fn,rx,ry){const c=document.createElement('canvas');c.width=w;c.height=h;fn(c.getContext('2d'),w,h);const t=new THREE.CanvasTexture(c);t.wrapS=t.wrapT=THREE.RepeatWrapping;t.repeat.set(rx||1,ry||1);t.anisotropy=4;return t}
function grassT(a,b,r){return tex(256,256,(g,w,h)=>{for(let i=0;i<8;i++){g.fillStyle=i%2?a:b;g.fillRect(i*w/8,0,w/8,h)}for(let i=0;i<1200;i++){g.fillStyle='rgba(0,0,0,.05)';g.fillRect(Math.random()*w,Math.random()*h,2,3)}},r,r)}
function dirtT(r){return tex(128,128,(g,w,h)=>{g.fillStyle='#b98757';g.fillRect(0,0,w,h);for(let i=0;i<900;i++){g.fillStyle=Math.random()<.5?'rgba(90,60,35,.14)':'rgba(220,180,130,.14)';g.fillRect(Math.random()*w,Math.random()*h,2,2)}},r,r)}
function wallT(){return tex(2048,64,(g,w,h)=>{
  g.fillStyle='#0f1013';g.fillRect(0,0,w,h);
  const C=['#c0392b','#2471a3','#d4ac0d','#1e8449'],N=['3D','BASEBALL','HOME RUN','PLAY BALL','STRIKE','OUT','SAFE','BALL'];
  for(let i=0;i<8;i++){g.fillStyle=C[i%4];g.fillRect(i*256+10,12,236,44);g.save();g.translate(i*256+128,45);g.scale(.45,1);g.fillStyle='#fff';g.textAlign='center';g.font='bold 34px sans-serif';g.fillText(N[i],0,0);g.restore()}
  g.fillStyle='#f37321';g.fillRect(0,0,w,6);
},-1,1)}
scene.background=tex(2,256,(g,w,h)=>{const gr=g.createLinearGradient(0,0,0,h);gr.addColorStop(0,'#05070f');gr.addColorStop(.6,'#0b1530');gr.addColorStop(1,'#1c2a4a');g.fillStyle=gr;g.fillRect(0,0,w,h)});
scene.fog=new THREE.Fog(0x0b1328,170,420);
const cam=new THREE.PerspectiveCamera(52,1,.1,600);
function baseFov(){const a=innerWidth/Math.max(1,innerHeight);return a>2.1?64:a>1.7?58:a>1.4?54:52}
function resize(){ren.setSize(innerWidth,innerHeight,false);cam.aspect=innerWidth/innerHeight;cam.fov=baseFov();cam.updateProjectionMatrix()}
addEventListener('resize',resize);resize();
scene.add(new THREE.HemisphereLight(0xcfd8ff,0x2f4a30,.55));
const sun=new THREE.DirectionalLight(0xfff1d0,.95);sun.position.set(40,70,10);sun.target.position.set(0,0,-25);scene.add(sun,sun.target);
sun.castShadow=true;sun.shadow.mapSize.set(2048,2048);const shc=sun.shadow.camera;shc.left=-45;shc.right=45;shc.top=45;shc.bottom=-45;shc.near=10;shc.far=200;sun.shadow.bias=-.0005;

const M=c=>new THREE.MeshLambertMaterial({color:c});
function add(g,c,x,y,z){const m=new THREE.Mesh(g,M(c));m.position.set(x,y,z);m.receiveShadow=true;scene.add(m);return m}
const flat=m=>{m.rotation.x=-Math.PI/2;return m};
{const m=add(new THREE.PlaneGeometry(700,700),0x3f8f45,0,0,-120);m.material=new THREE.MeshLambertMaterial({map:grassT('#3d8a43','#4a9b50',14)});flat(m)}
{const m=add(new THREE.CircleGeometry(29,48),0xb98757,0,.02,-19.4);m.material=new THREE.MeshLambertMaterial({map:dirtT(6)});flat(m)}
const inf=add(new THREE.PlaneGeometry(24,24),0x4aa650,0,.04,-19.4);inf.material=new THREE.MeshLambertMaterial({map:grassT('#4aa650','#58b55d',1.5)});inf.rotation.set(-Math.PI/2,0,Math.PI/4);
{const m=add(new THREE.CircleGeometry(6,24),0xb98757,0,.05,0);m.material=new THREE.MeshLambertMaterial({map:dirtT(1)});flat(m)}
add(new THREE.CylinderGeometry(2.8,3.2,.3,24),0xb98757,0,.15,-18.44);
[[19.4,-19.4],[0,-38.8],[-19.4,-19.4]].forEach(p=>add(new THREE.BoxGeometry(.6,.1,.6),0xffffff,p[0],.1,p[1]));
add(new THREE.BoxGeometry(.45,.06,.45),0xffffff,0,.08,0);
for(const s of[-1,1]){
  const g=new THREE.BufferGeometry().setFromPoints([new THREE.Vector3(0,.07,0),new THREE.Vector3(s*(s<0?99:95)*.7071,.07,-(s<0?99:95)*.7071)]);
  scene.add(new THREE.Line(g,new THREE.LineBasicMaterial({color:0xffffff})));
}
const wall=new THREE.Mesh(fenceGeo(-45,26.5),new THREE.MeshLambertMaterial({map:wallT(),side:THREE.DoubleSide}));
scene.add(wall);
const zone=new THREE.Mesh(new THREE.PlaneGeometry(.5,.7),new THREE.MeshBasicMaterial({color:0xffffff,transparent:true,opacity:.07,depthWrite:false,side:THREE.DoubleSide}));
zone.position.set(0,.8,0);scene.add(zone);
const ret=new THREE.Mesh(new THREE.RingGeometry(.05,.075,24),new THREE.MeshBasicMaterial({color:0xffd34d,side:THREE.DoubleSide,depthTest:false}));
ret.position.set(0,.8,.02);ret.visible=false;ret.renderOrder=5;ret.scale.setScalar(2.4);scene.add(ret);

/* ---------- 선수 (관절 있는 사람 모델 + 동작) ---------- */
const HUM=[],BP=[[19.4,-19.4],[0,-38.8],[-19.4,-19.4]],runners=[null,null,null],running=[];let MV=[],pw=false;
function humanOld(shirt,pants,cap,x,z,glove){
  const g=new THREE.Group(),P={};
  const L=(len,r,c,px,py)=>{const p=new THREE.Group();p.position.set(px,py,0);const m=new THREE.Mesh(new THREE.CylinderGeometry(r,r*.85,len,6),M(c));m.position.y=-len/2;m.castShadow=true;p.add(m);return p};
  P.lL=L(.9,.11,pants,-.14,.9);P.lR=L(.9,.11,pants,.14,.9);g.add(P.lL,P.lR);
  const body=new THREE.Group();body.position.y=.9;g.add(body);P.body=body;
  const t=new THREE.Mesh(new THREE.CylinderGeometry(.26,.22,.7,8),M(shirt));t.position.y=.35;t.castShadow=true;
  const hd=new THREE.Mesh(new THREE.SphereGeometry(.2,10,8),M(0xf0c9a0));hd.position.y=.95;
  const cp=new THREE.Mesh(new THREE.SphereGeometry(.215,10,6,0,Math.PI*2,0,Math.PI/2),M(cap));cp.position.y=.98;
  const br=new THREE.Mesh(new THREE.BoxGeometry(.3,.02,.25),M(cap));br.position.set(0,.98,-.22);
  body.add(t,hd,cp,br);
  P.aL=L(.65,.08,shirt,-.34,.65);P.aR=L(.65,.08,shirt,.34,.65);body.add(P.aL,P.aR);
  if(glove){const gl=new THREE.Mesh(new THREE.SphereGeometry(.13,8,6),M(0x7a4a22));gl.position.y=-.68;P.aL.add(gl)}
  /* 디테일: 신발·손·벨트·목·어깨·등번호·유니폼 줄무늬·헬멧·포수/심판 보호구 */
  const skin=0xf0c9a0,dark=0x1b1b1f;
  [P.lL,P.lR].forEach(l=>{const s=new THREE.Mesh(new THREE.BoxGeometry(.17,.09,.32),M(dark));s.position.set(0,-.9,-.07);s.castShadow=true;l.add(s)});
  [P.aL,P.aR].forEach(a=>{const h=new THREE.Mesh(new THREE.SphereGeometry(.075,8,6),M(skin));h.position.y=-.66;a.add(h)});
  const belt=new THREE.Mesh(new THREE.CylinderGeometry(.235,.235,.07,10),M(0x222222));belt.position.y=.05;
  const neck=new THREE.Mesh(new THREE.CylinderGeometry(.07,.08,.1,6),M(skin));neck.position.y=.76;
  const sL=new THREE.Mesh(new THREE.SphereGeometry(.11,8,6),M(shirt)),sR=sL.clone();sL.position.set(-.3,.66,0);sR.position.set(.3,.66,0);
  body.add(belt,neck,sL,sR);
  if(shirt===0xf4f4f6){
    [P.lL,P.lR].forEach((l,i)=>{const st=new THREE.Mesh(new THREE.BoxGeometry(.016,.86,.07),M(0xf37321));st.position.set(i?.118:-.118,-.45,0);l.add(st)});
    const ch=new THREE.Mesh(new THREE.PlaneGeometry(.3,.15),new THREE.MeshBasicMaterial({map:tex(128,64,(c,w,h)=>{c.clearRect(0,0,w,h);c.fillStyle='#f37321';c.font='italic bold 40px serif';c.textAlign='center';c.fillText('Eagles',w/2,44)}),transparent:true}));
    ch.position.set(0,.5,-.262);ch.rotation.y=Math.PI;body.add(ch);
  }
  if(glove){t.material=new THREE.MeshLambertMaterial({map:tex(64,32,(c,w,h)=>{c.fillStyle='#'+shirt.toString(16).padStart(6,'0');c.fillRect(0,0,w,h);c.fillStyle='rgba(30,50,110,.5)';for(let x=3;x<w;x+=8)c.fillRect(x,0,1.5,h)},3,1)})}
  if(cap===shirt||cap===0x17181c||cap===0x4a1414){cp.material=new THREE.MeshPhongMaterial({color:cap,shininess:90});cp.scale.set(1.08,1.05,1.08);const fl=new THREE.Mesh(new THREE.BoxGeometry(.05,.15,.15),cp.material);fl.position.set(.2,.88,-.02);body.add(fl)}
  if(shirt===0x3a3f4d||shirt===0x22252b){
    const gear=new THREE.Mesh(new THREE.BoxGeometry(.3,.22,.07),M(0x2a2a30));gear.position.set(0,.93,-.22);
    const chest=new THREE.Mesh(new THREE.BoxGeometry(.48,.5,.12),M(0x1c1c22));chest.position.set(0,.4,-.2);
    body.add(gear,chest);
  }
  const num=new THREE.Mesh(new THREE.PlaneGeometry(.24,.24),new THREE.MeshBasicMaterial({map:tex(64,64,(c,w,h)=>{c.clearRect(0,0,w,h);c.fillStyle='#fff';c.strokeStyle='#222';c.lineWidth=5;c.font='bold 44px sans-serif';c.textAlign='center';c.textBaseline='middle';const n=String(1+Math.random()*98|0);c.strokeText(n,w/2,h/2+2);c.fillText(n,w/2,h/2+2)}),transparent:true}));
  num.position.set(0,.45,.255);body.add(num);
  g.position.set(x,0,z);
  g.userData={P,mode:'idle',t0:0,ph:Math.random()*6,ready:false,spd:7.6+Math.random()*1.6,mats:[t.material,cp.material,br.material,P.aL.children[0].material,P.aR.children[0].material,sL.material]};
  scene.add(g);HUM.push(g);return g;
}
function setAnim(h,m,n,k){const u=h.userData;u.mode=m;u.t0=n;if(k)u.sig=k}
function animH(h,n){
  const u=h.userData,P=u.P,m=u.mode,t=n-u.t0;
  let aL=0,aR=0,zL=0,zR=0,lL=0,lR=0,ln=0,y=0,ty=0,bry=-1.57,brz=-.6;
  if(m==='run'){const s=Math.sin(n*13);lL=s*.9;lR=-s*.9;aL=-s*.8;aR=s*.8;ln=-.2;y=Math.abs(Math.cos(n*13))*.05}
  else if(m==='throw'){
    const k=Math.min(1,t/.4),w=k<.5?k/.5:1,q=k<.5?0:(k-.5)/.5;
    aR=k<.5?-2.7*w:-2.7+4.5*q;aL=k<.5?1.2*w:1.2-.9*q;lL=k<.5?-.5*w:-.5+1.4*q;lR=k<.5?.3*w:.3*(1-q);
    ln=k<.5?.12*w:.12-.42*q;ty=k<.5?-.7*w:-.7+1.3*q;
    if(t>.8)u.mode=u.base||'idle';
  }
  else if(m==='pitch'){
    if(t<.45){const k=t/.45;lL=1.3*k;aL=k;aR=-.6*k;ln=.15*k}
    else if(t<.9){const k=(t-.45)/.45;lL=1.3-k;aL=1-.5*k;aR=-.6-2*k;ln=.15-.35*k}
    else{const k=Math.min(1,(t-.9)/.25);aR=-2.6+4.4*k;aL=.5;lL=.3*(1-k);ln=-.35;if(t>1.6)u.mode='idle'}
  }
  else if(m==='catch'){aL=1.7;ln=-.2;if(u.base==='squat'){lL=lR=1.35;y=-.52}if(t>.8)u.mode=u.base||'idle'}
  else if(m==='tag'){aL=Math.min(2.6,1+t*5);ln=-.5;lL=.6;lR=-.3;y=-.2;if(t>.6)u.mode=u.base||'idle'}
  else if(m==='slide'){ln=1.1;lL=1.5;lR=.4;y=-.55;aL=aR=-1.6}
  else if(m==='dive'){ln=-1.3;aL=aR=2.6;y=-.35;if(t>.7)u.mode='idle'}
  else if(m==='punch'){const k=Math.min(1,t/.26);aR=k<.4?-.4+k/.4*2.2:1.8-(k-.4)/.6*1.4;aL=.9;ln=-.18*Math.sin(k*3.14);ty=-.5*Math.sin(k*3.14)}
  else if(m==='kick'){const k=Math.min(1,t/.42);lR=k<.5?k/.5*1.7:1.7-(k-.5)/.5*1.7;aL=1.0;aR=-.5;ln=.25*Math.sin(k*3.14)}
  else if(m==='block'){aL=aR=1.9;ln=-.1;lL=lR=.25}
  else if(m==='hurt'){ln=.38;aL=aR=-.4;ty=.25*Math.sin(t*20)}
  else if(m==='fstance'){aL=aR=1.5;ln=-.12;lL=.35;lR=-.2;y=-.05}
  else if(m==='jump'){aL=aR=2.9;y=Math.abs(Math.sin(n*9))*.3}
  else if(m==='squat'){lL=lR=1.35;aL=1.2;aR=.3;y=-.52}
  else if(m==='sig'){
    const k=u.sig;
    if(k==='strike')aR=2.7;else if(k==='out')aR=2.1+Math.sin(t*14)*.35;
    else if(k==='safe'){zL=-1.5;zR=1.5}else if(k==='foul')aL=aR=3;
    else if(k==='hr'){aR=2.7;zR=Math.sin(t*10)*.7}
    if(t>1.4)u.mode='idle';
  }
  else if(m==='bat'){
    const p=(n-swingAt)/.3,e=p<0||p>2?0:Math.min(1,p);
    h.rotation.y=(pitch&&pitch.bunt)?-1.7+.9*e:-1.7+1.4*e;
    if(p<0||p>2){const w=Math.sin(n*5+u.ph);aL=aR=1.15+w*.06;ln=-.12;lL=.2;lR=-.1;ty=-.05;zL=.4;zR=-.4;bry=-1.57+w*.08;brz=-.6+w*.05}
    else if(pitch&&pitch.bunt){aL=aR=1.0;ln=-.35;lL=.5;lR=-.2;ty=-.4;zL=.2;zR=-.2;bry=.9;brz=-1.5}
    else{
      const k=Math.min(1,p),f=p>1?Math.min(1,p-1):0;
      const st=Math.min(1,k/.3),rt=Math.max(0,Math.min(1,(k-.2)/.4)),ex=Math.max(0,Math.min(1,(k-.45)/.4));
      lL=.2+.5*st-.25*ex;lR=-.1-.25*st+.2*rt;
      ln=-.12+.1*st-.22*ex-.05*f;
      ty=-.05-.55*(1-rt)+.5*ex+.4*f;
      aL=aR=1.15+.55*ex+.9*f;zL=.4-.25*ex;zR=-.4+.25*ex;bry=(k<.4?-1.6+1.6*(k/.4):(k-.4)/.6*1.6)+f*.9;brz=-.6-.9*Math.min(1,k/.35)+.5*f;
    }
  }
  else{const r=u.ready;if(r)h.rotation.y=turnTo(h.rotation.y,Math.PI,.12);aL=aR=r?.5:0;lL=lR=r?.3:0;ln=(r?-.28:0)+Math.sin(n*2+u.ph)*.02;y=r?-.07:0}
  const c=u.c||(u.c={aL:0,aR:0,zL:0,zR:0,lL:0,lR:0,ln:0,ty:0,y:0}),dt=Math.min(.1,n-(u.pn||n)),kk=Math.min(1,dt*((m==='throw'||m==='pitch'||m==='bat'||m==='punch'||m==='kick'||m==='hurt')?32:13));u.pn=n;
  c.aL+=(aL-c.aL)*kk;c.aR+=(aR-c.aR)*kk;c.zL+=(zL-c.zL)*kk;c.zR+=(zR-c.zR)*kk;c.lL+=(lL-c.lL)*kk;c.lR+=(lR-c.lR)*kk;c.ln+=(ln-c.ln)*kk;c.ty+=(ty-c.ty)*kk;c.y+=(y-c.y)*kk;
  P.aL.rotation.set(c.aL,0,c.zL);P.aR.rotation.set(c.aR,0,c.zR);P.lL.rotation.x=c.lL;P.lR.rotation.x=c.lR;P.body.rotation.x=c.ln;P.body.rotation.y=c.ty;h.position.y=c.y;
  if(P.kL){
    const run=m==='run',bk=u.ready?.4:.06,sq=m==='squat'?1.4:0;
    P.kL.rotation.x=-(Math.max(0,-c.lL)*1.1+(run?Math.max(0,c.lL)*.25:0)+bk+sq+(m==='slide'?.5:0));
    P.kR.rotation.x=-(Math.max(0,-c.lR)*1.1+(run?Math.max(0,c.lR)*.25:0)+bk+sq+(m==='slide'?.2:0));
    const eb=run?1.1:(m==='bat'||m==='fstance'||m==='block')?1.1:m==='punch'?.3:(m==='throw'||m==='pitch')?.35:.2;
    P.eL.rotation.x=eb+Math.abs(c.aL)*.15;P.eR.rotation.x=eb+Math.abs(c.aR)*.15;
    if(u.bat&&bat.parent===P.eR){u.bs=u.bs||{ry:-1.57,rz:-.6};u.bs.ry+=(bry-u.bs.ry)*kk;u.bs.rz+=(brz-u.bs.rz)*kk;const qf=new THREE.Quaternion().copy(P.aR.quaternion).multiply(P.eR.quaternion).invert();bat.quaternion.copy(qf).multiply(new THREE.Quaternion().setFromEuler(new THREE.Euler(0,u.bs.ry,u.bs.rz)))}
  }
}
function sigFor(t){const k=/홈런/.test(t)?'hr':/스트라이크|헛스윙/.test(t)?'strike':/병살|아웃|삼진/.test(t)?'out':/안타|루타|볼넷/.test(t)?'safe':/파울/.test(t)?'foul':null;if(k)setAnim(ump,'sig',now(),k)}
/* 주루: 베이스 이동 기록(MV) → 주자가 베이스를 따라 달림 */
function pathTo(f,t){const w=[[0,0],...BP,[0,0]],r=[];for(let k=f+1;k<=t+1;k++)r.push(new THREE.Vector3(w[k][0],0,w[k][1]));return r}
function runMoves(){
  MV.forEach(([f,t])=>{
    let h;
    if(f>=0){h=runners[f];runners[f]=null}
    else{const c=G.half?0xc0392b:0xf4f4f6,cp=G.half?0x4a1414:0x17181c;h=human(c,0xf1f1f3,cp,-1,0);h.userData.spd=7.4+Math.random()*1.6+(cb().s-50)*.012;batter.visible=false}
    if(!h)return;
    if(t==='out'){scene.remove(h);return}
    const p=pathTo(f,t);if(f<0)p[0].set(-1,0,0);
    h.userData.run={p,i:1,end:t===3?(f<0?'hr':'gone'):'stay',slide:t>=1&&!MV.some(q=>q[0]<0&&q[1]===3),sp:MV.some(q=>q[0]<0&&q[1]===3)?10:(h.userData.spd||8.6)};h.userData.mode='run';if(!running.includes(h))running.push(h);
    if(t<3)runners[t]=h;
  });
  MV=[];
}
function stepRunners(dt){
  for(let k=running.length-1;k>=0;k--){
    const h=running[k],r=h.userData.run,g=r.p[r.i],dx=g.x-h.position.x,dz=g.z-h.position.z,d=Math.hypot(dx,dz),s=(r.sp||8.5)*dt;
    if(d<=s){
      h.position.x=g.x;h.position.z=g.z;r.i++;
      if(r.i>=r.p.length){running.splice(k,1);h.userData.run=null;if(r.end==='gone')scene.remove(h);else if(r.end==='hr')celebrate(h);else if(r.end==='jump'){setAnim(h,'jump',now());setTimeout(()=>scene.remove(h),1700)}else{h.rotation.y=0;setAnim(h,'idle',now())}}
    }else{h.position.x+=dx/d*s;h.position.z+=dz/d*s;h.rotation.y=turnTo(h.rotation.y,Math.atan2(-dx,-dz),.25);h.userData.mode=(r.slide&&r.i===r.p.length-1&&d<2.6)?'slide':'run'}
  }
}
/* ---------- 송구 / 도루 / 번트 / 견제 / 세리모니 ---------- */
const tball=new THREE.Mesh(new THREE.SphereGeometry(.14,18,12),new THREE.MeshLambertMaterial({map:ballTex(),emissive:0x2b2b2b}));tball.visible=false;scene.add(tball);
let tq=null,stealArm=false,stealH=null;
function relay(pts,fi){
  const n=now();tq={pts,k:0,t0:n+.22,d:Math.hypot(pts[1][0]-pts[0][0],pts[1][1]-pts[0][1])};tball.visible=true;
  coverFor(pts,fi);{const w=fi!=null&&fielders[fi]?fielders[fi]:whoAt(pts[0][0],pts[0][1]);if(w){facePt(w,pts[1][0],pts[1][1]);setAnim(w,'throw',n)}}
}
function stepThrow(n){
  if(!tq)return;
  const a=tq.pts[tq.k],b=tq.pts[tq.k+1],k=Math.max(0,Math.min(1,(n-tq.t0)/(tq.d/26+.12)));
  tball.position.set(a[0]+(b[0]-a[0])*k,1.6-.6*k+Math.sin(k*Math.PI)*Math.min(5,tq.d*.05),a[1]+(b[1]-a[1])*k);
  tball.scale.setScalar(Math.max(1,cam.position.distanceTo(tball.position)/40));
  if(k>=1){
    tq.k++;{const rc=whoAt(b[0],b[1]);if(rc)setAnim(rc,BS.some(q=>Math.hypot(q[0]-b[0],q[1]-b[1])<1.5)?'tag':'catch',n)}
    if(tq.k>=tq.pts.length-1){tball.visible=false;tq=null}
    else{const a2=tq.pts[tq.k],b2=tq.pts[tq.k+1];tq.t0=n+.25;tq.d=Math.hypot(b2[0]-a2[0],b2[1]-a2[1]);const w=whoAt(a2[0],a2[1]);if(w){facePt(w,b2[0],b2[1]);setAnim(w,'throw',n+.03)}}
  }
}
function whoAt(x,z){let b=null,bd=6;[...fielders,catcher].forEach(h=>{const d=Math.hypot(h.position.x-x,h.position.z-z);if(d<bd){bd=d;b=h}});return b}
function facePt(h,x,z){h.rotation.y=Math.atan2(-(x-h.position.x),-(z-h.position.z))}
function cancelSteal(){
  if(!stealH)return;
  const k=running.indexOf(stealH);if(k>=0)running.splice(k,1);
  stealH.userData.run=null;stealH.position.set(BP[0][0],0,BP[0][1]);setAnim(stealH,'idle',now());stealH=null;
}
function stealGo(){
  if(stealArm&&G.bases[0]&&!G.bases[1]&&runners[0]){
    stealH=runners[0];stealH.userData.run={p:pathTo(0,1),i:1,end:'stay',slide:true,sp:9.2};stealH.userData.mode='run';running.push(stealH);
    {const cv=Math.random()<.5?2:3;FT=F.map(()=>null);FT[cv]=[BS[1][0]*.95,BS[1][1]*.97]}
  }
  stealArm=false;$('st').classList.remove('on');
}
function stealRes(kmh){
  const h=stealH;stealH=null;
  if(!h||runners[0]!==h||!G.bases[0]||G.bases[1]||G.outs>=3||mode==='hit')return;
  relay([[0,2.6],[0,-38.8]]);
  const ok=Math.random()<Math.max(.35,.92-(kmh-100)*.01);
  G.bases[0]=0;runners[0]=null;
  if(ok){G.bases[1]=1;runners[1]=h;say(G.half?'도루 허용!':'도루 성공!',G.half?'red':'gold');hud();later(1.6)}
  else{
    if(h.userData.run)h.userData.run.end='gone';else scene.remove(h);
    G.outs++;say(G.outs>=3?'도루 저지 아웃! 3아웃 공수교대':'도루 저지 아웃!',G.half?'gold':'red');hud();later(G.outs>=3?2.2:1.8);
  }
}
function celebrate(h){
  const c=h.userData.mats[0].color.getHex();
  h.rotation.y=0;setAnim(h,'jump',now());setTimeout(()=>scene.remove(h),1700);
  [[-4,7,-.9,.8],[4,7,.9,.8],[0,9,0,1.4]].forEach(a=>{
    const m=human(c,0xdfe3ea,c,a[0],a[1]);
    m.userData.run={p:[new THREE.Vector3(a[0],0,a[1]),new THREE.Vector3(a[2],0,a[3])],i:1,end:'jump',sp:8};m.userData.mode='run';running.push(m);
  });
}
function mitt(n,p){
  absShow(p);snd('pop');setAnim(catcher,'catch',n);ball.visible=true;ball.position.set(.05,.75,2.3);ball.scale.setScalar(.75);
  if(stealH)setTimeout(()=>stealRes(p.kmh),600);
  if(G.outs<2&&G.bases.some(x=>x)&&p.ty<.3&&Math.random()<.14)setTimeout(()=>wildPitch(p),700);
  setTimeout(()=>{if(mode==='result')ball.visible=false},400);
}
function doBunt(){
  if(G.half===1||mode!=='pitch'||pitch.swung)return;
  pitch.swung=true;pitch.bunt=true;swingAt=now();
}
function stealBtn(){
  if(G.half===1||mode==='over')return;
  if(!G.bases[0]||G.bases[1]){say('도루 불가');setTimeout(()=>{if(mode==='wait')$('msg').className=''},900);return}
  stealArm=!stealArm;$('st').classList.toggle('on',stealArm);
}
function buntHit(d,p){buzz(.3);
  cancelSteal();
  const v=4+Math.random()*6,th=(d*300+(Math.random()-.5)*30)*Math.PI/180,la=(-2+Math.random()*6)*Math.PI/180,vh=v*Math.cos(la);
  play=sim({x:p.tx,y:Math.max(.3,p.ty),z:0},{x:vh*Math.sin(th),y:v*Math.sin(la),z:-vh*Math.cos(th)});
  const r=Math.random(),fair=Math.abs(th)<=.785;
  play.dec={type:'bunt',res:!fair||r<.12?'foul':r<.32?'hit':'out'};
  play.di=Math.min(play.pts.length-1,70);play.t0=now();play.done=false;
  const e=play.pts[play.di];let bi=0,bd=1e9;
  F.forEach((f,i)=>{const dd=Math.hypot(f[0]-e[0],f[1]-e[2]);if(dd<bd){bd=dd;bi=i}});
  play.chaser=bi;if(play.dec.res!=='foul'){play.dec=play.dec.res==='hit'?{type:'hit'}:{type:'out',gb:true,f:bi,t:play.pts.length/60};play.sac=true;planPlay()}assignFielders();
  mode='hit';ball.visible=shadow.visible=true;cam.fov=baseFov();cam.updateProjectionMatrix();fielders[0].visible=true;ret.visible=false;
}
function buntRes(d){
  if(d.res==='foul'){if(G.strikes>=2)strike('번트 파울');else foul();return}
  if(d.res==='hit'){advance(1);G.balls=G.strikes=0;say(G.half?'번트 안타 허용':'번트 안타!',G.half?'red':'gold');hud();later(2.2);return}
  const b=G.bases;MV=[];
  if(G.outs<2)for(let i=2;i>=0;i--)if(b[i]){b[i]=0;if(i+1>=3){G.runs[G.half]++;MV.push([i,3])}else{b[i+1]=1;MV.push([i,i+1])}}
  runMoves();out('희생번트 아웃!');outThrow({gb:true});
}
function outThrow(d){
  const c=play.chaser,f=fielders[c].position,to=d.gb?(c===1?null:[19.4,-19.4]):[0,-18.44];
  if(to){ball.visible=shadow.visible=false;relay([[f.x,f.z],to],c)}
}
function hitThrow(n){
  const c=play.chaser,f=fielders[c];
  setTimeout(()=>{
    const p=[[f.position.x,f.position.z]];
    if(c>=5){const m=F[f.position.x<-12?3:2];p.push([m[0],m[1]]);p.push(n===1?[0,-18.44]:n===2?[0,-38.8]:[-19.4,-19.4])}
    else p.push(n>=2?[0,-38.8]:[0,-18.44]);
    ball.visible=shadow.visible=false;relay(p,c);
  },1300);
}
/* ---------- 실제 야구 규칙 2: 달리기 vs 송구 판정, AI 진루 판단, 보크·폭투·낙아웃·고의사구·교체·런다운 ---------- */
const BS=[[19.4,-19.4],[0,-38.8],[-19.4,-19.4],[0,0]],SN=['1루','2루','3루','홈'];
let pcount=0,cpc=0,poCount=0,pitchedSince=false,phLeft=3,pinch=false,cpuPinch=false,pitchSub=0;
const gauss=()=>Math.random()+Math.random()+Math.random()-1.5;
const at=(s,f)=>setTimeout(f,Math.max(0,s)*1000/TS);
const fat=()=>Math.min(1,Math.max(0,(pcount-18)/30));
function vanish(h){if(h&&h.userData.hold)return;const k=running.indexOf(h);if(k>=0)running.splice(k,1);scene.remove(h)}
function launchRun(f,t,spd,delay,end){
  let h;
  if(f>=0){h=runners[f];runners[f]=null}
  else{const c=G.half?0xc0392b:0xf4f4f6,cp=G.half?0x4a1414:0x17181c;h=human(c,0xf1f1f3,cp,-1,0);h.userData.spd=spd;batter.visible=false}
  if(!h)return null;
  const p=pathTo(f,t);if(f<0)p[0].set(-1,0,0);
  const go=()=>{h.userData.run={p,i:1,end,slide:t>=1,sp:spd};h.userData.mode='run';if(!running.includes(h))running.push(h)};
  if(delay>0)at(delay,go);else go();
  if(end==='stay'&&t<3)runners[t]=h;
  return h;
}
function throwT(c,p,s){const d=Math.hypot(p[0]-BS[s][0],p[1]-BS[s][1]);return(c>=5?.42:.28)+d/(c>=5?31.5:34.5)+(d>55?.32:0)}
function fieldInfo(){
  if(play.fi)return play.fi;const pts=play.pts,d=play.dec,n=pts.length;
  if(d.type==='out'){const e=pts[n-1];return{c:d.f,t:d.t+.15,p:[e[0],e[2]]}}
  for(let i=0;i<n;i++){
    const q=pts[i];if(q[1]>1.6)continue;
    const t=i/60;
    for(let j=0;j<F.length;j++)if(Math.hypot(F[j][0]-q[0],F[j][1]-q[2])/6.1+.3<=t)return{c:j,t:t+.2,p:[q[0],q[2]]};
  }
  const e=pts[n-1],dt=Math.max(1,Math.min(3,n-1)),vx=(e[0]-pts[n-1-dt][0])/dt*60,vz=(e[2]-pts[n-1-dt][2])/dt*60;
  let ex=e[0]+vx,ez=e[2]+vz;const r=Math.hypot(ex,ez);{const rm=Rf(Math.atan2(ex,-ez)*57.2958)-1;if(r>rm){ex*=rm/r;ez*=rm/r}}
  let bt=1e9,bj=0;
  F.forEach((f,j)=>{const tj=Math.hypot(f[0]-ex,f[1]-ez)/6.1+.3;if(tj<bt){bt=tj;bj=j}});
  return{c:bj,t:Math.max(bt,n/60+1)+.2,p:[ex,ez]};
}
function planPlay(){
  play.planned=true;
  const d=play.dec,gb=d.type==='out',GR=!!play.gr,fi=fieldInfo(),c=fi.c,p=fi.p,b=G.bases,outs=G.outs;
  play.chaser=c;
  const err=!!play.err||(!GR&&Math.random()<.03),tf=fi.t+(err&&!play.err?1.3:0);
  const A=s=>tf+throwT(c,p,s)+.15,vb=7.4+Math.random()*1.6+(cb().s-50)*.012;
  const sp=i=>(runners[i]&&runners[i].userData.spd)||7.4;
  const mk=(who,from,to,spd,delay)=>({who,from,to,spd,delay,tR:delay+27.4*(to-from)/spd,out:false,tOut:0,force:false,forced:false});
  const lim=outs===2?-.15:outs===0?.22:.12,thr=gb?.55:lim,go=(m,th)=>m+gauss()*.4>th;
  const M=[];let dpMode=null;
  if(gb&&b[0]&&outs<2&&c<=4&&!play.sac&&!GR){
    const t2=tf+throwT(c,p,1)+.15;
    if(t2<.2+27.4/sp(0)){const tDP=tf+throwT(c,p,1)+.55+27.4/30+.1;dpMode=tDP<.3+27.4/vb?'dp':'fc';play.tDP=tDP}
  }
  if(dpMode){
    const r1=mk('r',0,1,sp(0),.2);r1.out=true;r1.tOut=tf+throwT(c,p,1)+.15;r1.force=true;M.push(r1);
    if(b[1]&&b[2]){const x=mk('r',2,3,sp(2),.2);x.forced=true;M.push(x)}
    if(b[1]){const x=mk('r',1,2,sp(1),.2);x.forced=true;M.push(x)}
    const bm=mk('b',-1,0,vb,.3);bm.forced=true;
    if(dpMode==='dp'){bm.out=true;bm.tOut=play.tDP;bm.force=true}
    M.push(bm);
  }else{
    let cap=3;
    for(let i=2;i>=0;i--){
      if(!b[i])continue;
      const forced=[0,1,2].slice(0,i).every(x=>b[x]),s=sp(i);
      let t=Math.min(GR?i+2:(forced||(play.sac&&outs<2))?i+1:i,cap);
      if(!GR)while(t<cap){const to=t+1;if(go(A(to)-(.2+27.4*(to-i)/s),thr))t=to;else break}
      if(t>i){const m=mk('r',i,t,s,.2);m.forced=forced;M.push(m)}
      cap=t>=3?2:t-1;
    }
    let t=GR?Math.min(1,cap):0;
    if(!GR&&!gb)while(t<cap){const to=t+1;if(go(A(to)-(.3+27.4*(to+1)/vb),lim))t=to;else break}
    const bm=mk('b',-1,t,vb,.3);bm.forced=true;M.push(bm);
  }
  M.forEach(m=>{m.m=A(m.to)-m.tR});
  let tg=null;
  if(!dpMode&&!GR){
    M.forEach(m=>{if(!tg||m.m<tg.m)tg=m});
    if(gb){if(!tg||tg.m>.45)tg=M.find(m=>m.who==='b')}else if(tg&&tg.m>.45)tg=null;
    if(tg&&tg.m<0){
      if(tg.m>-.25&&Math.random()<.2)tg.obs=true;
      else{tg.out=true;tg.tOut=A(tg.to);tg.force=(tg.who==='b'&&tg.to===0)||(tg.forced&&tg.to===tg.from+1)}
    }
  }
  let rev=null,rvh=null;
  if(tg&&!dpMode&&!GR&&!tg.obs&&Math.abs(tg.m)<.15){
    const wrong=Math.random()<.4,callOut=wrong?!tg.out:tg.out,team=callOut?G.half:1-G.half;
    rev={wrong,callOut,team};
  }
  const o0=tg?!!tg.out:false,ot0=tg?tg.tOut:0;
  const build=flip=>{
  if(flip&&tg){tg.out=!o0;tg.tOut=!o0?A(tg.to):0;tg.force=!o0&&((tg.who==='b'&&tg.to===0)||(tg.forced&&tg.to===tg.from+1))}
  const bm=M.find(m=>m.who==='b'),outList=M.filter(m=>m.out),outsAdd=outList.length,third=outs+outsAdd>=3;
  const tOutMin=Math.min(...outList.map(m=>m.tOut),1e9),forceOnly=outList.every(m=>m.force);
  let runs=0;
  M.forEach(m=>{if(!m.out&&m.to===3&&(!third||(!forceOnly&&m.tR<tOutMin)))runs++});
  const nb=[0,0,0];
  for(let i=0;i<3;i++)if(b[i]&&!M.some(m=>m.from===i))nb[i]=1;
  M.forEach(m=>{if(!m.out&&m.to<3)nb[m.to]=1});
  const bl=dpMode==='dp'?'병살타!':dpMode==='fc'?'1루 세이프':bm.out?(gb?(play.sac?'희생번트 아웃!':'땅볼 아웃!'):SN[bm.to]+'에서 아웃!'):err?'실책! 출루':GR?'그라운드룰 2루타!':play.sac?'번트 안타!':gb?'내야 안타!':['안타!','2루타!','3루타!'][bm.to];
  let msg=dpMode==='dp'?(Math.random()<.06?'수비방해! 병살타!':'병살타!'):dpMode==='fc'?'야수 선택! 주자 아웃':bl;
  M.forEach(m=>{if(m.who==='r'&&m.out&&!dpMode)msg+=' · '+SN[m.to]+' 주자 아웃';if(m.obs)msg+=' · 주루방해 세이프'});
  if(runs)msg+=' · '+runs+'점';
  if(third)msg+=' 3아웃! 공수교대';
  const bSafe=!bm.out,col=((G.half===0)===bSafe)?'gold':'red';
  /* 판정 메시지 접두사는 판독 후에 붙임 */
  const Tb=bm.out?bm.tOut:bm.tR,Tf=Math.max(...M.map(m=>m.out?m.tOut:m.tR))+.12;
  if(tg){tg.out=o0;tg.tOut=ot0}
  return{bm,outsAdd,third,runs,nb,bl,msg,col,Tb,Tf};
  };
  const R0=build(false),RC=(rev&&rev.wrong)?build(true):R0;
  const {bm,outsAdd,third,runs,nb,bl,msg,col,Tb,Tf}=RC;
  M.forEach(m=>{
    const h=launchRun(m.from,m.to,m.spd,m.delay,(rev&&m===tg)?'stay':(m.out||m.to===3)?'gone':'stay');if(rev&&m===tg){rvh=h;if(h)h.userData.hold=true}
    if(m.out)at(m.tOut,()=>{if(h)vanish(h)});
  });
  at(tf,()=>{ball.visible=shadow.visible=false;relay(dpMode?[p,BS[1],BS[0]]:[p,tg?BS[tg.to]:[0,-18.44]],c)});
  if(!rev&&Tf-Tb>.5)at(Tb,()=>say(bl,col));
  const ctx={reqd:false,until:0};let tApply=0;
  if(rev){
    const Tc=tg.out?tg.tOut:tg.tR,tOpen=Tc+.6;
    at(Tc,()=>say(SN[tg.to]+(rev.callOut?' 아웃!':' 세이프!'),''));
    if(rev.team===0&&CH[0]>0){at(tOpen,()=>openRq(ctx,rev));tApply=tOpen+5.4}
    else if(rev.team===1&&(rev.wrong||(CH[1]>0&&Math.random()<.3))){ctx.reqd=true;at(tOpen,()=>{ctx.until=now()+3.3;review(rev)});tApply=tOpen+3.4}
    else tApply=tOpen+.4;
  }
  const fin=()=>{
    if(ctx.until&&now()<ctx.until){setTimeout(fin,(ctx.until-now())*1000+60);return}
    const R=ctx.reqd?R0:RC;
    let pre='';
    if(rev){
      const fo=ctx.reqd?o0:rev.callOut;
      if(rvh){rvh.userData.hold=false;if(fo||tg.to===3){vanish(rvh);if(tg.to<3)runners[tg.to]=null}}
      pre=ctx.reqd?(rev.wrong?'판독 결과 번복! ':'판독 결과 판정 유지 · '):(rev.wrong?'판정 확정 · ':'');
    }
    G.bases=R.nb;G.runs[G.half]+=R.runs;G.outs+=R.outsAdd;G.balls=G.strikes=0;
    say(pre+R.msg,R.col);hud();later(R.third?2.4:2.1);
  };
  at(Math.max(Tf,tApply),fin);
}
function planFly(d){
  const e=play.pts[play.pts.length-1],p=[e[0],e[2]],c=d.f,b=G.bases,outs=G.outs+1;
  const infield=c<=4,label=(infield&&b[0]&&b[1]&&G.outs<2)?'인필드 플라이 아웃!':'뜬공 아웃!';
  if(outs>=3||infield||!b.some(x=>x)){out(label);outThrow(d);return}
  G.outs++;G.balls=G.strikes=0;hud();
  say(label,G.half?'gold':'red');
  const A=s=>throwT(c,p,s)+.15,sp=i=>(runners[i]&&runners[i].userData.spd)||7.4,lim=outs===2?-.15:.12;
  const M=[];let cap=3;
  for(let i=2;i>=0;i--){
    if(!b[i])continue;
    const s=sp(i);let t=i;
    while(t<cap){const to=t+1;if(A(to)-(.15+27.4*(to-i)/s)+gauss()*.4>lim)t=to;else break}
    if(t>i)M.push({from:i,to:t,spd:s,tR:.15+27.4*(t-i)/s,out:false,tOut:0,m:0});
    cap=t>=3?2:t-1;
  }
  if(!M.length){outThrow(d);later(2);return}
  M.forEach(m=>{m.m=A(m.to)-m.tR});
  let tg=M.reduce((a,m)=>!a||m.m<a.m?m:a,null);
  if(tg.m>.45)tg=null;
  if(tg&&tg.m<0){if(tg.m>-.25&&Math.random()<.2)tg.obs=true;else{tg.out=true;tg.tOut=A(tg.to)}}
  const outList=M.filter(m=>m.out),outsAdd=outList.length,third=outs+outsAdd>=3,tOutMin=Math.min(...outList.map(m=>m.tOut),1e9);
  let runs=0;M.forEach(m=>{if(!m.out&&m.to===3&&(!third||m.tR<tOutMin))runs++});
  const nb=[0,0,0];
  for(let i=0;i<3;i++)if(b[i]&&!M.some(m=>m.from===i))nb[i]=1;
  M.forEach(m=>{if(!m.out&&m.to<3)nb[m.to]=1});
  let msg=runs?'희생플라이!':outsAdd?'태그업 주자 아웃!':'태그업 진루!';
  if(runs)msg+=' · '+runs+'점';
  if(M.some(m=>m.obs))msg+=' · 주루방해 세이프';
  if(third)msg+=' 3아웃! 공수교대';
  const col=((G.half===0)===!outsAdd)?'gold':'red';
  const Tf=Math.max(...M.map(m=>m.out?m.tOut:m.tR))+.12;
  M.forEach(m=>{
    const h=launchRun(m.from,m.to,m.spd,.15,(m.out||m.to===3)?'gone':'stay');
    if(m.out)at(m.tOut,()=>{if(h)vanish(h)});
  });
  ball.visible=shadow.visible=false;relay([p,tg?BS[tg.to]:[0,-18.44]],c);
  at(Tf,()=>{G.bases=nb;G.runs[G.half]+=runs;G.outs+=outsAdd;say(msg,col);hud();later(third?2.4:2.1)});
}
function flyError(d){
  const e=play.pts[play.pts.length-1];
  play.fi={c:d.f,t:d.t+1.3,p:[e[0],e[2]]};play.err=true;play.dec={type:'hit'};play.sac=false;
  planPlay();
}
function advAll(msg){
  if(G.outs>=3||!G.bases.some(x=>x))return;
  const b=G.bases;MV=[];
  for(let i=2;i>=0;i--)if(b[i]){b[i]=0;if(i+1>=3){G.runs[G.half]++;MV.push([i,3])}else{b[i+1]=1;MV.push([i,i+1])}}
  runMoves();say(msg);hud();later(2);
}
function wildPitch(p){if(mode!=='result')return;advAll((/커브|슬라이더|체인지업/.test(p.name)?'폭투!':'포일!')+' 주자 진루')}
function ibbCpu(){
  if(G.half===0&&G.bases[1]&&!G.bases[0]&&G.outs<2&&G.balls===0&&G.strikes===0&&Math.random()<.2){
    mode='result';paOpen=true;walk();G.balls=G.strikes=0;say('고의사구!');hud();later(1.8);return true;
  }
  return false;
}
function ibbUser(){
  if(mode!=='aim'||running.length)return;
  mode='result';ret.visible=false;paOpen=true;walk();G.balls=G.strikes=0;say('고의사구!');hud();later(1.8);
}
function doPinch(){
  const t=TM[0];
  if(G.half===1||mode!=='wait'||paOpen||!t.bench.length)return;
  const nb=t.bench.shift();t.lineup[G.ord[0]]=nb;
  $('ph').textContent='대타 '+t.bench.length;
  say('대타 '+nb.name+'!');showBar();showPA();
  setTimeout(()=>{if(mode==='wait')$('msg').className=''},1200);
}
function doPinchOld(){
  if(G.half===1||mode!=='wait'||phLeft<=0||pinch)return;
  phLeft--;pinch=true;$('ph').textContent='대타 '+phLeft;
  say('대타 기용!');batter.userData.mats.forEach(m=>m.color.set(0xffd34d));
  setTimeout(()=>{if(mode==='wait')$('msg').className=''},1000);
}
function changePitcherV2(){
  const t=TM[0];
  if(mode!=='aim'||running.length||t.cur>=t.pit.length-1)return;if(!chgOK){say('방금 올라온 투수는 최소 한 명의 타자를 상대해야 합니다.');return}
  t.cur++;chgOK=false;mode='result';ret.visible=false;
  $('pc').textContent='교체 '+(t.pit.length-1-t.cur);
  say('투수 교체! '+curP(0).name+' 등판');later(1.8);
}
function changePitcherOld(){
  if(mode!=='aim'||running.length||pitchSub>=2)return;
  pitchSub++;pcount=0;mode='result';ret.visible=false;
  $('pc').textContent='교체 '+(2-pitchSub);say('투수 교체! 새 투수 등판');later(1.6);
}
function dropped(){
  const safe=Math.random()<.3,vb=7.4+Math.random()*1.6+(cb().s-50)*.012,tb=.3+27.4/vb;
  say('낙아웃! 타자가 1루로 뜁니다');
  if(safe){walk();G.balls=G.strikes=0;hud();at(tb,()=>{say('낙아웃 출루!');later(1.6)});return}
  const h=launchRun(-1,0,vb,.3,'gone');
  at(.7,()=>relay([[0,2.6],[19.4,-19.4]]));
  at(1.9,()=>{if(h)vanish(h);out('낙아웃 아웃!')});
}
function rundown(i,h){
  const a=BS[i],b=BS[Math.min(i+1,3)],P=k=>new THREE.Vector3(a[0]+(b[0]-a[0])*k,0,a[1]+(b[1]-a[1])*k);
  const out=Math.random()<.7,pts=[new THREE.Vector3(h.position.x,0,h.position.z),P(.35),P(.1),P(.4)];
  if(!out)pts.push(P(0));
  let len=0;for(let k=1;k<pts.length;k++)len+=pts[k].distanceTo(pts[k-1]);
  h.userData.run={p:pts,i:1,end:'stay',sp:8.5};h.userData.mode='run';running.push(h);
  const BM=[F[1],F[2],F[4]],fa=BM[i],fb=i<2?BM[i+1]:[0,2.6];
  at(.3,()=>relay([fa,fb,fa,fb]));
  at(len/8.5+.15,()=>{
    if(out){
      vanish(h);runners[i]=null;G.bases[i]=0;G.outs++;
      say(G.outs>=3?'런다운! 아웃 · 3아웃 공수교대':'런다운! 아웃',G.half?'gold':'red');hud();later(G.outs>=3?2.2:1.8);
    }else{say('런다운 탈출! 세이프');hud();later(1.6)}
  });
}
function pickoff(){
  if(mode!=='aim'||running.length||!G.bases.some(x=>x))return;
  const i=G.bases.findIndex(x=>x),h=runners[i],r=Math.random();
  mode='result';ret.visible=false;poCount++;
  if(h)setAnim(h,'dive',now());
  FT=F.map(()=>null);FT[i===0?1:i===1?2:4]=[BS[i][0]*.95,BS[i][1]*.97];relay([F[0],i===0?F[1]:i===1?F[2]:F[4]]);
  if(r<.1){
    G.bases[i]=0;MV=[[i,'out']];runMoves();G.outs++;
    say(G.outs>=3?'견제사! 3아웃 공수교대':'견제사 아웃!','gold');hud();later(G.outs>=3?2.2:1.6);
  }else if(r<.2&&h)rundown(i,h);
  else if(poCount>=4)advAll('보크! 견제 횟수 초과 · 주자 진루');
  else{say('견제 - 세이프');later(.9)}
}
function pickoffOld(){
  if(mode!=='aim'||running.length||!G.bases.some(x=>x))return;
  const i=G.bases.findIndex(x=>x),h=runners[i];
  mode='result';ret.visible=false;
  if(h)setAnim(h,'dive',now());
  if(Math.random()<.12){
    G.bases[i]=0;MV=[[i,'out']];runMoves();G.outs++;
    say(G.outs>=3?'견제사! 3아웃 공수교대':'견제사 아웃!','gold');hud();later(G.outs>=3?2.2:1.6);
  }else{say('견제 - 세이프');later(.9)}
}
function clearRunners(){pinch=false;tq=null;tball.visible=false;stealH=null;runners.forEach(h=>h&&scene.remove(h));runners.fill(null);running.forEach(h=>scene.remove(h));running.length=0;MV=[];batter.visible=true}
function person(c,x,z){
  const g=new THREE.Group();
  const b=new THREE.Mesh(new THREE.CylinderGeometry(.3,.35,1.1,10),M(c));b.position.y=.95;
  const h=new THREE.Mesh(new THREE.SphereGeometry(.22,10,8),M(0xf0c9a0));h.position.y=1.72;
  b.castShadow=h.castShadow=true;g.add(b,h);g.position.set(x,0,z);scene.add(g);return g;
}
/* 수비수: 투수, 1루, 2루, 유격, 3루, 좌익, 중견, 우익 (+x가 1루쪽) */
const F=[[0,-18.44],[22,-22],[9,-34],[-9,-34],[-22,-22],[-42,-65],[0,-78],[42,-65]];
const fielders=F.map(p=>{const h=human(0xe9ecf2,0xc9ced8,0x1d3b72,p[0],p[1],true);h.userData.ready=true;h.rotation.y=Math.PI;return h});
const batter=human(0xf4f4f6,0xf1f1f3,0x17181c,-1,0);batter.userData.mode='bat';batter.rotation.y=-1.7;
const catcher=human(0x3a3f4d,0x3a3f4d,0x3a3f4d,0,2.6,true);catcher.userData.mode='squat';catcher.userData.base='squat';
const ump=human(0x22252b,0x4a4f5a,0x22252b,1.3,3.6);
/* ---------- 경기장 꾸미기 ---------- */
const mk=(g,m,x,y,z)=>{const o=new THREE.Mesh(g,m);o.position.set(x,y,z);scene.add(o);return o};
mk(trackGeo(),new THREE.MeshLambertMaterial({map:dirtT(10),side:THREE.DoubleSide}),0,.03,0);
mk(standsGeo(),new THREE.MeshLambertMaterial({map:tex(512,128,(g,w,h)=>{g.fillStyle='#1a2a52';g.fillRect(0,0,w,h);for(let y=0;y<h;y+=8)for(let x=0;x<w;x+=6){g.fillStyle='hsl('+(Math.random()*360|0)+',45%,'+(35+Math.random()*30|0)+'%)';g.fillRect(x+Math.random()*2,y,4,5)}},5,1),side:THREE.DoubleSide}),0,14,0);
mk(new THREE.BoxGeometry(34,13,2),new THREE.MeshBasicMaterial({map:tex(512,192,(g,w,h)=>{g.fillStyle='#0b1f3a';g.fillRect(0,0,w,h);g.strokeStyle='#ffd34d';g.lineWidth=8;g.strokeRect(6,6,w-12,h-12);g.fillStyle='#ffd34d';g.textAlign='center';g.font='bold 40px sans-serif';g.fillText('대전 한화생명 볌파크',w/2,100);g.fillStyle='#f3f0e4';g.font='32px sans-serif';g.fillText('HANWHA EAGLES',w/2,155)})}),-104,31,-94).lookAt(0,31,0);
[[165,-70],[-150,-100],[85,-170],[-85,-170]].forEach(p=>{mk(new THREE.CylinderGeometry(.5,.8,40,8),M(0x8a8f99),p[0],20,p[1]);mk(new THREE.BoxGeometry(9,5,1),new THREE.MeshBasicMaterial({color:0xfff4c8}),p[0],42,p[1]).lookAt(0,42,0)});
for(const s of[-1,1]){
  mk(new THREE.CylinderGeometry(.12,.12,14,8),M(0xffd34d),s*(s<0?99:95)*.7071,7,-(s<0?99:95)*.7071);
  const bg=new THREE.BufferGeometry().setFromPoints([[.6,-.9],[1.7,-.9],[1.7,.9],[.6,.9]].map(p=>new THREE.Vector3(s*p[0],.09,p[1])));
  scene.add(new THREE.LineLoop(bg,new THREE.LineBasicMaterial({color:0xffffff})));
}
/* ---- 경기장 디테일: 슬라이딩 흙, 백네트, 덕아웃, 구름, 스카이라인, 조명 빛무리 ---- */
[[19.4,-19.4],[0,-38.8],[-19.4,-19.4]].forEach(p=>mk(new THREE.CircleGeometry(3,24),new THREE.MeshLambertMaterial({map:dirtT(1)}),p[0],.045,p[1]).rotation.x=-Math.PI/2);
const netT=tex(64,64,(c,w,h)=>{c.clearRect(0,0,w,h);c.strokeStyle='rgba(30,30,34,.75)';c.lineWidth=1.5;for(let i=0;i<=w;i+=8){c.beginPath();c.moveTo(i,0);c.lineTo(i,h);c.stroke();c.beginPath();c.moveTo(0,i);c.lineTo(w,i);c.stroke()}},12,5);
mk(new THREE.PlaneGeometry(26,10),new THREE.MeshBasicMaterial({map:netT,transparent:true,side:THREE.DoubleSide,depthWrite:false}),0,5,16);
[-13,-6.5,0,6.5,13].forEach(x=>mk(new THREE.CylinderGeometry(.12,.12,10,6),M(0x2b2f36),x,5,16));
for(const s of[-1,1]){
  mk(new THREE.BoxGeometry(14,.8,3.2),M(0x3a3f4a),s*26,.4,-4);
  mk(new THREE.BoxGeometry(14.6,.3,4),M(0x1f2530),s*26,3,-4);
  mk(new THREE.BoxGeometry(14,2.2,.2),M(0x14171d),s*26,1.9,-5.6);
}
const cloudT=tex(128,64,(c,w,h)=>{const g=c.createRadialGradient(w/2,h/2,4,w/2,h/2,w/2);g.addColorStop(0,'rgba(255,255,255,.95)');g.addColorStop(1,'rgba(255,255,255,0)');c.fillStyle=g;c.fillRect(0,0,w,h)});
for(let i=0;i<10;i++){
  const sp=new THREE.Sprite(new THREE.SpriteMaterial({map:cloudT,transparent:true,opacity:0,fog:false,depthWrite:false})),a=Math.PI+(i/9-.5)*2.4;
  sp.position.set(Math.sin(a)*300,70+Math.random()*50,Math.cos(a)*300);sp.scale.set(120+Math.random()*80,40+Math.random()*20,1);scene.add(sp);
}
[[-140,-330,130,60],[40,-360,150,75],[210,-310,110,55],[-260,-300,100,45]].forEach(h=>mk(new THREE.ConeGeometry(h[2],h[3],10),M(0x14202a),h[0],h[3]/2-4,h[1]));
for(let i=0;i<0;i++){
  const a=Math.PI+(i/25-.5)*2.6,r=240+Math.random()*30,hg=15+Math.random()*50;
  mk(new THREE.BoxGeometry(8+Math.random()*10,hg,8+Math.random()*10),M(0x8aa0b8),Math.sin(a)*r,hg/2,Math.cos(a)*r);
}
const glowT=tex(64,64,(c,w,h)=>{const g=c.createRadialGradient(32,32,2,32,32,32);g.addColorStop(0,'rgba(255,248,210,.9)');g.addColorStop(1,'rgba(255,248,210,0)');c.fillStyle=g;c.fillRect(0,0,w,h)});
[[165,-70],[-150,-100],[85,-170],[-85,-170]].forEach(p=>{const s=new THREE.Sprite(new THREE.SpriteMaterial({map:glowT,transparent:true,blending:THREE.AdditiveBlending,depthWrite:false}));s.position.set(p[0],43,p[1]);s.scale.set(44,44,1);scene.add(s)});
mk(new THREE.BoxGeometry(.6,.06,.15),M(0xffffff),0,.33,-18.44);
const bat=new THREE.Group();
const batPts=[[.001,0],[.03,.004],[.045,.02],[.04,.035],[.026,.055],[.022,.08],[.022,.3],[.03,.48],[.043,.62],[.05,.72],[.052,.85],[.05,.95],[.04,.985],[.001,1]].map(a=>new THREE.Vector2(a[0],a[1]));
const batMat=new THREE.MeshPhongMaterial({shininess:70,side:THREE.DoubleSide,map:tex(128,256,(g,w,h)=>{
  g.fillStyle='#d6a96b';g.fillRect(0,0,w,h);
  for(let i=0;i<260;i++){g.fillStyle='rgba(110,70,30,'+(.06+Math.random()*.1)+')';g.fillRect(Math.random()*w,Math.random()*h,1+Math.random()*1.5,12+Math.random()*50)}
  g.fillStyle='#1c1c20';g.fillRect(0,128,w,52);
  g.strokeStyle='rgba(255,255,255,.12)';g.lineWidth=2;
  for(let y=128;y<180;y+=7){g.beginPath();g.moveTo(0,y);g.lineTo(w,y+4);g.stroke()}
  g.fillStyle='#f37321';g.fillRect(0,80,w,5);g.fillRect(0,48,w,5);
  g.fillStyle='#15171c';g.fillRect(0,0,w,10);
})});
const stick=new THREE.Mesh(new THREE.LatheGeometry(batPts,20),batMat);stick.castShadow=true;bat.add(stick);
bat.position.set(-.7,1.25,.1);scene.add(bat);
const ball=new THREE.Mesh(new THREE.SphereGeometry(.17,24,16),new THREE.MeshLambertMaterial({map:ballTex(),emissive:0x2b2b2b}));ball.castShadow=true;scene.add(ball);
const shadow=flat(new THREE.Mesh(new THREE.CircleGeometry(.25,12),new THREE.MeshBasicMaterial({color:0,transparent:true,opacity:.35})));
shadow.position.y=.06;scene.add(shadow);
ball.visible=shadow.visible=false;

/* ---------- 게임 상태 ---------- */
const TYPES={
  "직구":{lo:130,hi:145,mv:[0,.05]},
  "슬라이더":{lo:110,hi:120,mv:[-.7,-.25]},
  "커브":{lo:100,hi:110,mv:[.15,-.95]},
  "체인지업":{lo:120,hi:130,mv:[.06,-.38]}
};
let G,mode='wait',waitAt=0,pitch=null,swingAt=-9,nextAt=0,play=null;
function newGame(){
  phLeft=3;pitchSub=0;pcount=0;cpc=0;pinch=false;$('ph').textContent='대타 3';$('pc').textContent='투수교체';clearRunners();G={inn:1,half:0,runs:[0,0],outs:0,balls:0,strikes:0,bases:[0,0,0],ord:[0,0]};paOpen=false;lastMsg='';CH=[2,2];chgOK=true;
  $('end').classList.remove('on');startWait();
}
const dots=(n,m)=>'●'.repeat(Math.min(n,m))+'○'.repeat(Math.max(0,m-n));
function hud(){paHook();showBar();
  $('role').textContent=G.half?'수비':'공격';
  $('inn').innerHTML='<b>'+G.inn+'</b><i>'+(G.half?'▼':'▲')+'</i>'+(chall?'<small>챌린지</small>':'');
  $('sp').textContent=G.runs[0];$('sc').textContent=G.runs[1];
  $('cnt').innerHTML='<div class="c1">'+G.balls+' - '+G.strikes+'</div><div class="c2">'+G.outs+' OUTS</div>';
  ['b1','b2','b3'].forEach((id,i)=>$(id).classList.toggle('on',!!G.bases[i]));
}
function say(t,cls){lastMsg=t;const m=$('msg');m.textContent=t;m.className='show '+(cls||'');sigFor(t)}
const later=s=>{nextAt=now()+s};
function advance(n){
  let r=0;const b=G.bases;MV=[];
  for(let i=2;i>=0;i--)if(b[i]){b[i]=0;if(i+n>=3){r++;MV.push([i,3])}else{b[i+n]=1;MV.push([i,i+n])}}
  if(n>=4){r++;MV.push([-1,3])}else{b[n-1]=1;MV.push([-1,n-1])}
  G.runs[G.half]+=r;runMoves();return r;
}
function walk(){const b=G.bases;MV=[];if(b[0]&&b[1]&&b[2]){G.runs[G.half]++;MV.push([2,3])}if(b[0]&&b[1]){b[2]=1;MV.push([1,2])}if(b[0]){b[1]=1;MV.push([0,1])}b[0]=1;MV.push([-1,0]);runMoves()}
function out(t){
  G.outs++;G.balls=G.strikes=0;
  const c=G.half?'gold':'red';if(G.outs>=3)say(t+' 3아웃! 공수교대',c);else say(t,c);
  hud();later(G.outs>=3?2.2:1.8);
}
function strike(t){
  G.strikes++;
  if(G.strikes>=3){if((!G.bases[0]||G.outs===2)&&Math.random()<(pitch&&/슬라이더|커브/.test(pitch.name)?.12:.05)){dropped();return}out(/헛스윙/.test(t)?'헛스윙 삼진 아웃!':'루킹 삼진 아웃!');return}
  say(t);hud();later(1.4);
}
function ballCall(){
  G.balls++;
  if(G.balls>=4){walk();G.balls=G.strikes=0;say('볼넷!');}else say('볼');
  hud();later(1.4);
}
function foul(){if(G.strikes<2)G.strikes++;say('파울');hud();later(1.6)}
function proceed(){if(mode==='over')return;if(G.half===1&&G.inn>=INNINGS&&G.runs[1]>G.runs[0]){finish();return}if(G.outs>=3)changeSides();else startWait()}
function changeSides(){
  clearRunners();G.outs=0;G.balls=G.strikes=0;G.bases=[0,0,0];
  if(G.half===0){if(G.inn>=INNINGS&&G.runs[1]>G.runs[0]){finish();return}G.half=1;startWait()}
  else{
    G.half=0;G.inn++;
    if(G.inn>INNINGS&&(G.runs[0]!==G.runs[1]||G.inn>(chall?INNINGS:12))){finish();return}
    startWait();
  }
}
function cpuHalf(){
  mode='result';ball.visible=shadow.visible=false;
  const r0=G.runs[1];let o=0;
  while(o<3){
    const x=Math.random();
    if(x<.64)o++;else if(x<.72)walk();else if(x<.89)advance(1);else if(x<.94)advance(2);else if(x<.955)advance(3);else advance(4);
  }
  G.bases=[0,0,0];G.outs=3;hud();
  say('상대 공격 '+(G.runs[1]-r0)+'득점 · 3아웃 공수교대');
  $('pinfo').textContent='상대 공격';later(2.8);
}
function finish(){
  mode='over';if(G.half===0&&G.inn>INNINGS)G.inn--;hud();
  const a=G.runs[0],b=G.runs[1];
  $('res').textContent=a>b?'승리':a<b?'패배':'무승부';
  $('fin').textContent='한화 '+a+' : '+b+' 상대'+(chall?' · 챌린지 '+(a>b?'클리어!':a<b?'실패':'무승부'):'');
  if(chall&&a>b){try{localStorage.setItem('chal_clear',String((+localStorage.getItem('chal_clear')||0)+1))}catch(e){}}
  $('end').classList.add('on');
}

/* ---------- 투구 ---------- */
function startWait(){
  mode=G.half===1?'aim':'wait';pw=false;if(G.balls===0&&G.strikes===0&&pitchedSince){poCount=0;pitchedSince=false;ptrail=[]}waitAt=now();ball.visible=shadow.visible=false;ball.scale.setScalar(.75);setRole();
  $('msg').className='';cpuSub();if(!paOpen)showPA();showBar();hud();
  fielders.forEach((f,i)=>{if(Math.hypot(f.position.x-F[i][0],f.position.z-F[i][1])>25)f.position.set(F[i][0],0,F[i][1])});
}
/* ---------- 투수 모드 (수비) ---------- */
let selType='직구';const aim={x:0,y:.8};
const rc=new THREE.Raycaster(),pl=new THREE.Plane(new THREE.Vector3(0,0,1),0),pt3=new THREE.Vector3(),ndc=new THREE.Vector2();
function setRole(){
  const p=G.half===1;
  $('sw').style.display=p?'none':'';$('pt').style.display=p?'flex':'none';
  $('bt').style.display=$('st').style.display=$('ph').style.display=p?'none':'';$('po').style.display=$('ib').style.display=$('pc').style.display=p?'block':'none';$('az').style.display=p?'block':'none';drawAZ();
  fielders[0].visible=true;ret.visible=p;resetBat();
  fielders.forEach(f=>{f.rotation.y=Math.PI;f.userData.mode='idle'});FT=holdFT();batter.visible=true;
  batter.userData.mats.forEach((m,k)=>m.color.set((k===1||k===2)?(p?0x4a1414:0x17181c):(p?0xc0392b:(pinch?0xffd34d:0xf4f4f6))));
  fielders.forEach(f=>{const m=f.userData.mats;m[0].color.set(p?0xffffff:0xc0392b);[3,4,5].forEach(k=>m[k].color.set(p?0xf4f4f6:0xc0392b));[1,2].forEach(k=>m[k].color.set(p?0xf37321:0x4a1414))});
  $('hint').textContent=p?'구종을 고르고 조준창을 눌러 다른 곳으로 끌고 떼면 투구합니다':'공이 홈플레이트에 오기 직전에 스윙 · 투구당 1번만 (스페이스 / 버튼 / 화면 터치)';
  if(p)$('pinfo').textContent='내 투구 차례';
}
function setAim(e){
  const r=$('c').getBoundingClientRect();
  ndc.set((e.clientX-r.left)/r.width*2-1,-((e.clientY-r.top)/r.height*2-1));
  rc.setFromCamera(ndc,cam);
  if(rc.ray.intersectPlane(pl,pt3)){aim.x=Math.max(-.7,Math.min(.7,pt3.x));aim.y=Math.max(.1,Math.min(1.5,pt3.y));ret.position.set(aim.x,aim.y,.02);drawAZ()}
}
function throwUser(n){mode='wind';ret.visible=false;setAnim(fielders[0],'pitch',n);setTimeout(()=>throwUser2(now()),900/TS)}
function throwUser2(n){
  curP(0).cnt++;pcount++;pitchedSince=true;paOpen=true;const P0=curP(0),T=TYPES[selType],kmh=Math.round(T.lo+Math.random()*(T.hi-T.lo)+P0.vel-fatP(P0)*9);
  const ef=.24*(1.4-P0.ctrl/99*.8)*(1+fatP(P0)*2.2),tx=aim.x+(Math.random()-.5)*ef,ty=aim.y+(Math.random()-.5)*ef;ptrail.push([tx,ty,selType]);drawAZ();
  const S={x:.25,y:1.85,z:-17.4},mv=[T.mv[0]*(.8+P0.brk/250),T.mv[1]*(.8+P0.brk/250)],dur=17.4/(kmh/3.6)*SLOW;
  pitch={name:selType,kmh,S,A:{x:tx-mv[0],y:ty-mv[1]},mv,dur,start:n,tx,ty,user:true};
  if(G.bases[0]&&!G.bases[1]&&Math.random()<.2)stealArm=true;stealGo();mode='pitch';ball.visible=true;ret.visible=false;
  $('pinfo').textContent='투구 중…';
}
function resolveCpu(p){revealPitch(p);
  ball.visible=false;mode='result';if((G.bases[0]||G.bases[1])&&G.outs<2&&Math.random()<.18)p.bunt=true;
  const z=inZone(p.tx,p.ty);
  const edge=Math.abs(p.tx)>.17||p.ty<.6||p.ty>1.0;
  const sw=Math.random()<(z?.8:.3*(1.3-cb().e/165)*(p.name==='직구'?1:1+(50-vsOf(cb()))/160));
  if(!sw){mitt(now(),p);if(z)strike('스트라이크!');else if(p.tx<-.45){walk();G.balls=G.strikes=0;say('몸에 맞는 공 허용');hud();later(1.6)}else ballCall();return}
  swingAt=now()-.1;
  const gs=(Math.random()+Math.random()+Math.random()-1.5)*(cpuPinch?.19:DF[diff].sig)*(edge||!z?1.25:1)*(p.name==='직구'?1:1.45-vsOf(cb())/99*.6);
  if(Math.abs(gs)>=win()){mitt(now(),p);strike('헛스윙 스트라이크!');return}
  if(p.bunt)buntHit(gs,p);else hit(gs,p);return;
  hit((Math.random()*2-1)*.11,p);return;
  if(Math.random()<.22){foul();return}
  const q=Math.random();
  if(q<.58){out(Math.random()<.5?'뜬공 아웃!':'땅볼 아웃!');return}
  const n=q<.82?1:q<.91?2:q<.93?3:4;
  advance(n);G.balls=G.strikes=0;
  say(['','안타 허용','2루타 허용','3루타 허용','홈런 허용'][n],'red');hud();later(2.4);
}
function throwPitch(n){
  cpuPitchMgr();
  if(G.half===0&&G.bases.some(x=>x)&&Math.random()<.01){mode='result';advAll('보크! 주자 진루');return}
  if(ibbCpu())return;
  paOpen=true;const names=Object.keys(TYPES),name=names[Math.random()*4|0],T=TYPES[name];
  const kmh=Math.round(T.lo+Math.random()*(T.hi-T.lo)+curP(1).vel-fatP(curP(1))*9);
  let tx=(Math.random()-.5)*.44,ty=.55+Math.random()*.5;
  if(Math.random()>.5+curP(1).ctrl*.0016){
    if(Math.random()<.5)tx=(Math.random()<.5?-1:1)*(.3+Math.random()*.25);
    else ty=Math.random()<.5?.15+Math.random()*.25:1.2+Math.random()*.25;
  }
  const S={x:.25,y:1.85,z:-17.4},bk=(.75+curP(1).brk/280)*DF[diff].brk,mv=[T.mv[0]*bk,T.mv[1]*bk];
  const dur=17.4/(kmh/3.6)*SLOW;
  pitch={name,kmh,S,A:{x:tx-mv[0],y:ty-mv[1]},mv,dur,start:n,tx,ty};if(autoBat)autoSwing(pitch);
  stealGo();mode='pitch';ball.visible=true;ball.scale.setScalar(.75);
  $('pinfo').textContent='투구 중…';
}
function resolve(n){
  if(pitch.user){resolveCpu(pitch);return}
  const p=pitch,tc=p.start+p.dur,d=swingAt+.12-tc;
  const swung=swingAt>p.start-.2;revealPitch(p);if(swung)showTiming(d);
  const reach=Math.abs(p.tx)<.6&&Math.abs(p.ty-.8)<.6;
  ball.visible=false;
  if(swung&&Math.abs(d)<win()){if(p.bunt)buntHit(d,p);else hit(d,p);return}
  mode='result';
  mitt(n,p);if(swung&&Math.random()<.012){walk();G.balls=G.strikes=0;say('타격방해! 출루');hud();later(1.8)}else if(swung)strike('헛스윙 스트라이크!');
  else if(inZone(p.tx,p.ty))strike('스트라이크!');else if(p.tx<-.45){walk();G.balls=G.strikes=0;say('몸에 맞는 공! 출루');hud();later(1.6)}
  else ballCall();
}

/* ---------- 타구 ---------- */
function hit(d,p){cancelSteal();buzz(1-Math.abs(d)/win());snd('crack');showBf();
  const q=1-Math.abs(d)/win(),v=24+q*18+Math.random()*3+(cb().p-50)*.08-(G.half===1?1.2:0);
  const th=(d*400+(Math.random()-.5)*14)*Math.PI/180;
  const lr=Math.random(),la=Math.max(-12,Math.min(56,(lr<.42?-10+Math.random()*13:lr<.75?24+Math.random()*20:lr<.88?8+Math.random()*12:45+Math.random()*12)+(.8-p.ty)*15))*Math.PI/180;
  const vh=v*Math.cos(la);
  play=sim({x:p.tx,y:Math.max(.3,p.ty),z:0},{x:vh*Math.sin(th),y:v*Math.sin(la),z:-vh*Math.cos(th)});
  play.t0=now();play.done=false;
  const e=play.pts[play.pts.length-1];
  let bi=0,bd=1e9;
  F.forEach((f,i)=>{const dd=Math.hypot(f[0]-e[0],f[1]-e[2]);if(dd<bd){bd=dd;bi=i}});
  play.chaser=play.dec.type==='out'?play.dec.f:bi;if(play.dec.type==='hit'||(play.dec.type==='out'&&play.dec.gb))planPlay();assignFielders();
  mode='hit';ball.visible=shadow.visible=true;cam.fov=baseFov();cam.updateProjectionMatrix();fielders[0].visible=true;ret.visible=false;
}
function sim(p,v){
  const pts=[[p.x,p.y,p.z]];
  let x=p.x,y=p.y,z=p.z,vx=v.x,vy=v.y,vz=v.z,b=0,dec=null,di=0,my=0,wallTh=null,rmax=0,gr=false;
  for(let i=1;i<=420;i++){
    const D=o=>{dec=o;di=i};
    const t=i/60,k=.0021*Math.hypot(vx,vy,vz);
    vx-=vx*k/60;vy-=(vy*k+9.8)/60;vz-=vz*k/60;
    x+=vx/60;y+=vy/60;z+=vz/60;
    const r=Math.hypot(x,z),th=Math.atan2(x,-z)*57.2958;
    /* 수비수 정면: 공이 글러브 높이로 닿는 범위 안이면 아웃 (외야에서 바운드된 뒤에는 불가) */
    if(!dec&&y<=2.6&&!(b>0&&r>45)){
      const rc=1.35+5.5*Math.min(t,3.1);
      for(let j=0;j<F.length;j++)if((b===0||j<5)&&Math.hypot(x-F[j][0],z-F[j][1])<=rc){D({type:'out',f:j,t,gb:b>0});break}
    }
    /* 담장: 노바운드로 넘기면 홈런 */
    if(r>=Rf(th)){
      const over=y>=WHf(th),fair=Math.abs(th)<=45;if(over&&b>0&&fair)gr=true;
      if(!dec)D(over&&b===0?{type:fair?'hr':'foul'}:{type:fair?'hit':'foul'});
      if(!over&&fair&&dec.type!=='hr'){
        const ux=x/r,uz=z/r,vr=vx*ux+vz*uz;
        if(vr>0){vx-=1.25*vr*ux;vz-=1.25*vr*uz;wallTh=th}
      }
    }
    /* 땅 */
    if(y<=.16){
      y=.16;
      if(vy<-1.5){
        b++;vy=-vy*.42;vx*=.85;vz*=.85;
        if(b===1&&!dec&&(z>.5||Math.abs(th)>45))D({type:'foul'});
      }else vy=0;
      vx*=.993;vz*=.993;
    }
    if(!dec&&b>0&&r>45)D({type:'hit'});
    pts.push([x,y,z]);my=Math.max(my,y);rmax=Math.max(rmax,r);
    if(dec&&(dec.type==='out'||i-di>=90))break;
    if(i===360&&!dec)D({type:'hit'});
  }
  if(!dec)dec={type:'hit'};
  return{pts,dec,di:dec.type==='out'?pts.length-1:di,high:my>5,wall:wallTh,rmax,gr};
}
function endReplay(){
  $('rp').style.display='none';$('skip').style.display='none';
  mode='result';ball.visible=shadow.visible=false;later(.3);
}
function startReplay(n){
  mode='replay';play.t0=n;play.rpEnd=n+play.pts.length/60/.7+.8;
  fielders.forEach((f,i)=>f.position.set(F[i][0],0,F[i][1]));
  cam.fov=40;cam.updateProjectionMatrix();look.set(0,2,-20);
  $('msg').className='';$('rp').style.display='block';$('skip').style.display='block';
}
/* ---------- 실제 야구 규칙: 타구 코스별 안타 종류, 태그업, 인필드 플라이, 야수선택, 실책 ---------- */
function basesFor(){
  let m=play.pts[0],mr=0;
  play.pts.forEach(q=>{const r=Math.hypot(q[0],q[2]);if(r>mr){mr=r;m=q}});
  const a=Math.abs(Math.atan2(m[0],-m[2])*57.2958),right=m[0]>0,gap=a>12,line=a>38;
  if(play.gr)return 2;
  if(play.wall!==null){if(!gap)return 2;return right?3:2}
  if(mr>=88&&gap&&right)return 3;
  if(mr>=70&&gap)return 2;
  if(mr>=85)return 2;
  if(line&&mr>=62)return 2;
  return 1;
}
function tagUp(){
  if(G.outs>=2)return false;
  const b=G.bases;MV=[];let s=false;
  if(b[2]){b[2]=0;G.runs[G.half]++;MV.push([2,3]);s=true}
  const e=play.pts[play.pts.length-1];
  if(b[1]&&!b[2]&&Math.hypot(e[0],e[2])>75){b[1]=0;b[2]=1;MV.push([1,2])}
  runMoves();return s;
}
function grAdv(){
  if(G.outs>=2)return;
  const b=G.bases;MV=[];
  if(b[0]&&b[1]&&b[2]){G.runs[G.half]++;b[2]=0;MV.push([2,3])}else if(b[2]&&Math.random()<.5){G.runs[G.half]++;b[2]=0;MV.push([2,3])}
  if(b[0]&&b[1]&&!b[2]){b[2]=1;b[1]=0;MV.push([1,2])}else if(b[1]&&!b[2]&&Math.random()<.5){b[2]=1;b[1]=0;MV.push([1,2])}
  if(b[0]&&!b[1]){b[1]=1;b[0]=0;MV.push([0,1])}
  runMoves();
}
function fc(){
  const b=G.bases;MV=[[0,'out']];b[0]=0;
  if(b[1]&&b[2]){G.runs[G.half]++;b[2]=0;MV.push([2,3])}
  if(b[1]){b[1]=0;b[2]=1;MV.push([1,2])}
  b[0]=1;MV.push([-1,0]);runMoves();
  G.outs++;G.balls=G.strikes=0;
  const f=fielders[play.chaser].position;ball.visible=shadow.visible=false;relay([[f.x,f.z],[0,-38.8]],play.chaser);
  say(G.outs>=3?'야수 선택! 3아웃 공수교대':'야수 선택! 주자 아웃',G.half?'gold':'red');hud();later(G.outs>=3?2.4:2.1);
}
function outPlay(d){
  if(Math.random()<.03&&!d.gb){flyError(d);return}
  const gb=d.gb;
  if(gb&&G.bases[0]&&G.outs<2){const r=Math.random();if(r<.55){dp();return}if(r<.8){fc();return}}
  if(!gb){planFly(d);return}
  if(gb)grAdv();
  const inf=!gb&&G.outs<2&&G.bases[0]&&G.bases[1]&&d.f<=4;
  out(gb?'땅볼 아웃!':inf?'인필드 플라이 아웃!':'뜬공 아웃!');outThrow(d);
}
function dp(){{const c=play.chaser,f=fielders[c].position;ball.visible=shadow.visible=false;relay([[f.x,f.z],[0,-38.8],[19.4,-19.4]],c)}
  MV=[[0,'out']];G.bases[0]=0;G.outs+=2;G.balls=G.strikes=0;
  if(G.outs<3){
    if(G.bases[2]){G.runs[G.half]++;G.bases[2]=0;MV.push([2,3])}
    if(G.bases[1]){G.bases[2]=1;G.bases[1]=0;MV.push([1,2])}
  }
  const c=G.half?'gold':'red';
  say(G.outs>=3?'병살타! 3아웃 공수교대':'병살타!',c);runMoves();hud();later(G.outs>=3?2.4:2.1);
}
function announce(){
  if(play.planned)return;const d=play.dec;if(d.type==='bunt'){buntRes(d);return}
  if(d.type==='out'){outPlay(d)}else if(0){if(0)dp();else{out(d.gb?'땅볼 아웃!':'뜬공 아웃!');outThrow(d)}}
  else if(d.type==='foul')foul();
  else if(d.type==='hr'){const r=advance(4);G.balls=G.strikes=0;say(G.half?'홈런 허용! '+r+'점':((bfl&&bfl.flip)?'빠던! ':'')+'홈런! '+r+'점',G.half?'red':'gold');hud();play.hr=true;snd('cheer')}
  else{
    /* 담장을 직접 맞히면 2루타(좌·우중간 깊은 곳은 3루타), 외야 깊숙이 굴러가면 2루타 */
    let n=1;
    n=basesFor();
    hitThrow(n);
    advance(n);G.balls=G.strikes=0;
    say(G.half?['','안타 허용','2루타 허용','3루타 허용'][n]:['','안타!','2루타!','3루타!'][n],G.half?'red':'gold');hud();later(2.4);
  }
}

/* ---------- 입력 ---------- */
function swing(){
  if(mode==='over')return;
  if(G.half===1||mode!=='pitch'||pitch.swung)return;pitch.swung=true;swingAt=now();
}
addEventListener('keydown',e=>{if(e.code==='Space'||e.code==='Enter'){e.preventDefault();swing()}else if(e.code==='KeyB')doBunt();else if(e.code==='KeyS')stealBtn()});
$('sw').addEventListener('pointerdown',e=>{e.preventDefault();swing()});
$('c').addEventListener('pointerdown',e=>{if(G.half===1){if(mode==='aim'&&!running.length){setAim(e);throwUser(now())}}else swing()});
$('c').addEventListener('pointermove',e=>{if(G.half===1&&mode==='aim')setAim(e)});
$('re').addEventListener('click',toLineup);
$('skip').addEventListener('click',()=>{if(mode==='replay')endReplay()});
$('bt').addEventListener('pointerdown',e=>{e.preventDefault();doBunt()});$('st').addEventListener('click',stealBtn);$('po').addEventListener('click',pickoff);$('ph').addEventListener('click',doPinch);$('ib').addEventListener('click',ibbUser);$('pc').addEventListener('click',changePitcher);
document.querySelectorAll('#pt button').forEach(b=>b.addEventListener('click',()=>{
  selType=b.dataset.t;document.querySelectorAll('#pt button').forEach(x=>x.classList.toggle('on',x===b));
}));

/* ---------- 루프 ---------- */
const look=new THREE.Vector3(0,1,-9);
function homeCam(){
  if(tq)return;const p=G.half===1;cam.fov=p?Math.min(36,baseFov()-16):baseFov();cam.updateProjectionMatrix();
  {const tp=p?[1.8,3.0,-27.5]:[0,1.5,4.2],tl=p?[0,1.0,-2]:[0,1.1,-10];cam.position.lerp(new THREE.Vector3(tp[0],tp[1],tp[2]),.1);look.lerp(new THREE.Vector3(tl[0],tl[1],tl[2]),.1)}
  cam.lookAt(look);
}
/* ---------- 야구공: 가죽 질감 + 빨간 실밥 + 회전 ---------- */
function ballTex(){
  return tex(512,256,(g,w,h)=>{
    g.fillStyle='#f3efe4';g.fillRect(0,0,w,h);
    for(let i=0;i<500;i++){g.fillStyle='rgba(120,100,70,.05)';g.fillRect(Math.random()*w,Math.random()*h,2,2)}
    g.strokeStyle='#b3231c';g.lineWidth=3;
    for(const ph of[0,Math.PI]){
      const y=x=>h/2+h*.3*Math.sin(x/w*Math.PI*2+ph);
      g.beginPath();
      for(let x=0;x<=w;x+=4){if(x)g.lineTo(x,y(x));else g.moveTo(x,y(x))}
      g.stroke();
      for(let x=0;x<w;x+=11){
        const y0=y(x),sl=(y(x+1)-y(x-1))/2,l=Math.hypot(sl,1),nx=-sl/l,ny=1/l;
        g.beginPath();g.moveTo(x-nx*9,y0-ny*9);g.lineTo(x+nx*9,y0+ny*9);g.stroke();
      }
    }
  });
}
const UP=new THREE.Vector3(0,1,0),SPIN={
  '직구':[new THREE.Vector3(1,0,0),45],
  '슬라이더':[new THREE.Vector3(.3,1,0).normalize(),40],
  '커브':[new THREE.Vector3(-1,0,0),38],
  '체인지업':[new THREE.Vector3(1,0,.4).normalize(),14]
};
/* ---------- 타격 진동 ---------- */
/* ---------- 수비 위치 이동: 낙구지점 기준 ---------- */
let FT=null;
function coverFor(pts,c){
  const T=(mode==='hit'&&play&&play.T)?play.T:(FT||(FT=F.map(()=>null)));
  pts.forEach(q=>{
    const s=BS.findIndex(b=>Math.hypot(b[0]-q[0],b[1]-q[1])<1.5);
    if(s<0||s===3)return;
    const tx=BS[s][0]*.95,tz=BS[s][1]*.97;
    if(T.some(t=>t&&Math.hypot(t[0]-tx,t[1]-tz)<.5))return;
    const i=s===0?(c===1?0:1):s===1?(c===2?3:c===3?2:(Math.random()<.5?2:3)):(c===4?3:4);
    T[i]=[tx,tz];
  });
}
/* ---------- 조준창: 투수 시점 정면에서 본 스트라이크 존 ---------- */
const azc=$('azc'),azg=azc.getContext('2d'),AZ_X=.7,AZ_Y0=.1,AZ_Y1=1.5,TC={'직구':'#ff6b5a','슬라이더':'#5ab0ff','커브':'#6be28a','체인지업':'#ffd34d'};
let ptrail=[],azDrag=false;
const azPx=(x,y)=>[(AZ_X-x)/(2*AZ_X)*azc.width,(AZ_Y1-y)/(AZ_Y1-AZ_Y0)*azc.height];
function drawAZ(){
  const w=azc.width,h=azc.height,g=azg;
  g.clearRect(0,0,w,h);g.fillStyle='rgba(255,255,255,.07)';g.fillRect(0,0,w,h);
  const hb=azPx(-.45,1.5);g.fillStyle='rgba(255,90,90,.13)';g.fillRect(hb[0],0,w-hb[0],h);
  const zz=zn(),a=azPx(.25,zz.top),b=azPx(-.25,zz.bot);
  g.fillStyle='rgba(255,255,255,.14)';g.fillRect(a[0],a[1],b[0]-a[0],b[1]-a[1]);
  g.strokeStyle='rgba(255,255,255,.85)';g.lineWidth=3;g.strokeRect(a[0],a[1],b[0]-a[0],b[1]-a[1]);
  g.lineWidth=1;g.strokeStyle='rgba(255,255,255,.4)';
  for(let i=1;i<3;i++){const x=a[0]+(b[0]-a[0])*i/3,y=a[1]+(b[1]-a[1])*i/3;g.beginPath();g.moveTo(x,a[1]);g.lineTo(x,b[1]);g.moveTo(a[0],y);g.lineTo(b[0],y);g.stroke()}
  ptrail.forEach(t=>{const p=azPx(t[0],t[1]);g.fillStyle=TC[t[2]];g.beginPath();g.arc(p[0],p[1],7,0,6.283);g.fill();g.strokeStyle='#000';g.lineWidth=1.5;g.stroke()});
  const q=azPx(aim.x,aim.y);g.strokeStyle='#ffd34d';g.lineWidth=3;g.beginPath();g.arc(q[0],q[1],12,0,6.283);g.moveTo(q[0]-20,q[1]);g.lineTo(q[0]+20,q[1]);g.moveTo(q[0],q[1]-20);g.lineTo(q[0],q[1]+20);g.stroke();
}
function azAim(e){
  const r=azc.getBoundingClientRect();
  aim.x=Math.max(-.7,Math.min(.7,AZ_X-(e.clientX-r.left)/r.width*2*AZ_X));
  aim.y=Math.max(AZ_Y0,Math.min(AZ_Y1,AZ_Y1-(e.clientY-r.top)/r.height*(AZ_Y1-AZ_Y0)));
  ret.position.set(aim.x,aim.y,.02);drawAZ();
}
azc.addEventListener('pointerdown',e=>{if(mode!=='aim'||running.length)return;e.preventDefault();azDrag=true;azc.setPointerCapture(e.pointerId);azAim(e)});
azc.addEventListener('pointermove',e=>{if(azDrag)azAim(e)});
azc.addEventListener('pointerup',e=>{if(!azDrag)return;azDrag=false;azAim(e);if(mode==='aim'&&!running.length)throwUser(now())});
/* ---------- KBO 라인업 · 선수 능력치 · 타순 ---------- */
const SUR='김이박최정강조윤장임한오서신권황안송류홍'.split(''),GIV=['민준','서준','도윤','시우','주원','하준','지호','지훈','준서','준우','현우','도현','건우','우진','선우','연우','유준','정우','승현','승우','시윤','지우','은우','재윤','태윤','민재','성민','동현','영호','상혁'];
const POSN=['포수','1루수','2루수','3루수','유격수','좌익수','중견수','우익수','지명타자'];
let TM=null,paOpen=false,lastMsg='',lnSel=-1;
const rnd=(a,b)=>Math.round(a+Math.random()*(b-a)),fmt=x=>x.toFixed(3).replace(/^0/,''),sgn=v=>(v>=0?'+':'')+v;
const ROLE={lead:[[55,72],[25,45],[65,85],[75,95]],contact:[[68,82],[30,50],[50,70],[55,75]],star:[[78,95],[70,90],[65,85],[45,65]],power:[[55,72],[82,98],[50,70],[30,50]],pow2:[[55,72],[68,85],[45,65],[35,55]],mid:[[48,65],[45,65],[40,60],[40,60]],low1:[[40,58],[30,50],[35,55],[45,65]],low2:[[38,55],[25,45],[30,50],[40,60]],spd:[[42,60],[20,40],[40,60],[70,92]]};
const pname=()=>SUR[rnd(0,SUR.length-1)]+GIV[rnd(0,GIV.length-1)];
function mkBatter(role,pos,d=0){
  const r=ROLE[role],b={name:pname(),pos,h:+(1.7+Math.random()*.2).toFixed(2),c:rnd(...r[0])-d,p:rnd(...r[1])-d,e:rnd(...r[2])-d,s:rnd(...r[3]),g:{ab:0,h:0,bb:0,k:0,hr:0}};
  b.avg=.212+b.c*.0011;b.hr=Math.round(4+(b.p/99)**2*34);
  b.obp=b.avg+.073+(b.e-50)*.0013;b.slg=b.avg+.14+(b.p-50)*.0018;b.ops=b.obp+b.slg;
  return b;
}
function mkPitcher(kind){
  const sp=kind==='SP',cl=kind==='CL';
  const p={name:pname(),vel:cl?rnd(2,5):rnd(-2,4),ctrl:cl?rnd(55,75):sp?rnd(45,80):rnd(40,70),brk:cl?rnd(55,80):sp?rnd(45,80):rnd(40,70),stam:cl?20:sp?rnd(75,105):rnd(25,40),cnt:0,kind};
  p.era=Math.max(2.4,Math.min(5.6,5.2-(p.ctrl+p.brk+p.vel*6)/200*2.2)).toFixed(2);
  return p;
}
function buildTeams(){
  const order=['lead','contact','star','power','pow2','mid','low1','low2','spd'];
  const mkT=d=>{const ps=POSN.slice().sort(()=>Math.random()-.5);return{lineup:order.map((r,i)=>mkBatter(r,ps[i],d)),bench:[mkBatter('contact','대타',d),mkBatter('pow2','대타',d),mkBatter('mid','대타',d)],pit:[mkPitcher('SP'),mkPitcher('RP'),mkPitcher('RP'),mkPitcher('CL')].map(p=>{p.ctrl-=d;p.brk-=d;p.era=Math.max(2.4,Math.min(5.6,5.2-(p.ctrl+p.brk+p.vel*6)/200*2.2)).toFixed(2);return p}),cur:0}};
  TM=[mkT(0),mkT(DF[diff].d)];TM[0].lineup=hwLineup();TM[0].pit=hwPitchers();
  if(DF[diff].bb)TM[1].lineup.concat(TM[1].bench).forEach(b=>{b.c=Math.min(99,b.c+DF[diff].bb);b.p=Math.min(99,b.p+DF[diff].bb);b.e=Math.min(99,b.e+DF[diff].bb);calcB(b)});
}
const curP=t=>TM[t].pit[TM[t].cur],cb=()=>TM[G.half].lineup[G.ord[G.half]];
const fatP=p=>Math.min(1,Math.max(0,(p.cnt-p.stam*.7)/(p.stam*.5)));
const win=()=>.1*(.75+cb().c/200)*(1.1-curP(1-G.half).brk/600)*(G.half===1?.92:DF[diff].win);
function paHook(){
  if(!G||!G.ord||G.balls||G.strikes||!paOpen)return;
  paOpen=false;
  const b=TM[G.half].lineup[G.ord[G.half]],m=lastMsg||'',g=b.g;
  if(/홈런/.test(m)){g.ab++;g.h++;g.hr++}
  else if(/안타|루타/.test(m)){g.ab++;g.h++}
  else if(/삼진|낙아웃/.test(m)){g.ab++;g.k++}
  else if(/볼넷|몸에 맞는|고의사구|타격방해/.test(m))g.bb++;
  else if(!/희생/.test(m))g.ab++;
  G.ord[G.half]=(G.ord[G.half]+1)%9;if(G.half===1)chgOK=true;
}
function showBar(){
  if(!TM||!G||!G.ord)return;setZone();
  const b=cb(),g=b.g,p=curP(1-G.half),o=G.ord[G.half]+1;
  $('bi').innerHTML='<b>'+o+'번 타자</b> '+b.name+' ('+b.pos+') 타율 '+fmt(b.avg)+' HR '+b.hr+' OPS '+fmt(b.ops)+' · 오늘 '+g.ab+'타수 '+g.h+'안타<br><span>투수 '+p.name+' · '+p.cnt+'구 · 구속 '+sgn(p.vel)+' 제구 '+p.ctrl+' 변화구 '+p.brk+'</span>';
}
function showPA(){if(autoOn())return;
  const b=cb(),o=G.ord[G.half]+1;
  $('pa').innerHTML='<b>'+o+'번 타자</b>'+b.name+' ('+b.pos+')<small>타율 '+fmt(b.avg)+' · HR '+b.hr+' · OPS '+fmt(b.ops)+'<br>컨택 '+b.c+' 파워 '+b.p+' 선구 '+b.e+' 주력 '+b.s+' 변화구대처 '+vsOf(b)+'</small>';
  $('pa').className='show';clearTimeout(showPA.t);showPA.t=setTimeout(()=>{$('pa').className=''},2300);
}
function cpuSub(){
  if(G.half!==1||paOpen)return;
  const t=TM[1],b=t.lineup[G.ord[1]];
  if(G.inn>=7&&(G.bases[1]||G.bases[2])&&G.outs<2&&t.bench.length&&Math.random()<.5){
    const nb=t.bench.reduce((a,x)=>(x.c+x.p>a.c+a.p?x:a),t.bench[0]);
    if(nb.c+nb.p>b.c+b.p+10){t.bench.splice(t.bench.indexOf(nb),1);t.lineup[G.ord[1]]=nb;say('상대 대타 '+nb.name);setTimeout(()=>{if(mode==='aim')$('msg').className=''},1600)}
  }
}
function cpuPitchMgr(){
  const t=TM[1],p=curP(1);p.cnt++;
  const lead=G.runs[1]-G.runs[0],last=t.pit.length-1;
  let nx=-1;
  if(G.inn>=9&&lead>0&&lead<=3&&t.cur<last)nx=last;
  else if(t.cur<last&&(p.cnt>p.stam||fatP(p)>.95))nx=t.cur+1;
  if(nx>t.cur){t.cur=nx;say((nx===last?'상대 마무리 ':'상대 투수 교체 ')+curP(1).name);setTimeout(()=>{if(mode==='pitch')$('msg').className=''},1400)}
}
function renderLn(){
  const t=TM[0],c=TM[1],my=t.pit[0],op=c.pit[0];
  const row=(b,i)=>'<div class="lr'+(lnSel===i?' sel':'')+'" data-i="'+i+'"><b>'+(i+1)+'</b><div>'+b.name+' <small>'+b.pos+'</small><i>컨택 '+b.c+' · 파워 '+b.p+' · 선구 '+b.e+' · 주력 '+b.s+' · 변화구 '+vsOf(b)+'</i></div><div style="text-align:right">'+fmt(b.avg)+'<i>HR '+b.hr+' · OPS '+fmt(b.ops)+'</i></div></div>';
  $('lnU').innerHTML=t.lineup.map(row).join('');
  $('lnS').innerHTML='<p class="note"><b>한화 선발</b> '+my.name+' · ERA '+my.era+' · 구속 '+sgn(my.vel)+' · 제구 '+my.ctrl+' · 변화구 '+my.brk+' · 체력 '+my.stam+'구<br><b>상대 선발</b> '+op.name+' · ERA '+op.era+' · 구속 '+sgn(op.vel)+' · 제구 '+op.ctrl+' · 변화구 '+op.brk+'<br><b>상대 타선</b> '+c.lineup.map((b,i)=>(i+1)+' '+b.name).join(' · ')+'</p>';
  $('lnU').querySelectorAll('.lr').forEach(r=>r.onclick=()=>{const i=+r.dataset.i;if(lnSel<0)lnSel=i;else{if(lnSel!==i){const a=t.lineup;[a[lnSel],a[i]]=[a[i],a[lnSel]]}lnSel=-1}renderLn()});
}
function toLineup(){
  buildTeams();G={inn:1,half:0,runs:[0,0],outs:0,balls:0,strikes:0,bases:[0,0,0],ord:[0,0]};
  mode='over';lnSel=-1;renderLn();$('end').classList.remove('on');$('ln').style.display='flex';
}
function showTiming(d){
  const el=$('tm'),w=win(),a=Math.abs(d),ms=Math.round(a*1000);
  let t,c;
  if(a<.03){t='PERFECT';c='#ffd34d'}
  else if(a<w){t=(d<0?'◀ 빠름 ':'늦음 ▶ ')+ms+'ms';c=a<w*.6?'#6be28a':'#ffb347'}
  else{t=(d<0?'◀ 너무 빠름 ':'너무 늦음 ▶ ')+ms+'ms';c='#ff7262'}
  el.textContent=t;el.style.color=c;el.className='show';
  clearTimeout(showTiming.t);showTiming.t=setTimeout(()=>{el.className=''},1100);
}
const DF={
  easy:{d:14,sig:.31,win:1.2,brk:.9,t:'상대 능력치 -14 · 타이밍 범위 넓음 · 상대 변화구 약함'},
  normal:{d:7,sig:.27,win:1,brk:1,t:'상대 능력치 -7 · 기본 난이도'},
  hard:{d:0,sig:.23,win:.9,brk:1.12,t:'상대 능력치 그대로 · 타이밍 범위 좁음 · 상대 변화구 강함'}
};
DF.extreme={d:0,bb:6,sig:.21,win:.86,brk:1.2,t:'상대 타자 능력치 +6 · 타이밍 범위 매우 좁음 · 상대 변화구 매우 강함'};
let diff='normal';
function setDf(d,keep){
  diff=d;
  document.querySelectorAll('#dfr button').forEach(x=>x.classList.toggle('on',x.dataset.d===d));
  $('dfd').textContent=DF[d].t;
  if(keep){const u=TM[0];buildTeams();TM[0]=u;lnSel=-1;renderLn()}
}
/* ---------- ABS(자동 볼·스트라이크) / 비디오 판독 요청 / 한화 로스터 ---------- */
const zn=()=>{const h=(TM&&G&&G.ord)?cb().h:1.8;return{bot:h*.2764-.037,top:h*.5635+.037}};
const inZone=(x,y)=>{const z=zn();return Math.abs(x)<=.253&&y>=z.bot&&y<=z.top};
function setZone(){const z=zn();zone.position.y=(z.bot+z.top)/2;zone.scale.y=(z.top-z.bot)/.7;zoneL.position.y=(z.bot+z.top)/2;zoneL.scale.y=(z.top-z.bot)/.7}
function absShow(p){
  const c=$('absc'),g=c.getContext('2d'),w=c.width,h=c.height,z=zn(),st=inZone(p.tx,p.ty);
  const X=x=>(x+.5)*w,Y=y=>(1.7-y)/1.7*h;
  g.clearRect(0,0,w,h);g.fillStyle='rgba(255,255,255,.08)';g.fillRect(0,0,w,h);
  const x0=X(-.253),x1=X(.253),y0=Y(z.top),y1=Y(z.bot);
  g.strokeStyle='rgba(255,255,255,.9)';g.lineWidth=2;g.strokeRect(x0,y0,x1-x0,y1-y0);
  g.lineWidth=1;g.strokeStyle='rgba(255,255,255,.35)';
  for(let i=1;i<3;i++){g.beginPath();g.moveTo(x0+(x1-x0)*i/3,y0);g.lineTo(x0+(x1-x0)*i/3,y1);g.moveTo(x0,y0+(y1-y0)*i/3);g.lineTo(x1,y0+(y1-y0)*i/3);g.stroke()}
  g.fillStyle=st?'#ff5a4a':'#5ad07a';g.beginPath();g.arc(X(Math.max(-.5,Math.min(.5,p.tx))),Y(Math.max(0,Math.min(1.7,p.ty))),9,0,6.283);g.fill();
  g.strokeStyle='#000';g.lineWidth=1.5;g.stroke();
  $('abst').textContent='ABS '+(st?'스트라이크':'볼');
  const el=$('abs');el.className='show';clearTimeout(absShow.t);absShow.t=setTimeout(()=>{el.className=''},1700);
}
let rqCur=null,rqT=0;
function openRq(ctx,rev){
  const b=$('rq');rqCur={ctx,rev};let s=5;
  b.style.display='block';b.textContent='📹 비디오 판독 요청 (남은 '+CH[0]+'회) '+s;
  clearInterval(rqT);
  rqT=setInterval(()=>{s--;if(!rqCur||s<=0){clearInterval(rqT);b.style.display='none';rqCur=null;return}b.textContent='📹 비디오 판독 요청 (남은 '+CH[0]+'회) '+s},1000);
}
function pressRq(){
  if(!rqCur)return;
  const c=rqCur;rqCur=null;clearInterval(rqT);$('rq').style.display='none';
  c.ctx.reqd=true;c.ctx.until=now()+3.3;review(c.rev);
}
function calcB(b){b.avg=.212+b.c*.0011;b.hr=Math.round(4+(b.p/99)**2*34);b.obp=b.avg+.073+(b.e-50)*.0013;b.slg=b.avg+.14+(b.p-50)*.0018;b.ops=b.obp+b.slg}
function realB(name,pos,h,c,p,e,s){const b=mkBatter('mid',pos);Object.assign(b,{name,h,c,p,e,s});calcB(b);return b}
function hwLineup(){return[
  realB('심우준','유격수',1.80,52,30,48,90),
  realB('문현빈','중견수',1.80,90,48,60,68),
  realB('강백호','지명타자',1.84,84,76,72,42),
  realB('노시환','3루수',1.85,50,80,62,45),
  realB('페라자','우익수',1.85,70,84,66,62),
  realB('채은성','1루수',1.85,58,58,56,32),
  realB('허인서','포수',1.82,62,72,52,35),
  realB('김태연','좌익수',1.78,60,42,50,55),
  realB('이도윤','2루수',1.78,52,30,46,62)
]}
function realP(name,kind,vel,ctrl,brk,stam){const p=mkPitcher(kind);Object.assign(p,{name,vel,ctrl,brk,stam});p.era=Math.max(2.4,Math.min(5.6,5.2-(p.ctrl+p.brk+p.vel*6)/200*2.2)).toFixed(2);return p}
function hwPitchers(){return[
  realP('문동주','SP',5,56,66,95),
  realP('류현진','SP',-2,85,80,90),
  realP('윌켈 에르난데스','SP',2,58,64,90),
  realP('왕예청','SP',1,66,62,90),
  realP('박상원','RP',1,60,62,30),
  realP('정우주','RP',4,48,58,30),
  realP('김서현','CL',5,40,55,20)
]}
/* ---------- 대전 한화생명 볌파크: 비대칭 오각형 외야 ---------- */
function Rf(d){
  const a=Math.max(-45,Math.min(45,d)),P=[[-45,99],[-22.5,115],[0,122],[22.5,112],[45,95]];
  for(let i=0;i<4;i++)if(a<=P[i+1][0])return P[i][1]+(P[i+1][1]-P[i][1])*(a-P[i][0])/(P[i+1][0]-P[i][0]);
  return 95;
}
function WHf(d){return d>=26.5?8:2.4}
function fenceGeo(d0=-45,d1=45){
  const g=new THREE.BufferGeometry(),pos=[],uv=[],idx=[],N=90;
  for(let i=0;i<=N;i++){
    const d=d0+(d1-d0)*i/N,r=Rf(d),a=d*Math.PI/180,x=r*Math.sin(a),z=-r*Math.cos(a),u=1-i/N;
    pos.push(x,0,z,x,WHf(d),z);uv.push(u,0,u,1);
    if(i<N){const k=i*2;idx.push(k,k+1,k+2,k+1,k+3,k+2)}
  }
  g.setAttribute('position',new THREE.Float32BufferAttribute(pos,3));g.setAttribute('uv',new THREE.Float32BufferAttribute(uv,2));
  g.setIndex(idx);g.computeVertexNormals();return g;
}
function trackGeo(){
  const g=new THREE.BufferGeometry(),pos=[],uv=[],idx=[],N=90;
  for(let i=0;i<=N;i++){
    const d=-45+90*i/N,r=Rf(d),a=d*Math.PI/180,s=Math.sin(a),c=Math.cos(a);
    pos.push(r*s,0,-r*c,(r-6)*s,0,-(r-6)*c);uv.push(i/N*10,0,i/N*10,1);
    if(i<N){const k=i*2;idx.push(k,k+1,k+2,k+1,k+3,k+2)}
  }
  g.setAttribute('position',new THREE.Float32BufferAttribute(pos,3));g.setAttribute('uv',new THREE.Float32BufferAttribute(uv,2));
  g.setIndex(idx);g.computeVertexNormals();return g;
}
function standsGeoOld(){
  const g=new THREE.BufferGeometry(),pos=[],uv=[],idx=[],N=96;
  for(let i=0;i<=N;i++){
    const d=-72+144*i/N,rb=Rf(Math.max(-45,Math.min(45,d))),a=d*Math.PI/180,s=Math.sin(a),c=Math.cos(a);
    pos.push((rb+6)*s,-11,-(rb+6)*c,(rb+36)*s,11,-(rb+36)*c);uv.push(i/N,0,i/N,1);
    if(i<N){const k=i*2;idx.push(k,k+1,k+2,k+1,k+3,k+2)}
  }
  g.setAttribute('position',new THREE.Float32BufferAttribute(pos,3));g.setAttribute('uv',new THREE.Float32BufferAttribute(uv,2));
  g.setIndex(idx);g.computeVertexNormals();return g;
}
/* ---------- 부드러운 움직임 · 수비 위치 · 사운드 · 궁적 · 최소 1타자 상대 ---------- */
let chgOK=true,AC=null,sndOn=true;
const TRN=28,trGeo=new THREE.BufferGeometry();
trGeo.setAttribute('position',new THREE.BufferAttribute(new Float32Array(TRN*3),3));
const trail=new THREE.Line(trGeo,new THREE.LineBasicMaterial({color:0xffffff,transparent:true,opacity:.5}));
trail.frustumCulled=false;trail.visible=false;scene.add(trail);
let trp=[];
let chall=false;
function setMode(m){
  chall=m==='chal';INNINGS=chall?3:9;
  document.querySelectorAll('#mdr button').forEach(x=>x.classList.toggle('on',x.dataset.m===m));
  document.querySelectorAll('#dfr button').forEach(b=>{b.disabled=chall});
  if(chall)setDf('extreme',true);
}
function revealPitch(p){$('pinfo').textContent=p.name+' '+p.kmh+'km/h';showPV(p.name,p.kmh)}
function turnTo(cur,tgt,k){const d=Math.atan2(Math.sin(tgt-cur),Math.cos(tgt-cur));return cur+d*k}
function holdFT(){
  const T=F.map(f=>[f[0],f[1]]),b=G.bases,o=G.outs,pw=(TM&&G.ord)?cb().p:50;
  if(pw>75)[5,6,7].forEach(i=>{T[i]=[F[i][0]*1.07,F[i][1]*1.07]});
  else if(pw<35)[5,6,7].forEach(i=>{T[i]=[F[i][0]*.94,F[i][1]*.94]});
  if(b[2]&&o<2&&G.inn>=7)[1,2,3,4].forEach(i=>{T[i]=[F[i][0]*.82,F[i][1]*.82]});
  else if(b[0]&&o<2)[2,3].forEach(i=>{T[i]=[F[i][0]*.82,F[i][1]+2]});
  if(b[0])T[1]=[BS[0][0]*.95,BS[0][1]*.97];
  return T;
}
function snd(k){
  if(!sndOn)return;
  try{
    AC=AC||new (window.AudioContext||window.webkitAudioContext)();
    if(AC.state==='suspended')AC.resume();
    const dur=k==='cheer'?2.2:.14,n=Math.floor(AC.sampleRate*dur),buf=AC.createBuffer(1,n,AC.sampleRate),d=buf.getChannelData(0);
    for(let i=0;i<n;i++){const e=i/n;d[i]=(Math.random()*2-1)*(k==='cheer'?Math.sin(Math.PI*Math.min(1,e*1.2))*.5:Math.pow(1-e,k==='crack'?3:2))}
    const s=AC.createBufferSource(),f=AC.createBiquadFilter(),g=AC.createGain();
    s.buffer=buf;f.type='bandpass';f.frequency.value=k==='crack'?2400:k==='pop'?900:650;f.Q.value=k==='cheer'?.7:1.2;g.gain.value=k==='cheer'?.5:k==='crack'?1:.7;
    s.connect(f);f.connect(g);g.connect(AC.destination);s.start();
  }catch(e){}
}
function showPV(n,k){const e=$('pv');e.innerHTML=n+' <b>'+k+'</b><small>km/h</small>';e.className='show';clearTimeout(showPV.t);showPV.t=setTimeout(()=>{e.className=''},1500)}
function trailStep(b){
  if(b.visible&&(mode==='pitch'||mode==='hit')){trp.push([b.position.x,b.position.y,b.position.z]);if(trp.length>TRN)trp.shift()}else trp.length=0;
  const ta=trGeo.attributes.position.array;
  for(let i=0;i<TRN;i++){const q=trp.length?trp[Math.min(trp.length-1,i)]:[0,-50,0];ta[i*3]=q[0];ta[i*3+1]=q[1];ta[i*3+2]=q[2]}
  trGeo.attributes.position.needsUpdate=true;trail.visible=trp.length>1;
}
/* ---------- 대전 한화생명 볌파크 구조: 먼스터월(8m · 미디어 글라스), 복층 불펜, 3단 관중석, 띠전광판, 4층 지붕 ---------- */
function standsGeo(){
  const g=new THREE.BufferGeometry(),pos=[],uv=[],idx=[],N=96,PR=[[6,-11],[16,-5],[16,-3.5],[26,2],[26,3.5],[36,11]],M2=PR.length;
  for(let i=0;i<=N;i++){
    const d=-72+144*i/N,rb=Rf(Math.max(-45,Math.min(45,d))),a=d*Math.PI/180,s=Math.sin(a),c=Math.cos(a);
    PR.forEach((p,j)=>{pos.push((rb+p[0])*s,p[1],-(rb+p[0])*c);uv.push(i/N,j/(M2-1))});
    if(i<N)for(let j=0;j<M2-1;j++){const a0=i*M2+j,b0=(i+1)*M2+j;idx.push(a0,a0+1,b0,a0+1,b0+1,b0)}
  }
  g.setAttribute('position',new THREE.Float32BufferAttribute(pos,3));g.setAttribute('uv',new THREE.Float32BufferAttribute(uv,2));
  g.setIndex(idx);g.computeVertexNormals();return g;
}
function ringGeo(a0,y0,a1,y1){
  const g=new THREE.BufferGeometry(),pos=[],uv=[],idx=[],N=96;
  for(let i=0;i<=N;i++){
    const d=-72+144*i/N,rb=Rf(Math.max(-45,Math.min(45,d))),a=d*Math.PI/180,s=Math.sin(a),c=Math.cos(a);
    pos.push((rb+a0)*s,y0,-(rb+a0)*c,(rb+a1)*s,y1,-(rb+a1)*c);uv.push(i/N*10,0,i/N*10,1);
    if(i<N){const k=i*2;idx.push(k,k+1,k+2,k+1,k+3,k+2)}
  }
  g.setAttribute('position',new THREE.Float32BufferAttribute(pos,3));g.setAttribute('uv',new THREE.Float32BufferAttribute(uv,2));
  g.setIndex(idx);g.computeVertexNormals();return g;
}
function mwT(){
  return tex(512,128,(g,w,h)=>{
    const gr=g.createLinearGradient(0,0,0,h);gr.addColorStop(0,'#16233f');gr.addColorStop(1,'#0b1226');g.fillStyle=gr;g.fillRect(0,0,w,h);
    g.strokeStyle='rgba(120,180,255,.18)';g.lineWidth=1;
    for(let x=0;x<w;x+=16){g.beginPath();g.moveTo(x,0);g.lineTo(x,h);g.stroke()}
    for(let y=0;y<h;y+=16){g.beginPath();g.moveTo(0,y);g.lineTo(w,y);g.stroke()}
    g.fillStyle='#f37321';g.fillRect(0,0,w,6);
    g.fillStyle='#fff';g.font='bold 40px sans-serif';g.textAlign='center';g.fillText('EAGLES',w/2,78);
  },-1,1);
}
{
  const mw=new THREE.Mesh(fenceGeo(26.5,45),new THREE.MeshPhongMaterial({map:mwT(),side:THREE.DoubleSide,shininess:90}));scene.add(mw);
  const th=36*Math.PI/180,rr=Rf(36)+5.5,bx=rr*Math.sin(th),bz=-rr*Math.cos(th);
  [2,6].forEach((y,i)=>{const b=mk(new THREE.BoxGeometry(30,4,10),M(i?0x3a3f4d:0x2d323d),bx,y,bz);b.lookAt(0,y,0)});
  const ribT=tex(64,16,(g,w,h)=>{g.fillStyle='#f37321';g.fillRect(0,0,w,h);g.fillStyle='rgba(255,255,255,.85)';for(let x=2;x<w;x+=6)g.fillRect(x,5,3,6)},1,1);
  const ribM=new THREE.MeshBasicMaterial({map:ribT,side:THREE.DoubleSide});
  mk(ringGeo(6.3,-10.8,6.3,-9.4),ribM,0,14,0);
  mk(ringGeo(16.2,-4.9,16.2,-3.7),ribM,0,14,0);
  mk(ringGeo(18,13,42,13),new THREE.MeshLambertMaterial({color:0x20242c,side:THREE.DoubleSide}),0,14,0);
}
const zoneL=new THREE.LineLoop(new THREE.BufferGeometry().setFromPoints([new THREE.Vector3(-.25,-.35,0),new THREE.Vector3(.25,-.35,0),new THREE.Vector3(.25,.35,0),new THREE.Vector3(-.25,.35,0)]),new THREE.LineBasicMaterial({color:0xffffff}));
zoneL.position.set(0,.8,.01);scene.add(zoneL);
/* ---------- 빠던 / 벤치 클리어링 ---------- */
let bfl=null,bcOn=false;
function showBf(){
  if(G.half!==0)return;
  dropBat();$('bf').style.display='block';clearTimeout(showBf.t);
  showBf.t=setTimeout(()=>{$('bf').style.display='none'},3000);
}
function flipBatOld(){
  if(bfl||G.half!==0||mode!=='hit')return;
  bfl={vx:-2.4-Math.random()*1.6,vy:5.2,vz:-1.2-Math.random()*1.5,rx:9,ry:4,rz:7,landed:false};
  $('bf').style.display='none';snd('pop');
}
function stepBat(dt){
  if(!bfl||bfl.landed)return;
  bat.position.x+=bfl.vx*dt;bat.position.y+=bfl.vy*dt;bat.position.z+=bfl.vz*dt;bfl.vy-=9.8*dt;
  bat.rotation.x+=bfl.rx*dt;bat.rotation.y+=bfl.ry*dt;bat.rotation.z+=bfl.rz*dt;
  if(bat.position.y<=.06){bat.position.y=.06;bfl.landed=true;bat.rotation.set(0,bat.rotation.y,-1.5708)}
}
function resetBat(){bfl=null;batter.userData.P.eR.add(bat);bat.position.set(0,-.27,0);bat.quaternion.identity()}
function benchClear(){
  if(!(mode==='wait'||mode==='aim')||running.length||bcOn)return;
  bcOn=true;mode='bc';snd('cheer');$('bc').style.display='none';
  say('⚠ 벤치 클리어링!','red');
  const crowd=[];
  for(let k=0;k<16;k++){
    const side=k%2?1:-1,c=side>0?0xf4f4f6:0xc0392b,cp=side>0?0xf37321:0x4a1414;
    const h=human(c,0xf1f1f3,cp,side*26+(Math.random()-.5)*6,-4+(Math.random()-.5)*4);
    const tx=(Math.random()-.5)*7,tz=-17+(Math.random()-.5)*5;
    h.userData.run={p:[h.position.clone(),new THREE.Vector3(tx,0,tz)],i:1,end:'stay',sp:7+Math.random()*2};
    h.userData.mode='run';running.push(h);crowd.push(h);
  }
  setTimeout(()=>crowd.forEach(h=>setAnim(h,'jump',now())),2600);
  setTimeout(()=>{
    crowd.forEach(h=>vanish(h));
    openFight3D();
  },3200);
}
/* ---------- 벤치 클리어링 격투 미니게임 ---------- */
const FG={on:false,p:[],t:0,k:{},end:0,last:0,ai:0,win:0};
function openFight(){
  const mk2=(x,face,c)=>({x,face,hp:100,st:'idle',tm:0,cd:0,hit:false,c,fl:0});
  FG.p=[mk2(170,1,'#f37321'),mk2(470,-1,'#c0392b')];
  FG.t=40;FG.on=true;FG.k={};FG.end=0;FG.ai=0;FG.last=performance.now();
  $('fg').style.display='flex';requestAnimationFrame(fgLoop);
}
function fgAtk(i,kind){
  const a=FG.p[i];
  if(a.cd>0||a.st!=='idle'||a.hp<=0)return;
  a.st=kind;a.tm=kind==='P'?.24:.38;a.hit=false;a.cd=kind==='P'?.34:.55;
}
function fgDmg(i){
  const a=FG.p[i],b=FG.p[1-i],range=a.st==='P'?62:84,dmg=a.st==='P'?6:10;
  if(a.hit||Math.abs(a.x-b.x)>range)return;
  a.hit=true;
  if(b.st==='B'){b.x+=a.face*6;b.fl=.1;return}
  b.hp=Math.max(0,b.hp-dmg);b.st='H';b.tm=.28;b.x+=a.face*(a.st==='P'?14:26);b.fl=.2;snd('pop');
}
function fgLoop(n){
  if(!FG.on)return;
  const dt=Math.min(.05,(n-FG.last)/1000);FG.last=n;
  const p=FG.p[0],q=FG.p[1];
  if(!FG.end)FG.t-=dt;
  if(!FG.end&&(p.st==='idle'||p.st==='B')){
    const mv=(FG.k.R?1:0)-(FG.k.L?1:0);
    p.x+=mv*170*dt;
    if(FG.k.B&&p.st==='idle'){p.st='B';p.tm=9}
    if(!FG.k.B&&p.st==='B')p.st='idle';
    if(p.st==='idle'){if(FG.k.P)fgAtk(0,'P');else if(FG.k.K)fgAtk(0,'K')}
  }
  FG.ai-=dt;
  if(!FG.end&&(q.st==='idle'||q.st==='B')){
    const d=Math.abs(p.x-q.x);
    if(q.st==='B'&&FG.ai<=0)q.st='idle';
    if(d>86)q.x+=(p.x<q.x?-1:1)*140*dt;
    else if(FG.ai<=0){
      FG.ai=.35+Math.random()*.3;
      const r=Math.random();
      if(p.st==='P'||p.st==='K'){if(r<.5){q.st='B';q.tm=9;FG.ai=.5}}
      else if(r<.45)fgAtk(1,'P');else if(r<.7)fgAtk(1,'K');else if(r<.82){q.st='B';q.tm=9;FG.ai=.5}
    }
  }
  FG.p.forEach((a,i)=>{
    a.cd=Math.max(0,a.cd-dt);a.fl=Math.max(0,a.fl-dt);
    a.face=FG.p[1-i].x>a.x?1:-1;
    a.x=Math.max(40,Math.min(600,a.x));
    if(a.st==='P'||a.st==='K'){
      a.tm-=dt;
      if(!a.hit&&a.tm<(a.st==='P'?.14:.2))fgDmg(i);
      if(a.tm<=0)a.st='idle';
    }else if(a.st==='H'){a.tm-=dt;if(a.tm<=0)a.st='idle'}
  });
  if(Math.abs(p.x-q.x)<34){const m=(34-Math.abs(p.x-q.x))/2;p.x-=p.face*m;q.x-=q.face*m}
  fgDraw();
  if(!FG.end&&(p.hp<=0||q.hp<=0||FG.t<=0)){FG.end=performance.now();FG.win=p.hp>q.hp?1:p.hp<q.hp?-1:0}
  if(FG.end&&performance.now()-FG.end>1800){closeFight(FG.win);return}
  requestAnimationFrame(fgLoop);
}
function drawFighter(g,a){
  const col=(a.fl>0&&a.st==='H')?'#ffffff':a.c;
  g.save();g.translate(a.x,296);g.scale(a.face,1);
  g.fillStyle='#f1f1f3';
  g.fillRect(-12,-44,10,44);
  if(a.st==='K'&&a.tm<.3){g.save();g.translate(4,-44);g.rotate(-1.3);g.fillRect(0,0,10,46);g.restore()}else g.fillRect(2,-44,10,44);
  g.fillStyle=col;g.fillRect(-14,-92,28,50);
  g.fillStyle='#f0c9a0';g.beginPath();g.arc(0,-104,13,0,6.283);g.fill();
  g.fillStyle=a.c==='#f37321'?'#17181c':'#4a1414';g.fillRect(-13,-118,26,8);g.fillRect(4,-112,16,4);
  g.fillStyle=col;
  if(a.st==='P')g.fillRect(8,-86,a.tm>.1?52:30,9);
  else if(a.st==='B'){g.fillRect(8,-90,10,34);g.fillRect(14,-92,8,20)}
  else g.fillRect(8,-84,9,30);
  g.restore();
}
function fgDraw(){
  const c=$('fgc'),g=c.getContext('2d'),w=640,h=360;
  const gr=g.createLinearGradient(0,0,0,h);gr.addColorStop(0,'#0b1530');gr.addColorStop(1,'#1c2a4a');g.fillStyle=gr;g.fillRect(0,0,w,h);
  g.fillStyle='rgba(255,255,255,.06)';for(let i=0;i<w;i+=30)g.fillRect(i,210,16,40);
  g.fillStyle='#1b2a1f';g.fillRect(0,250,w,110);g.fillStyle='#8a5d3a';g.fillRect(0,296,w,64);
  FG.p.forEach(a=>drawFighter(g,a));
  [0,1].forEach(i=>{
    const a=FG.p[i],x=i?w-300:20,bw=280*a.hp/100;
    g.fillStyle='rgba(0,0,0,.6)';g.fillRect(x,16,280,18);
    g.fillStyle=a.c;g.fillRect(i?x+280-bw:x,16,bw,18);
    g.fillStyle='#fff';g.font='14px sans-serif';g.textAlign=i?'right':'left';g.fillText(i?'상대 선수':'한화 선수',i?x+280:x,52);
  });
  g.fillStyle='#fff';g.font='bold 26px sans-serif';g.textAlign='center';g.fillText(Math.max(0,Math.ceil(FG.t)),w/2,36);
  if(FG.end){g.font='bold 54px sans-serif';g.fillStyle='#ffd34d';g.fillText(FG.win>0?'승리!':FG.win<0?'패배…':'무승부',w/2,170)}
}
function fgKey(e,d){
  if(!FG.on)return;
  const k={ArrowLeft:'L',KeyA:'L',ArrowRight:'R',KeyD:'R',KeyJ:'P',KeyK:'K',KeyL:'B'}[e.code];
  if(k){FG.k[k]=d;e.preventDefault()}
}
addEventListener('keydown',e=>fgKey(e,true));
addEventListener('keyup',e=>fgKey(e,false));
document.querySelectorAll('#fgm button').forEach(b=>{
  const k=b.dataset.a;
  b.addEventListener('pointerdown',e=>{e.preventDefault();FG.k[k]=true});
  ['pointerup','pointerleave','pointercancel'].forEach(ev=>b.addEventListener(ev,()=>{FG.k[k]=false}));
});
function closeFight(r){
  FG.on=false;fightCleanup();$('fg').style.display='none';bcOn=false;
  say(r>0?'벤치 클리어링 승리! 한화 선수단이 분위기를 가져왔습니다.':r<0?'벤치 클리어링 패배… 심판이 사태를 수습했습니다.':'무승부로 끝났습니다. 심판이 사태를 수습했습니다.');
  if(r>0)snd('cheer');
  startWait();
}
/* ---------- 고품질 선수 모델 (관절 팔꿈치·무릎, 얼굴, 유니폼 디테일) ---------- */
function human(shirt,pants,cap,x,z,glove){
  const g=new THREE.Group(),P={};
  const ph=c=>new THREE.MeshPhongMaterial({color:c,shininess:14,side:THREE.DoubleSide}),SK=[0xf1c9a2,0xe8b88f,0xd9a47a][Math.random()*3|0];
  const mesh=(geo,mat,px,py,pz,par)=>{const m=new THREE.Mesh(geo,mat);m.position.set(px,py,pz);m.castShadow=true;(par||g).add(m);return m};
  const isHW=shirt===0xf4f4f6,isCPU=shirt===0xc0392b,isCatcher=shirt===0x3a3f4d,isUmp=shirt===0x22252b;
  const helm=cap===shirt||cap===0x17181c||cap===0x4a1414;
  const under=isHW?0xf37321:isCPU?0x4a1414:glove?0x1d3b72:shirt,sock=isHW?0xf37321:isCPU?0x4a1414:0x1d3b72;
  const skinM=ph(SK),capM=ph(cap),brimM=ph(cap),sleeveM=glove?ph(0xffffff):ph(shirt),underM=ph(under),pantsM=ph(pants),sockM=ph(sock),dkM=ph(0x1b1b1f),whM=ph(0xf0f0f0),orM=ph(0xf37321),hairM=ph(0x1d140e);
  const handM=ph(glove?SK:isHW?0xf4f4f6:isCPU?0x222226:SK);
  let torsoM;
  if(glove)torsoM=new THREE.MeshPhongMaterial({side:THREE.DoubleSide,shininess:10,map:tex(64,32,(c,w,h)=>{c.fillStyle='#'+shirt.toString(16).padStart(6,'0');c.fillRect(0,0,w,h);c.fillStyle='rgba(30,50,110,.35)';for(let x=3;x<w;x+=8)c.fillRect(x,0,1.2,h)},3,1)});
  else torsoM=ph(shirt);
  const leg=sx=>{
    const hip=new THREE.Group();hip.position.set(sx*.105,.91,0);g.add(hip);
    mesh(LA([[.001,.22],[.075,.2],[.092,.1],[.085,-.05],[.067,-.2],[.062,-.22],[.001,-.22]],20),pantsM,0,-.22,0,hip);
    const kn=new THREE.Group();kn.position.set(0,-.44,0);hip.add(kn);
    mesh(LA([[.001,.2],[.06,.19],[.066,.1],[.05,-.05],[.045,-.2],[.001,-.2]],20),pantsM,0,-.2,0,kn);
    mesh(new THREE.CylinderGeometry(.052,.046,.13,18),sockM,0,-.34,0,kn);
    const shoe=mesh(new THREE.SphereGeometry(1,18,12),dkM,0,-.43,-.06,kn);shoe.scale.set(.052,.042,.135);
    const sole=mesh(new THREE.SphereGeometry(1,18,8),whM,0,-.455,-.06,kn);sole.scale.set(.056,.016,.14);
    if(isHW){mesh(new THREE.BoxGeometry(.014,.4,.05),orM,sx*.082,-.22,0,hip);mesh(new THREE.BoxGeometry(.014,.3,.05),orM,sx*.062,-.17,0,kn)}
    if(isCatcher)mesh(new THREE.BoxGeometry(.11,.34,.07),ph(0x1c1c22),0,-.2,-.06,kn);
    return[hip,kn];
  };
  const [lL,kL]=leg(-1),[lR,kR]=leg(1);P.lL=lL;P.lR=lR;P.kL=kL;P.kR=kR;
  const body=new THREE.Group();body.position.y=.91;g.add(body);P.body=body;
  const torso=mesh(LA([[.001,-.29],[.19,-.285],[.215,-.22],[.205,-.12],[.215,0],[.245,.12],[.268,.21],[.255,.27],[.12,.295],[.001,.3]],26),torsoM,0,.33,0,body);torso.scale.set(1.12,1,.66);
  
  mesh(new THREE.CylinderGeometry(.205,.205,.04,26),dkM,0,.1,0,body).scale.set(1.12,1,.7);
  mesh(new THREE.BoxGeometry(.04,.03,.012),ph(0xcfd2d8),0,.1,-.15,body);
  mesh(new THREE.CylinderGeometry(.055,.06,.1,18),skinM,0,.68,0,body);
  const col=mesh(new THREE.TorusGeometry(.068,.013,6,14),isHW?orM:ph(isCPU?0x4a1414:0x1d3b72),0,.64,0,body);col.rotation.x=Math.PI/2;
  if(!isCatcher&&!isUmp){
    for(let i=0;i<5;i++)mesh(new THREE.SphereGeometry(.011,6,5),whM,0,.52-i*.09,-.168,body);
    if(isHW)mesh(new THREE.BoxGeometry(.014,.52,.008),orM,0,.36,-.172,body);
  }
  const head=mesh(new THREE.SphereGeometry(.112,30,22),skinM,0,.81,0,body);head.scale.set(.92,1.14,1);
  const eyeM=ph(0xffffff),pupM=ph(0x14110e),browM=ph(0x2a1d14);
  [-1,1].forEach(s=>{
    mesh(new THREE.SphereGeometry(.017,8,6),eyeM,s*.041,.825,-.098,body);
    mesh(new THREE.SphereGeometry(.009,6,5),pupM,s*.041,.825,-.113,body);
    mesh(new THREE.BoxGeometry(.045,.01,.012),browM,s*.041,.855,-.1,body);
    mesh(new THREE.SphereGeometry(.024,8,6),skinM,s*.104,.8,0,body);
  });
  mesh(new THREE.BoxGeometry(.022,.045,.03),skinM,0,.79,-.112,body);
  mesh(new THREE.BoxGeometry(.055,.009,.01),ph(0x8a3a30),0,.745,-.1,body);
  const hair=mesh(new THREE.SphereGeometry(.114,12,10),hairM,0,.82,.022,body);hair.scale.set(1,1.1,1);
  if(helm){
    const hm=mesh(new THREE.SphereGeometry(.135,16,12),capM,0,.835,.005,body);hm.scale.set(1.04,1.05,1.12);
    mesh(new THREE.BoxGeometry(.03,.09,.11),capM,.118,.79,-.01,body);
    mesh(new THREE.CylinderGeometry(.12,.12,.01,14,1,false,Math.PI-.8,1.6),brimM,0,.83,-.06,body);
  }else{
    mesh(new THREE.SphereGeometry(.124,16,10,0,6.2832,0,1.5),capM,0,.835,.004,body);
    const br=mesh(new THREE.CylinderGeometry(.15,.15,.012,18,1,false,Math.PI-1.15,2.3),brimM,0,.84,-.04,body);br.rotation.x=-.1;
  }
  const arm=sx=>{
    const sh=new THREE.Group();sh.position.set(sx*.3,.56,0);body.add(sh);
    mesh(new THREE.SphereGeometry(.07,18,14),sleeveM,0,0,0,sh);
    mesh(LA([[.001,.14],[.05,.13],[.055,.04],[.046,-.1],[.043,-.14],[.001,-.14]],18),sleeveM,0,-.14,0,sh);
    if(isHW){const cf=mesh(new THREE.TorusGeometry(.05,.01,6,12),orM,0,-.27,0,sh);cf.rotation.x=Math.PI/2}
    const el=new THREE.Group();el.position.set(0,-.28,0);sh.add(el);
    mesh(LA([[.001,.125],[.043,.12],[.042,.05],[.033,-.1],[.03,-.125],[.001,-.125]],18),underM,0,-.125,0,el);
    const hnd=mesh(new THREE.SphereGeometry(.046,18,14),handM,0,-.275,0,el);hnd.scale.set(1,1.15,.85);
    return[sh,el];
  };
  const [aL,eL]=arm(-1),[aR,eR]=arm(1);P.aL=aL;P.aR=aR;P.eL=eL;P.eR=eR;
  if(glove){const mt=mesh(new THREE.SphereGeometry(.085,18,14),ph(0x7a4a22),0,-.3,-.03,eL);mt.scale.set(1.1,1.25,.9)}
  if(isCatcher||isUmp){
    mesh(new THREE.BoxGeometry(.3,.22,.07),ph(0x2a2a30),0,.82,-.12,body);
    mesh(new THREE.BoxGeometry(.48,.5,.12),ph(0x1c1c22),0,.34,-.17,body);
  }
  if(isHW){
    const ch=new THREE.Mesh(new THREE.PlaneGeometry(.3,.15),new THREE.MeshBasicMaterial({map:tex(128,64,(c,w,h)=>{c.clearRect(0,0,w,h);c.fillStyle='#f37321';c.font='italic bold 40px serif';c.textAlign='center';c.fillText('Eagles',w/2,44)}),transparent:true}));
    ch.position.set(0,.44,-.19);ch.rotation.y=Math.PI;body.add(ch);
  }
  const num=new THREE.Mesh(new THREE.PlaneGeometry(.24,.24),new THREE.MeshBasicMaterial({map:tex(64,64,(c,w,h)=>{c.clearRect(0,0,w,h);c.fillStyle='#fff';c.strokeStyle='#222';c.lineWidth=5;c.font='bold 44px sans-serif';c.textAlign='center';c.textBaseline='middle';const n=String(1+Math.random()*98|0);c.strokeText(n,w/2,h/2+2);c.fillText(n,w/2,h/2+2)}),transparent:true}));
  num.position.set(0,.4,.19);body.add(num);
  g.position.set(x,0,z);
  g.userData={P,mode:'idle',t0:0,ph:Math.random()*6,ready:false,spd:7.6+Math.random()*1.6,mats:[torsoM,capM,brimM,sleeveM,sleeveM,sleeveM]};
  scene.add(g);HUM.push(g);return g;
}
function LA(pts,seg){return new THREE.LatheGeometry(pts.map(p=>new THREE.Vector2(p[0],p[1])),seg||22)}
/* ---------- 3D 격투 미니게임 / 자동 타격·투구 ---------- */
function vsOf(b){if(b.vs==null)b.vs=Math.max(10,Math.min(99,Math.round(b.c*.5+b.e*.4+10+(Math.random()*20-10))));return b.vs}
let arena=null,autoBat=false,autoPitch=false,autoT=0;
const autoOn=()=>!!(G&&TM&&mode!=='over'&&mode!=='fight'&&((G.half===0&&autoBat)||(G.half===1&&autoPitch)));
function ensureArena(){
  if(arena)return;
  arena=new THREE.Group();arena.position.set(300,0,0);
  const fl=new THREE.Mesh(new THREE.CylinderGeometry(15,15,.3,40),new THREE.MeshPhongMaterial({color:0x8a5d3a}));fl.position.y=-.1;fl.receiveShadow=true;arena.add(fl);
  const rp=new THREE.MeshPhongMaterial({color:0xf37321}),r1=new THREE.Mesh(new THREE.TorusGeometry(14.5,.08,6,48),rp);r1.rotation.x=Math.PI/2;r1.position.y=1.0;arena.add(r1);
  const r2=new THREE.Mesh(new THREE.TorusGeometry(14.5,.08,6,48),rp);r2.rotation.x=Math.PI/2;r2.position.y=1.5;arena.add(r2);
  for(let i=0;i<10;i++){const a=i/10*Math.PI*2,p=new THREE.Mesh(new THREE.CylinderGeometry(.1,.1,1.7,8),new THREE.MeshPhongMaterial({color:0x2a2f3a}));p.position.set(Math.cos(a)*14.5,.85,Math.sin(a)*14.5);arena.add(p)}
  const lt=new THREE.PointLight(0xfff0d8,1.4,70);lt.position.set(0,10,5);arena.add(lt);
  scene.add(arena);
}
function fightCleanup(){document.body.classList.remove('fighting');FG.p.forEach(a=>{if(a.h)scene.remove(a.h)});if(arena)arena.visible=false}
function fgSet(a,m2){if(a.mode!==m2){a.mode=m2;setAnim(a.h,m2,now())}}
function openFight3D(){
  ensureArena();arena.visible=true;
  const a=TM[0].lineup[Math.random()*9|0],b=TM[1].lineup[Math.random()*9|0];
  const mkF=(c,cap,x,rot,nm)=>{const h=human(c,0xf1f1f3,cap,300+x,0);h.rotation.y=rot;h.userData.mode='fstance';return{h,x:300+x,hp:100,st:'idle',tm:0,cd:0,hit:false,face:rot<0?1:-1,nm,mode:'fstance'}};
  FG.p=[mkF(0xf4f4f6,0x17181c,-4,-Math.PI/2,a.name+' ('+a.pos+')'),mkF(0xc0392b,0x4a1414,4,Math.PI/2,b.name+' ('+b.pos+')')];
  $('fn1').textContent=FG.p[0].nm;$('fn2').textContent=FG.p[1].nm;
  FG.t=40;FG.on=true;FG.k={};FG.end=0;FG.ai=0;FG.last=performance.now();
  ['msg','pa','tm','vr','abs','pv'].forEach(id=>{const e=$(id);if(e)e.className=''});
  mode='fight';document.body.classList.add('fighting');$('fg').style.display='flex';requestAnimationFrame(fgLoop3);
}
function fgAtk3(i,kind){
  const a=FG.p[i];
  if(a.cd>0||a.st!=='idle'||a.hp<=0)return;
  a.st=kind;a.tm=kind==='P'?.26:.42;a.hit=false;a.cd=kind==='P'?.36:.58;fgSet(a,kind==='P'?'punch':'kick');
}
function fgDmg3(i){
  const a=FG.p[i],b=FG.p[1-i],rg=a.st==='P'?1.15:1.55,dmg=a.st==='P'?6:10;
  if(a.hit||Math.abs(a.x-b.x)>rg)return;
  a.hit=true;
  if(b.st==='B'){b.x+=a.face*.12;return}
  b.hp=Math.max(0,b.hp-dmg);b.st='H';b.tm=.3;b.x+=a.face*(a.st==='P'?.25:.5);fgSet(b,'hurt');snd('pop');
}
function fgUI(){
  $('fh1').style.width=FG.p[0].hp+'%';$('fh2').style.width=FG.p[1].hp+'%';
  $('fgt').textContent=FG.end?(FG.win>0?'승리!':FG.win<0?'패배…':'무승부'):Math.max(0,Math.ceil(FG.t));
}
function fgLoop3(n){
  if(!FG.on)return;
  const dt=Math.min(.05,(n-FG.last)/1000);FG.last=n;
  const p=FG.p[0],q=FG.p[1];
  if(!FG.end)FG.t-=dt;
  let pm=false,qm=false;
  if(!FG.end&&(p.st==='idle'||p.st==='B')){
    const mv=(FG.k.R?1:0)-(FG.k.L?1:0);
    if(mv){p.x+=mv*3.2*dt;pm=true}
    if(FG.k.B&&p.st==='idle')p.st='B';
    if(!FG.k.B&&p.st==='B')p.st='idle';
    if(p.st==='idle'){if(FG.k.P)fgAtk3(0,'P');else if(FG.k.K)fgAtk3(0,'K')}
  }
  FG.ai-=dt;
  if(!FG.end&&(q.st==='idle'||q.st==='B')){
    const d=Math.abs(p.x-q.x);
    if(q.st==='B'&&FG.ai<=0)q.st='idle';
    if(d>1.5){q.x+=(p.x<q.x?-1:1)*2.6*dt;qm=true}
    else if(FG.ai<=0){
      FG.ai=.35+Math.random()*.3;
      const r=Math.random();
      if(p.st==='P'||p.st==='K'){if(r<.5){q.st='B';FG.ai=.5}}
      else if(r<.45)fgAtk3(1,'P');else if(r<.7)fgAtk3(1,'K');else if(r<.82){q.st='B';FG.ai=.5}
    }
  }
  FG.p.forEach((a,i)=>{
    a.cd=Math.max(0,a.cd-dt);
    a.x=Math.max(294.5,Math.min(305.5,a.x));
    a.face=FG.p[1-i].x>a.x?1:-1;
    if(a.hp>0)a.h.rotation.y=a.face>0?-Math.PI/2:Math.PI/2;
    if(a.st==='P'||a.st==='K'){a.tm-=dt;if(!a.hit&&a.tm<(a.st==='P'?.15:.22))fgDmg3(i);if(a.tm<=0)a.st='idle'}
    else if(a.st==='H'){a.tm-=dt;if(a.tm<=0)a.st='idle'}
    if(a.hp>0){
      if(a.st==='P')fgSet(a,'punch');else if(a.st==='K')fgSet(a,'kick');else if(a.st==='B')fgSet(a,'block');else if(a.st==='H')fgSet(a,'hurt');
      else fgSet(a,(i===0?pm:qm)?'run':'fstance');
    }
    a.h.position.x=a.x;
  });
  if(Math.abs(p.x-q.x)<.85){const m=(.85-Math.abs(p.x-q.x))/2;p.x-=p.face*m;q.x-=q.face*m}
  fgUI();
  if(!FG.end&&(p.hp<=0||q.hp<=0||FG.t<=0)){
    FG.end=performance.now();FG.win=p.hp>q.hp?1:p.hp<q.hp?-1:0;
    const l=FG.win>0?q:FG.win<0?p:null,w=FG.win>0?p:FG.win<0?q:null;
    if(l){l.fall=1;l.h.userData.mode='idle'}
    if(w)setAnim(w.h,'jump',now());
  }
  if(FG.end)FG.p.forEach(a=>{if(a.fall){const pr=Math.min(1,(performance.now()-FG.end)/450);a.h.rotation.z=(a.face>0?1:-1)*pr*1.45;a.h.userData.mode='idle'}});
  if(FG.end&&performance.now()-FG.end>2200){closeFight(FG.win);return}
  requestAnimationFrame(fgLoop3);
}
function autoSwing(p){
  const z=inZone(p.tx,p.ty),sw=Math.random()<(z?.82:.28*(1.3-cb().e/165));
  if(!sw)return;
  const g=(Math.random()+Math.random()+Math.random()-1.5)*(z?.2:.25)*(p.name==='직구'?1:1.45-vsOf(cb())/99*.6);
  p.swung=true;swingAt=p.start+p.dur+g-.12;
}
function autoThrow(){
  selType=['직구','슬라이더','커브','체인지업'][Math.random()*4|0];
  const z=zn();aim.x=(Math.random()-.5)*.44;aim.y=z.bot+.08+Math.random()*(z.top-z.bot-.16);
  drawAZ();throwUser(now());
}
/* ---------- 배트를 손에 쥐는 타격 폼 ---------- */
batter.userData.bat=true;batter.userData.P.eR.add(bat);bat.position.set(0,-.27,0);
function dropBat(){
  if(bfl||bat.parent!==batter.userData.P.eR)return;
  scene.attach(bat);
  bfl={vx:-.6,vy:1.2,vz:.5,rx:2.5,ry:1.2,rz:3,landed:false,flip:false};
}
function flipBat(){
  if(!bfl||bfl.flip||G.half!==0)return;bfl.landed=false;bat.position.y=Math.max(bat.position.y,.7);
  Object.assign(bfl,{vx:-2.4-Math.random()*1.6,vy:5.2,vz:-1.2-Math.random()*1.5,rx:9,ry:4,rz:7,flip:true});
  $('bf').style.display='none';snd('pop');
}
/* ---------- 투수 교체: 등록 투수 중 고르기 (횟수 제한 없음) ---------- */
function changePitcher(){
  if(mode!=='aim'||running.length)return;
  if(!chgOK){say('방금 올라온 투수는 최소 한 명의 타자를 상대해야 합니다.');return}
  const t=TM[0],KN={SP:'선발',RP:'중간',CL:'마무리'};
  const rows=t.pit.map((p,i)=>{
    const f=fatP(p),cur=i===t.cur;
    return '<button data-pi="'+i+'" style="display:block;width:100%;text-align:left;margin:0 0 6px;padding:8px 10px;'+(cur?'border-color:var(--lamp);opacity:.6':'')+'"><b style="font-weight:400">'+p.name+'</b> <small style="color:var(--dim)">'+KN[p.kind]+(cur?' · 현재 투수':'')+'</small><br><small style="color:var(--dim)">구속 '+sgn(p.vel)+' · 제구 '+p.ctrl+' · 변화구 '+p.brk+' · 투구수 '+p.cnt+'/'+p.stam+(f>.5?' · 피로':'')+'</small></button>';
  }).join('');
  modal('<h3>투수 교체</h3><p style="font-size:13px;color:var(--dim)">올릴 투수를 고르세요. 교체 횟수는 제한이 없고, 올라온 투수는 최소 한 명의 타자를 상대해야 합니다.</p>'+rows);
}
function selectPitcher(i){
  const t=TM[0];
  if(mode!=='aim'||running.length||i===t.cur||!t.pit[i])return;
  t.cur=i;chgOK=false;mode='result';ret.visible=false;closeModal();
  say('투수 교체! '+curP(0).name+' 등판');later(1.8);showBar();
}
$('mdc').addEventListener('click',e=>{const b=e.target.closest('[data-pi]');if(b)selectPitcher(+b.dataset.pi)});
let CH=[2,2];
function review(rv){
  const el=$('vr'),nm=rv.team===0?'한화':'상대';
  el.style.color='';el.textContent='📹 비디오 판독 중… ('+nm+' 요청 · 남은 '+CH[rv.team]+'회)';el.className='show';
  setTimeout(()=>{
    if(!rv.wrong)CH[rv.team]=Math.max(0,CH[rv.team]-1);
    el.textContent=rv.wrong?'📹 판정 번복!':'📹 판정 유지';el.style.color=rv.wrong?'#ffd34d':'#ff7262';
  },2000);
  setTimeout(()=>{el.className=''},3200);
}
function moveTo(f,t,s){
  if(!t)return;
  const dx=t[0]-f.position.x,dz=t[1]-f.position.z,d=Math.hypot(dx,dz);
  if(d>.3){const k=Math.min(d,s);f.position.x+=dx/d*k;f.position.z+=dz/d*k;f.userData.mode='run';f.rotation.y=turnTo(f.rotation.y,Math.atan2(-dx,-dz),.22)}
  else if(f.userData.mode==='run')f.userData.mode='idle';
}
function assignFielders(){
  const pts=play.pts,gi=pts.findIndex((q,i)=>i>3&&q[1]<=.2);
  const L=gi>=0?pts[gi]:pts[pts.length-1];play.L=L;
  const lx=L[0],lz=L[2],far=Math.hypot(lx,lz),c=play.chaser,T=F.map(f=>[f[0],f[1]]);
  const cov=(i,s)=>{T[i]=[BS[s][0]*.95,BS[s][1]*.97]};
  const others=[5,6,7].filter(i=>i!==c).sort((a,b)=>Math.hypot(F[a][0]-lx,F[a][1]-lz)-Math.hypot(F[b][0]-lx,F[b][1]-lz));
  others.forEach((i,k)=>{
    if(k===0&&c>=5){const m=1+10/Math.max(30,far);T[i]=[lx*m,lz*m]}
    else T[i]=[F[i][0]+(lx-F[i][0])*.3,F[i][1]+(lz-F[i][1])*.3];
  });
  const left=lx<0,cut=far>60?(left?3:2):-1;
  if(cut>=0&&c>=5)T[cut]=[lx/far*38,lz/far*38];
  if(c!==1)cov(1,0);else cov(0,0);
  let cv=left?2:3;
  if(cv===c||cv===cut)cv=cv===2?3:2;
  if(cv!==c&&cv!==cut)cov(cv,1);
  if(c!==4&&far>40)cov(4,2);
  T.forEach(t=>{const r=Math.hypot(t[0],t[1]),rm=Rf(Math.atan2(t[0],-t[1])*57.2958)-1.3;if(r>rm){t[0]*=rm/r;t[1]*=rm/r}});
  play.T=T;
}
function buzz(q){
  if(G.half===1)return;
  try{
    if(navigator.vibrate)navigator.vibrate(q>.7?[70,30,50]:q>.35?50:28);
    else $('c').animate([{transform:'translate(0,0)'},{transform:'translate(-4px,3px)'},{transform:'translate(3px,-3px)'},{transform:'translate(0,0)'}],{duration:140});
  }catch(e){}
}
function spinBall(dt){
  const b=ball,pv=b.userData.pv||(b.userData.pv=b.position.clone());
  if(b.visible&&dt>0){
    if(mode==='pitch'&&pitch){const s=SPIN[pitch.name];if(s)b.rotateOnWorldAxis(s[0],s[1]*dt)}
    else if(mode==='hit'||mode==='replay'){
      const v=new THREE.Vector3().subVectors(b.position,pv),l=v.length();
      if(l>1e-4){
        const ax=v.normalize().cross(UP),roll=b.position.y<.3;
        if(ax.lengthSq()>1e-6){ax.normalize();if(roll)ax.negate();b.rotateOnWorldAxis(ax,Math.min(roll?60:40,l/dt*(roll?5.9:1.2))*dt)}
      }
    }
  }
  trailStep(b);pv.copy(b.position);
}
function focusCam(){
  if(!tq)return;
  const a=tq.pts[tq.k],b=tq.pts[tq.k+1],dx=b[0]-a[0],dz=b[1]-a[1],d=Math.hypot(dx,dz)||1,ux=dx/d,uz=dz/d;
  const des=new THREE.Vector3(b[0]+ux*10-uz*4,6,b[1]+uz*10+ux*4);
  const tgt=new THREE.Vector3(b[0]*.7+tball.position.x*.3,1.2,b[1]*.7+tball.position.z*.3);
  if(cam.fov!==50){cam.fov=50;cam.updateProjectionMatrix()}
  cam.position.lerp(des,.1);look.lerp(tgt,.15);cam.lookAt(look);
}
function update(n){
  TS=autoOn()?2.2:1;const dt=Math.min(.05,n-(update.l||n));update.l=n;stepRunners(dt);stepThrow(n);focusCam();spinBall(dt);stepBat(dt);
  $('bc').style.display=((mode==='wait'||mode==='aim')&&!bcOn)?'block':'none';
  catcher.visible=G.half===1||mode==='hit'||mode==='replay'||!!tq;
  if(FT&&mode!=='hit')fielders.forEach((f,i)=>{if(FT[i])moveTo(f,FT[i],6*dt)});
  for(let i=HUM.length-1;i>=0;i--){const h=HUM[i];if(!h.parent)HUM.splice(i,1);else animH(h,n)}
  const sp=(n-swingAt)/.3;let ry=-1.2+Math.sin(n*5)*.05,rz=-1.0+Math.sin(n*5+1)*.04;
  if(pitch&&pitch.bunt&&sp>=0&&sp<2){ry=.15;rz=-1.5}else if(sp>=0&&sp<=1){ry=-1.2+2.8*sp;rz=-1.0-.55*sp}else if(sp>1&&sp<2){ry=1.6;rz=-1.55}
  
  if(nextAt&&n>=nextAt){nextAt=0;proceed()}
  if(mode==='wait'){
    if(running.length)waitAt=n;const left=4-(n-waitAt);
    $('pinfo').textContent=running.length?'주자 이동 중…':'투구까지 '+Math.max(0,left).toFixed(1)+'초';
    homeCam();if(left<=.9&&!pw&&G.half===0){pw=true;setAnim(fielders[0],'pitch',n)}if(left<=0)throwPitch(n);
  }else if(mode==='pitch'){
    const p=pitch,t=(n-p.start)/p.dur;
    ball.position.set(p.S.x+(p.A.x-p.S.x)*t+p.mv[0]*t*t,p.S.y+(p.A.y-p.S.y)*t+p.mv[1]*t*t,p.S.z*(1-t));
    homeCam();
    if(p.user)ball.scale.setScalar(1.1);
    if(n>=p.start+p.dur+.02)resolve(n);
  }else if(mode==='hit'){
    const el=n-play.t0,idx=Math.min(Math.floor(el*60),play.pts.length-1),q=play.pts[idx];
    ball.position.set(q[0],q[1],q[2]);
    ball.scale.setScalar(Math.max(.75,cam.position.distanceTo(ball.position)/45));
    shadow.position.set(q[0],.06,q[2]);
    /* 수비수 움직임 */
    fielders.forEach((f,i)=>{
      if(i!==play.chaser){moveTo(f,play.T&&play.T[i],6*dt);return}
      if(play.dec.type==='out'){
        const e=play.pts[play.pts.length-1],k=Math.min(1,el/play.dec.t);
        f.position.set(F[i][0]+(e[0]-F[i][0])*k,0,F[i][1]+(e[2]-F[i][1])*k);
        if(k<1){f.userData.mode='run';f.rotation.y=Math.atan2(-(e[0]-F[i][0]),-(e[2]-F[i][1]))}else if(f.userData.mode==='run')setAnim(f,'catch',now());
      }else{
        const tg0=(q[1]>.6&&play.L)?play.L:q,rr=Math.hypot(tg0[0],tg0[2]),sc=rr>Rf(Math.atan2(tg0[0],-tg0[2])*57.2958)-1.3?(Rf(Math.atan2(tg0[0],-tg0[2])*57.2958)-1.3)/rr:1,tg=[tg0[0]*sc,0,tg0[2]*sc],dx=tg[0]-f.position.x,dz=tg[2]-f.position.z,dd=Math.hypot(dx,dz);
        if(dd>.5){const s=Math.min(dd,6.9*.016*TS);f.position.x+=dx/dd*s;f.position.z+=dz/dd*s;f.userData.mode='run';f.rotation.y=turnTo(f.rotation.y,Math.atan2(-dx,-dz),.22)}else if(f.userData.mode==='run')setAnim(f,play.dec.type==='hr'?'jump':'catch',now());
      }
    });
    if(!tq)cam.position.lerp(new THREE.Vector3(q[0]*.35,Math.max(q[1],0)*.25+9,q[2]+26),.05);
    if(!tq)look.lerp(new THREE.Vector3(q[0],q[1]*.5,q[2]),.12);cam.lookAt(look);
    if(!play.done&&idx>=play.di){play.done=true;announce()}
    if(play.hr&&idx>=play.pts.length-1){if(!play.rp)play.rp=n+.9;else if(n>=play.rp)startReplay(n)}
  }else if(mode==='replay'){
    const el=(n-play.t0)*.7,idx=Math.min(Math.floor(el*60),play.pts.length-1),q=play.pts[idx];
    ball.position.set(q[0],q[1],q[2]);ball.scale.setScalar(Math.max(.75,cam.position.distanceTo(ball.position)/45));
    shadow.position.set(q[0],.06,q[2]);
    cam.position.set(Math.max(-25,Math.min(25,q[0]*.3)),7,-(R+4));
    look.lerp(new THREE.Vector3(q[0],q[1]*.6,q[2]),.15);cam.lookAt(look);
    if(n>=play.rpEnd)endReplay();
  }else if(mode==='fight'){const mx=FG.p.length?(FG.p[0].x+FG.p[1].x)/2:300;cam.fov=44;cam.updateProjectionMatrix();cam.position.lerp(new THREE.Vector3(mx,1.6,10.5),.12);look.lerp(new THREE.Vector3(mx,1.15,0),.15);cam.lookAt(look)}else if(mode==='bc'){cam.fov=50;cam.updateProjectionMatrix();cam.position.lerp(new THREE.Vector3(0,9,-3),.05);look.lerp(new THREE.Vector3(0,1,-17),.08);cam.lookAt(look)}else if(mode==='result'||mode==='aim'){homeCam();if(mode==='aim')$('pinfo').textContent=running.length?'주자 이동 중…':curP(0).name+' · '+curP(0).cnt+'구';
    if(mode==='aim'&&autoPitch&&!autoT&&!running.length){autoT=setTimeout(()=>{autoT=0;if(mode==='aim'&&autoPitch&&!running.length)autoThrow()},400)}}
}
function loop(){requestAnimationFrame(loop);update(now());ren.render(scene,cam)}
toLineup();$('lnGo').onclick=()=>{$('ln').style.display='none';newGame()};$('lnAuto').onclick=()=>{buildTeams();lnSel=-1;renderLn()};
document.querySelectorAll('#dfr button').forEach(b=>b.onclick=()=>setDf(b.dataset.d,true));setDf('normal');document.querySelectorAll('#mdr button').forEach(b=>b.onclick=()=>setMode(b.dataset.m));$('rq').addEventListener('click',pressRq);$('snd').onclick=()=>{sndOn=!sndOn;$('snd').textContent=sndOn?'🔊':'🔇'};$('bf').onclick=flipBat;$('bc').onclick=benchClear;
  $('tgB').onclick=()=>{autoBat=!autoBat;$('tgB').classList.toggle('on',!autoBat);$('tgB').textContent='타자 모드 '+(autoBat?'OFF':'ON');say(autoBat?'타자 모드 끈 · 자동 타격':'타자 모드 켠 · 직접 타격')};
  $('tgP').onclick=()=>{autoPitch=!autoPitch;$('tgP').classList.toggle('on',!autoPitch);$('tgP').textContent='투구 모드 '+(autoPitch?'OFF':'ON');say(autoPitch?'투구 모드 끈 · 자동 투구':'투구 모드 켠 · 직접 투구')};loop();
</script>
</body>
</html>
