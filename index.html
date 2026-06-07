import { useState, useEffect, useRef, useCallback } from "react";

/* ══════════════════════════════════════════════════════
   NEON VAULT CASINO — Cassino Social com Créditos Virtuais
   Sem dinheiro real. Apenas entretenimento.
══════════════════════════════════════════════════════ */

const CSS = `
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;700;900&family=Exo+2:wght@300;400;500;600;700&display=swap');
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#06060f;--bg2:#09091a;--bg3:#0d0d24;
  --p:#9333ea;--pd:#7c3aed;--pg:rgba(147,51,234,.55);--ps:rgba(147,51,234,.14);--pb:#c084fc;
  --c:#06b6d4;--cg:rgba(6,182,212,.5);--cs:rgba(6,182,212,.11);--cb:#67e8f9;
  --g:#f59e0b;--gg:rgba(245,158,11,.5);--gs:rgba(245,158,11,.11);--gb:#fde68a;
  --pk:#ec4899;--pks:rgba(236,72,153,.14);
  --gn:#22c55e;--gns:rgba(34,197,94,.14);
  --r:#ef4444;--rs:rgba(239,68,68,.14);
  --t:#e2e8f0;--t2:#94a3b8;--t3:#475569;
  --gl:rgba(9,9,26,.8);--gbr:rgba(147,51,234,.2)
}
html,body{background:var(--bg);color:var(--t);font-family:'Exo 2',sans-serif;overflow-x:hidden;min-height:100vh}
::-webkit-scrollbar{width:5px}::-webkit-scrollbar-track{background:var(--bg2)}::-webkit-scrollbar-thumb{background:var(--p);border-radius:3px}
.nvp{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden}
.nvpd{position:absolute;border-radius:50%;animation:rise linear infinite}
@keyframes rise{0%{transform:translateY(100vh) scale(0);opacity:0}5%{opacity:.7}90%{opacity:.15}100%{transform:translateY(-80px) scale(1.3);opacity:0}}
.glass{background:var(--gl);backdrop-filter:blur(16px);-webkit-backdrop-filter:blur(16px);border:1px solid var(--gbr);border-radius:16px}
.btn{display:inline-flex;align-items:center;justify-content:center;gap:6px;border:none;border-radius:12px;cursor:pointer;font-family:'Orbitron',sans-serif;font-size:11px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;transition:all .25s;padding:11px 22px;white-space:nowrap;outline:none}
.btn:disabled{opacity:.38;cursor:not-allowed!important;transform:none!important;box-shadow:none!important}
.bp{background:linear-gradient(135deg,var(--p),var(--pd));color:#fff;box-shadow:0 0 22px var(--pg)}
.bp:hover:not(:disabled){transform:translateY(-2px);box-shadow:0 0 38px var(--pg),0 8px 24px rgba(0,0,0,.4)}
.bc{background:linear-gradient(135deg,var(--c),#0891b2);color:#fff;box-shadow:0 0 18px var(--cg)}
.bc:hover:not(:disabled){transform:translateY(-2px);box-shadow:0 0 36px var(--cg)}
.bgld{background:linear-gradient(135deg,var(--g),#d97706);color:#000;font-weight:900;box-shadow:0 0 20px var(--gg)}
.bgld:hover:not(:disabled){transform:translateY(-2px);box-shadow:0 0 40px var(--gg)}
.bout{background:transparent;color:var(--cb);border:1px solid var(--c)}
.bout:hover:not(:disabled){background:var(--cs);box-shadow:0 0 18px var(--cg);transform:translateY(-2px)}
.bgn{background:linear-gradient(135deg,#16a34a,#15803d);color:#fff;box-shadow:0 0 18px rgba(34,197,94,.4)}
.bgn:hover:not(:disabled){transform:translateY(-2px);box-shadow:0 0 30px rgba(34,197,94,.5)}
.brd{background:linear-gradient(135deg,#dc2626,#b91c1c);color:#fff;box-shadow:0 0 16px rgba(239,68,68,.4)}
.brd:hover:not(:disabled){transform:translateY(-2px)}
.bsm{padding:7px 13px;font-size:10px;border-radius:8px}
.blg{padding:15px 36px;font-size:14px;border-radius:14px}
.bxl{padding:18px 44px;font-size:16px;border-radius:16px;letter-spacing:2px}
.nvin{width:100%;background:rgba(9,9,26,.8);border:1px solid rgba(147,51,234,.3);border-radius:10px;color:var(--t);padding:11px 14px;font-family:'Exo 2',sans-serif;font-size:15px;outline:none;transition:border .2s,box-shadow .2s}
.nvin:focus{border-color:var(--p);box-shadow:0 0 0 3px rgba(147,51,234,.17)}
.nvin::placeholder{color:var(--t3)}
.bdg{display:inline-flex;align-items:center;gap:3px;padding:2px 9px;border-radius:20px;font-size:10px;font-weight:700;letter-spacing:.7px;text-transform:uppercase}
.bdgp{background:var(--ps);color:var(--pb);border:1px solid rgba(147,51,234,.33)}
.bdgc{background:var(--cs);color:var(--cb);border:1px solid rgba(6,182,212,.28)}
.bdgg{background:var(--gs);color:var(--gb);border:1px solid rgba(245,158,11,.28)}
.bdggn{background:var(--gns);color:#86efac;border:1px solid rgba(34,197,94,.28)}
.bdgpk{background:var(--pks);color:#fda4af;border:1px solid rgba(236,72,153,.28)}
.bdgr{background:var(--rs);color:#fca5a5;border:1px solid rgba(239,68,68,.28)}
.gcard{position:relative;background:linear-gradient(155deg,rgba(9,9,26,.96),rgba(13,13,34,.9));border:1px solid rgba(147,51,234,.17);border-radius:16px;overflow:hidden;cursor:pointer;transition:all .3s cubic-bezier(.4,0,.2,1);display:flex;flex-direction:column}
.gcard::after{content:'';position:absolute;inset:0;border-radius:16px;background:linear-gradient(155deg,rgba(147,51,234,.1),rgba(6,182,212,.05));opacity:0;transition:opacity .3s}
.gcard:hover{transform:translateY(-8px) scale(1.02);border-color:rgba(147,51,234,.5);box-shadow:0 20px 40px rgba(0,0,0,.5),0 0 30px rgba(147,51,234,.2)}
.gcard:hover::after{opacity:1}
.gcico{height:130px;display:flex;align-items:center;justify-content:center;font-size:54px;background:linear-gradient(155deg,rgba(147,51,234,.08),rgba(6,182,212,.04));position:relative}
.chot{position:absolute;top:9px;right:9px;background:linear-gradient(135deg,#ef4444,#f97316);color:#fff;font-size:9px;font-weight:800;padding:2px 7px;border-radius:20px;z-index:10;animation:flt 2s ease-in-out infinite;letter-spacing:.7px;text-transform:uppercase}
.cnew{position:absolute;top:9px;left:9px;background:linear-gradient(135deg,#06b6d4,#8b5cf6);color:#fff;font-size:9px;font-weight:800;padding:2px 7px;border-radius:20px;z-index:10;animation:flt 2.2s ease-in-out infinite .4s;letter-spacing:.7px;text-transform:uppercase}
@keyframes flt{0%,100%{transform:translateY(0)}50%{transform:translateY(-4px)}}
.nwrap{position:fixed;top:70px;right:16px;z-index:9900;display:flex;flex-direction:column;gap:10px;pointer-events:none}
.notif{min-width:250px;max-width:320px;padding:12px 15px;border-radius:12px;display:flex;align-items:center;gap:10px;pointer-events:auto;animation:nin .4s cubic-bezier(.34,1.56,.64,1);font-weight:600;font-size:13px;box-shadow:0 8px 24px rgba(0,0,0,.4)}
@keyframes nin{from{transform:translateX(115%);opacity:0}to{transform:translateX(0);opacity:1}}
.nout{animation:nout .3s ease forwards!important}
@keyframes nout{to{transform:translateX(115%);opacity:0}}
.nwin{background:linear-gradient(135deg,rgba(21,128,61,.95),rgba(15,118,110,.9));border:1px solid rgba(34,197,94,.4)}
.nlose{background:linear-gradient(135deg,rgba(185,28,28,.95),rgba(159,18,57,.9));border:1px solid rgba(239,68,68,.4)}
.ninfo{background:linear-gradient(135deg,rgba(109,40,217,.95),rgba(79,70,229,.9));border:1px solid rgba(147,51,234,.4)}
.nbonus{background:linear-gradient(135deg,rgba(180,83,9,.95),rgba(154,52,18,.9));border:1px solid rgba(245,158,11,.4)}
.conf{position:fixed;top:-10px;pointer-events:none;z-index:9999;animation:cfl 3.2s ease-in forwards;border-radius:2px}
@keyframes cfl{0%{transform:translateY(0) rotateZ(0) scale(1);opacity:1}100%{transform:translateY(105vh) rotateZ(760deg) scale(.4);opacity:0}}
.mdbg{position:fixed;inset:0;background:rgba(6,6,15,.88);backdrop-filter:blur(6px);-webkit-backdrop-filter:blur(6px);z-index:1000;display:flex;align-items:center;justify-content:center;padding:16px;animation:fdin .2s}
@keyframes fdin{from{opacity:0}to{opacity:1}}
.mdbox{background:linear-gradient(155deg,#0b0b1e,#0f0f28);border:1px solid rgba(147,51,234,.38);border-radius:20px;width:100%;max-width:560px;max-height:92vh;overflow-y:auto;animation:popin .35s cubic-bezier(.34,1.56,.64,1);box-shadow:0 0 60px rgba(147,51,234,.22),0 40px 80px rgba(0,0,0,.6)}
@keyframes popin{from{transform:scale(.85) translateY(30px);opacity:0}to{transform:scale(1) translateY(0);opacity:1}}
.navi{display:flex;align-items:center;gap:6px;padding:7px 12px;border-radius:10px;cursor:pointer;font-size:11px;font-weight:700;letter-spacing:.5px;color:var(--t2);transition:all .2s;white-space:nowrap;border:1px solid transparent;text-transform:uppercase}
.navi:hover{color:var(--pb);background:var(--ps);border-color:rgba(147,51,234,.2)}
.navi.act{color:var(--pb);background:var(--ps);border-color:rgba(147,51,234,.32)}
.cpill{display:flex;align-items:center;gap:7px;padding:7px 16px;border-radius:30px;background:linear-gradient(135deg,rgba(245,158,11,.18),rgba(234,88,12,.12));border:1px solid rgba(245,158,11,.38);box-shadow:0 0 16px rgba(245,158,11,.17);user-select:none}
@keyframes cpop{0%,100%{transform:scale(1)}50%{transform:scale(1.15)}}
.cpop{animation:cpop .3s ease}
.hero{min-height:70vh;display:flex;align-items:center;justify-content:center;position:relative;text-align:center;padding:100px 20px 64px;background:radial-gradient(ellipse 80% 60% at 50% 0%,rgba(147,51,234,.22) 0%,rgba(6,182,212,.07) 46%,transparent 100%)}
.ggrid{display:grid;grid-template-columns:repeat(auto-fill,minmax(185px,1fr));gap:18px}
.ctab{padding:7px 15px;border-radius:20px;cursor:pointer;font-size:11px;font-weight:700;letter-spacing:.5px;transition:all .2s;border:1px solid transparent;color:var(--t2);white-space:nowrap;text-transform:uppercase}
.ctab:hover{color:var(--pb);border-color:rgba(147,51,234,.28);background:rgba(147,51,234,.07)}
.ctab.act{background:var(--ps);border-color:rgba(147,51,234,.45);color:var(--pb);box-shadow:0 0 12px rgba(147,51,234,.17)}
.av{width:42px;height:42px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:20px;flex-shrink:0;border:2px solid rgba(147,51,234,.45);background:linear-gradient(135deg,rgba(147,51,234,.25),rgba(6,182,212,.15));box-shadow:0 0 12px rgba(147,51,234,.23)}
.prog{height:6px;border-radius:3px;background:rgba(255,255,255,.08);overflow:hidden}
.progb{height:100%;border-radius:3px;transition:width .6s ease}
.stitle{display:flex;align-items:center;gap:12px;margin-bottom:20px}
.stitle::after{content:'';flex:1;height:1px;background:linear-gradient(90deg,rgba(147,51,234,.5) 0%,transparent 100%)}
.bjc{width:52px;height:78px;border-radius:7px;background:white;display:flex;flex-direction:column;align-items:flex-start;padding:5px;font-size:15px;font-weight:900;box-shadow:0 4px 12px rgba(0,0,0,.6);flex-shrink:0;border:1px solid rgba(0,0,0,.1);position:relative}
.bjc.red{color:#dc2626}
.bjc.dn{background:linear-gradient(135deg,#1e1b4b,#312e81)}
.bjc.dn::after{content:'?';position:absolute;inset:0;display:flex;align-items:center;justify-content:center;font-size:26px;font-weight:900;color:rgba(255,255,255,.3)}
.mc{aspect-ratio:1;border-radius:9px;cursor:pointer;border:1px solid rgba(147,51,234,.2);display:flex;align-items:center;justify-content:center;font-size:20px;transition:all .2s;background:rgba(9,9,26,.7)}
.mc.ur:hover{background:rgba(147,51,234,.17);border-color:rgba(147,51,234,.5);transform:scale(1.06)}
.mc.gem{background:linear-gradient(135deg,rgba(34,197,94,.28),rgba(16,185,129,.14));border-color:rgba(34,197,94,.5)}
.mc.bomb{background:linear-gradient(135deg,rgba(239,68,68,.38),rgba(185,28,28,.18));border-color:rgba(239,68,68,.6);animation:shk .3s}
@keyframes shk{0%,100%{transform:translateX(0)}25%{transform:translateX(-4px)}75%{transform:translateX(4px)}}
.scrc{aspect-ratio:1;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:26px;cursor:pointer;background:linear-gradient(135deg,#1e1b4b,#312e81);border:1px solid rgba(147,51,234,.4);position:relative;overflow:hidden;transition:transform .2s}
.scrc:hover:not(.done){transform:scale(1.06)}
.scrcov{position:absolute;inset:0;background:linear-gradient(135deg,#4c1d95,#5b21b6);display:flex;align-items:center;justify-content:center;font-size:22px;transition:transform .45s cubic-bezier(.4,0,.2,1),opacity .45s}
.scrc.done .scrcov{transform:scale(0) rotate(45deg);opacity:0}
.rrow{background:rgba(9,9,26,.7);border:1px solid rgba(147,51,234,.17);border-radius:10px;display:flex;align-items:center;gap:14px;padding:12px 16px;margin-bottom:6px;transition:all .2s}
.rrow:hover{background:rgba(147,51,234,.06);border-color:rgba(147,51,234,.28)}
.r1{background:linear-gradient(90deg,rgba(245,158,11,.12),rgba(9,9,26,.5))!important;border-color:rgba(245,158,11,.3)!important}
.r2{background:linear-gradient(90deg,rgba(148,163,184,.08),rgba(9,9,26,.5))!important;border-color:rgba(148,163,184,.2)!important}
.r3{background:linear-gradient(90deg,rgba(180,83,9,.1),rgba(9,9,26,.5))!important;border-color:rgba(205,127,50,.2)!important}
.mcard{padding:15px;border-radius:13px;background:rgba(9,9,26,.7);border:1px solid rgba(147,51,234,.17);display:flex;align-items:center;gap:13px}
.mcard.done{border-color:rgba(34,197,94,.38);background:rgba(34,197,94,.04)}
.mcard.clm{border-color:rgba(245,158,11,.38);animation:mbp 2s infinite}
@keyframes mbp{0%,100%{box-shadow:none}50%{box-shadow:0 0 18px rgba(245,158,11,.28)}}
.bnav{position:fixed;bottom:0;left:0;right:0;background:rgba(9,9,26,.96);backdrop-filter:blur(16px);border-top:1px solid rgba(147,51,234,.17);display:none;padding:8px 0 max(8px,env(safe-area-inset-bottom));z-index:100}
.bni{flex:1;display:flex;flex-direction:column;align-items:center;gap:3px;cursor:pointer;padding:4px;color:var(--t3);font-size:9px;font-weight:700;letter-spacing:.4px;text-transform:uppercase;transition:color .2s}
.bni.act,.bni:hover{color:var(--pb)}
.ticker{overflow:hidden;white-space:nowrap}
.tick-i{display:inline-flex;animation:tck 22s linear infinite;gap:50px}
@keyframes tck{from{transform:translateX(0)}to{transform:translateX(-50%)}}
.pge{animation:pgin .3s ease}
@keyframes pgin{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:translateY(0)}}
.regbg{position:fixed;inset:0;background:rgba(6,6,15,.95);backdrop-filter:blur(8px);z-index:2000;display:flex;align-items:center;justify-content:center;padding:20px}
@keyframes spin360{to{transform:rotate(360deg)}}
.spina{animation:spin360 .8s linear infinite;display:inline-block}
@media(max-width:768px){
  .ggrid{grid-template-columns:repeat(auto-fill,minmax(145px,1fr));gap:12px}
  .gcico{height:105px;font-size:44px}
  .desknav{display:none!important}
  .bnav{display:flex}
  .mainpad{padding-bottom:80px!important}
  .hero{min-height:55vh;padding:80px 16px 40px}
}
`;

/* ══════════ CONSTANTS ══════════ */
const GAMES = [
  {id:'slots',    name:'Slots Clássicos',  cat:'slots', e:'🎰',hot:true,       d:'Gire os rolos e alinhe os símbolos'},
  {id:'slots2',   name:'Slots Bônus',      cat:'slots', e:'🌟',nx:true,        d:'Slots com rodadas de bônus grátis'},
  {id:'roulette', name:'Roleta Europeia',  cat:'table', e:'🎡',hot:true,       d:'Roleta clássica de cassino europeu'},
  {id:'roulette2',name:'Roleta Americana', cat:'table', e:'🎯',               d:'Roleta com zero e duplo zero'},
  {id:'blackjack',name:'Blackjack',        cat:'table', e:'🃏',hot:true,       d:'Chegue ao 21 sem ultrapassar'},
  {id:'baccarat', name:'Baccarat',         cat:'table', e:'💎',               d:'Aposte no banker ou player'},
  {id:'poker',    name:'Texas Hold\'em',   cat:'table', e:'♠️',               d:'O poker mais popular do mundo'},
  {id:'vpoker',   name:'Video Poker',      cat:'table', e:'🎴',               d:'Poker contra a máquina virtual'},
  {id:'crash',    name:'Crash',            cat:'mini',  e:'🚀',hot:true,nx:true,d:'Saia antes que o foguete exploda!'},
  {id:'mines',    name:'Mines',            cat:'mini',  e:'💣',hot:true,       d:'Encontre gemas, evite as minas'},
  {id:'plinko',   name:'Plinko',           cat:'mini',  e:'⚡',nx:true,        d:'Deixe a bola cair pelos pinos'},
  {id:'wheel',    name:'Roda da Sorte',    cat:'mini',  e:'🎪',               d:'Gire a roda e descubra seu prêmio'},
  {id:'dice',     name:'Dados',            cat:'mini',  e:'🎲',               d:'Aposte no resultado dos dados'},
  {id:'coinflip', name:'Cara ou Coroa',    cat:'mini',  e:'🪙',               d:'Simples, rápido e emocionante'},
  {id:'highlow',  name:'High Low',         cat:'mini',  e:'📊',               d:'Mais alto ou mais baixo?'},
  {id:'scratch',  name:'Raspadinha',       cat:'mini',  e:'🎟️',nx:true,       d:'Raspe e descubra seu prêmio virtual'},
  {id:'craps',    name:'Craps',            cat:'table', e:'🎳',               d:'O jogo de dados americano clássico'},
  {id:'bingo',    name:'Bingo',            cat:'other', e:'📢',               d:'Complete seu cartão de bingo virtual'},
  {id:'keno',     name:'Keno',             cat:'other', e:'🔢',               d:'Escolha seus números da sorte'},
  {id:'sicbo',    name:'Sic Bo',           cat:'table', e:'🀄',nx:true,        d:'Jogo de dados asiático clássico'},
];

const AVS = ['🦊','🐺','🦁','🐯','🦅','🦋','🔥','⭐','💎','🌙','👑','🎭','🃏','🎮','🏆','🚀'];
const CONF_C = ['#f59e0b','#9333ea','#06b6d4','#ec4899','#22c55e','#fde68a','#c084fc'];
const SLOT_S = ['🍒','🍋','🍊','🔔','💎','⭐','7️⃣'];
const SLOT_P = {'🍒':2,'🍋':3,'🍊':4,'🔔':5,'💎':10,'⭐':15,'7️⃣':20};
const SUITS = ['♠','♥','♦','♣'];
const RANKS = ['A','2','3','4','5','6','7','8','9','10','J','Q','K'];
const RED_N = new Set([1,3,5,7,9,12,14,16,18,19,21,23,25,27,30,32,34,36]);
const WHEEL_S = [
  {l:'0.5×',m:.5,c:'#ef4444'},{l:'1.5×',m:1.5,c:'#f59e0b'},{l:'2×',m:2,c:'#22c55e'},
  {l:'BOOM',m:0,c:'#4b5563'},{l:'3×',m:3,c:'#9333ea'},{l:'1×',m:1,c:'#06b6d4'},
  {l:'5×',m:5,c:'#f59e0b'},{l:'0.5×',m:.5,c:'#ef4444'},{l:'2×',m:2,c:'#22c55e'},
  {l:'BOOM',m:0,c:'#4b5563'},{l:'1×',m:1,c:'#06b6d4'},{l:'4×',m:4,c:'#ec4899'},
];
const RANK_DATA = [
  {n:'NeonKing777',av:'👑',cr:125800,w:342},{n:'StarPlayer99',av:'⭐',cr:98450,w:287},
  {n:'DiamondFox',av:'🦊',cr:87200,w:251},{n:'LuckyTiger',av:'🐯',cr:76500,w:218},
  {n:'CrashMaster',av:'🚀',cr:65800,w:196},{n:'SlotHunter',av:'🎰',cr:54200,w:174},
  {n:'GemSeeker',av:'💎',cr:43700,w:152},{n:'WheelWizard',av:'🎪',cr:38900,w:143},
  {n:'AceOfClubs',av:'♠️',cr:32400,w:128},{n:'NightOwl22',av:'🌙',cr:28700,w:115},
];
const MISSIONS0 = [
  {id:'m1',n:'Iniciante',d:'Jogue 5 rodadas de Slots',e:'🎰',g:5,p:0,r:50,t:'slots'},
  {id:'m2',n:'Apostador',d:'Jogue 3 partidas de Blackjack',e:'🃏',g:3,p:0,r:75,t:'blackjack'},
  {id:'m3',n:'Rodador',d:'Aposte na Roleta 5 vezes',e:'🎡',g:5,p:0,r:60,t:'roulette'},
  {id:'m4',n:'Explorador',d:'Jogue 5 jogos diferentes',e:'🌟',g:5,p:0,r:100,t:'explore'},
  {id:'m5',n:'Sobrevivente',d:'Revele 10 gemas em Mines',e:'💎',g:10,p:0,r:80,t:'mines'},
  {id:'m6',n:'Piloto',d:'Cash out em Crash 3 vezes',e:'🚀',g:3,p:0,r:90,t:'crash'},
];
const ACHIEVE0 = [
  {id:'a1',n:'Primeiro Giro',e:'🎰',d:'Girou os slots pela primeira vez'},
  {id:'a2',n:'Sortudo',e:'🍀',d:'Ganhou 5 apostas seguidas'},
  {id:'a3',n:'Milionário Virtual',e:'💰',d:'Acumulou 1.000+ créditos virtuais'},
  {id:'a4',n:'Explorador',e:'🗺️',d:'Jogou 8 tipos de jogos diferentes'},
  {id:'a5',n:'Crash Master',e:'🚀',d:'Cash out com multiplicador 5× ou mais'},
  {id:'a6',n:'Sobrevivente',e:'💣',d:'Revelou 15 gemas em uma rodada de Mines'},
];

/* ══════════ HELPERS ══════════ */
const rnd = (a,b) => Math.floor(Math.random()*(b-a+1))+a;
const fmt = n => Math.floor(n).toLocaleString('pt-BR');
const mkCard = () => ({ r:RANKS[rnd(0,12)], s:SUITS[rnd(0,3)] });
const cVal = r => r==='A'?11:['J','Q','K'].includes(r)?10:+r;
const hVal = cs => { let v=cs.reduce((a,c)=>a+cVal(c.r),0),a=cs.filter(c=>c.r==='A').length; while(v>21&&a>0){v-=10;a--;} return v; };
const isRed = s => s==='♥'||s==='♦';

function blastConfetti() {
  for(let i=0;i<65;i++){
    const el=document.createElement('div');
    el.className='conf';
    el.style.cssText=`left:${rnd(5,95)}vw;width:${rnd(6,13)}px;height:${rnd(6,13)}px;background:${CONF_C[rnd(0,6)]};animation-duration:${(2+Math.random()*1.6).toFixed(2)}s;animation-delay:${(i*0.04).toFixed(2)}s`;
    document.body.appendChild(el);
    setTimeout(()=>el.remove(),5500);
  }
}

/* ══════════ PARTICLES ══════════ */
function Particles() {
  const dots = useRef([]);
  if(!dots.current.length) {
    dots.current = Array.from({length:28},(_,i)=>({
      id:i, size:rnd(2,5),
      left:rnd(2,98),
      dur:rnd(8,22),
      delay:rnd(0,15),
      col:i%3===0?'rgba(147,51,234,':'':i%3===1?'rgba(6,182,212,':'rgba(245,158,11,',
      op:(0.3+Math.random()*0.4).toFixed(2)
    }));
  }
  return (
    <div className="nvp">
      {dots.current.map(d=>(
        <div key={d.id} className="nvpd" style={{
          width:d.size+'px',height:d.size+'px',
          left:d.left+'%',
          background:d.col+d.op+')',
          animationDuration:d.dur+'s',
          animationDelay:-d.delay+'s',
        }}/>
      ))}
    </div>
  );
}

/* ══════════ NOTIFICATIONS ══════════ */
function Notifs({ns}) {
  const ico = {win:'✅',lose:'❌',info:'ℹ️',bonus:'🎁'};
  return (
    <div className="nwrap">
      {ns.map(n=>(
        <div key={n.id} className={`notif n${n.t} ${n.out?'nout':''}`}>
          <span style={{fontSize:18}}>{ico[n.t]||'•'}</span>
          <span>{n.msg}</span>
        </div>
      ))}
    </div>
  );
}

/* ══════════ GAME CARD ══════════ */
function GCard({g, onPlay, fav, onFav}) {
  const catMap = {slots:'bdgp',table:'bdgc',mini:'bdgg',other:'bdgpk'};
  const catName = {slots:'Slots',table:'Mesa',mini:'Mini',other:'Outro'};
  return (
    <div className="gcard" onClick={()=>onPlay(g.id)}>
      <div className="gcico">
        {g.hot&&<div className="chot">🔥 HOT</div>}
        {g.nx&&<div className="cnew">✨ NOVO</div>}
        {g.e}
      </div>
      <div style={{padding:'13px 15px 15px',flex:1,display:'flex',flexDirection:'column'}}>
        <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:6}}>
          <div style={{fontFamily:'Orbitron',fontWeight:700,fontSize:12,color:'var(--t)',lineHeight:1.3}}>{g.name}</div>
          <button onClick={e=>{e.stopPropagation();onFav(g.id);}} style={{background:'none',border:'none',cursor:'pointer',fontSize:14,padding:'2px',color:fav?'var(--g)':'var(--t3)',flexShrink:0}}>{fav?'⭐':'☆'}</button>
        </div>
        <div style={{fontSize:11,color:'var(--t2)',marginTop:4,flex:1,lineHeight:1.4}}>{g.d}</div>
        <div style={{marginTop:10,display:'flex',alignItems:'center',justifyContent:'space-between'}}>
          <span className={`bdg ${catMap[g.cat]}`}>{catName[g.cat]}</span>
          <span style={{fontSize:10,color:'var(--t3)'}}>créditos virtuais</span>
        </div>
      </div>
    </div>
  );
}

/* ══════════ MODAL ══════════ */
function GMod({onClose, maxW, children}) {
  useEffect(()=>{
    const h=e=>{if(e.key==='Escape')onClose();};
    window.addEventListener('keydown',h);
    return ()=>window.removeEventListener('keydown',h);
  },[onClose]);
  return (
    <div className="mdbg" onClick={e=>{if(e.target===e.currentTarget)onClose();}}>
      <div className="mdbox" style={maxW?{maxWidth:maxW}:{}}>{children}</div>
    </div>
  );
}

function GHdr({title, emoji, onClose, sub}) {
  return (
    <div style={{padding:'20px 22px 0',display:'flex',alignItems:'center',justifyContent:'space-between',gap:12}}>
      <div>
        <div style={{fontFamily:'Orbitron',fontSize:19,fontWeight:900,color:'var(--g)'}}>{emoji} {title}</div>
        <div style={{fontSize:11,color:'var(--t3)',marginTop:2}}>{sub||'Créditos virtuais — sem valor monetário'}</div>
      </div>
      <button onClick={onClose} style={{background:'none',border:'none',color:'var(--t2)',cursor:'pointer',fontSize:22,flexShrink:0}}>✕</button>
    </div>
  );
}

function BetRow({bet,setBet,credits,bets}) {
  return (
    <div style={{display:'flex',gap:6,flexWrap:'wrap',marginBottom:12,alignItems:'center'}}>
      <span style={{fontSize:11,color:'var(--t2)',fontWeight:600,marginRight:2}}>APOSTA:</span>
      {(bets||[5,10,25,50,100]).map(b=>(
        <button key={b} onClick={()=>setBet(b)} disabled={b>credits}
          style={{padding:'6px 11px',borderRadius:8,border:`1px solid ${bet===b?'rgba(147,51,234,.7)':'rgba(147,51,234,.22)'}`,background:bet===b?'rgba(147,51,234,.22)':'rgba(9,9,26,.7)',color:bet===b?'var(--pb)':'var(--t2)',cursor:b>credits?'not-allowed':'pointer',fontSize:12,fontWeight:700,opacity:b>credits?.35:1,transition:'all .2s'}}>
          {b}
        </button>
      ))}
    </div>
  );
}

function MsgBox({ok, msg}) {
  if(!msg) return null;
  return (
    <div style={{padding:'10px 14px',borderRadius:9,marginBottom:12,textAlign:'center',fontWeight:700,fontSize:13,background:ok?'rgba(34,197,94,.14)':'rgba(239,68,68,.12)',border:`1px solid ${ok?'rgba(34,197,94,.4)':'rgba(239,68,68,.35)'}`,color:ok?'#86efac':'#fca5a5'}}>
      {msg}
    </div>
  );
}

/* ══════════ SLOTS GAME ══════════ */
function SlotsGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [rows,setRows]=useState([[SLOT_S[0],SLOT_S[1],SLOT_S[2]],[SLOT_S[3],SLOT_S[4],SLOT_S[5]],[SLOT_S[6],SLOT_S[0],SLOT_S[1]]]);
  const [spin,setSpin]=useState(false);
  const [msg,setMsg]=useState(null);
  const [spins,setSpins]=useState(0);
  const [totalW,setTotalW]=useState(0);

  const doSpin = () => {
    if(spin||bet>credits) return;
    setSpin(true); setMsg(null); onLose(bet); track('slots');
    const nr = [[rnd(0,6),rnd(0,6),rnd(0,6)],[rnd(0,6),rnd(0,6),rnd(0,6)],[rnd(0,6),rnd(0,6),rnd(0,6)]].map(r=>r.map(i=>SLOT_S[i]));
    if(Math.random()<.27){const s=SLOT_S[rnd(0,6)];nr[0][1]=s;nr[1][1]=s;nr[2][1]=s;}
    else if(Math.random()<.3){const s=SLOT_S[rnd(0,4)];const ri=rnd(0,2);nr[ri][1]=s;nr[(ri+1)%3][1]=s;}
    setTimeout(()=>{
      setRows(nr); setSpin(false); setSpins(x=>x+1);
      const mid=[nr[0][1],nr[1][1],nr[2][1]];
      if(mid[0]===mid[1]&&mid[1]===mid[2]){
        const m=SLOT_P[mid[0]], w=bet*m;
        onWin(w); setTotalW(t=>t+w); addN('win',`🎰 JACKPOT! +${fmt(w)} créditos!`);
        setMsg({ok:true,txt:`3× ${mid[0]} — JACKPOT! +${fmt(w)} créditos!`});
        if(m>=10) blastConfetti();
      } else if(mid[0]===mid[1]||mid[1]===mid[2]||mid[0]===mid[2]){
        const w=Math.floor(bet*1.5); onWin(w); setTotalW(t=>t+w);
        addN('win',`Par! +${fmt(w)} créditos`); setMsg({ok:true,txt:`Par! +${fmt(w)} créditos`});
      } else { setMsg({ok:false,txt:'Sem combinação — tente novamente!'}); }
    },900);
  };

  return (
    <div>
      <GHdr title="Slots Clássicos" emoji="🎰" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{background:'rgba(0,0,0,.45)',borderRadius:14,padding:'18px 14px',border:'1px solid rgba(147,51,234,.25)',position:'relative',marginBottom:14}}>
          <div style={{position:'absolute',top:'50%',left:0,right:0,height:84,transform:'translateY(-50%)',background:'rgba(147,51,234,.07)',borderTop:'1px solid rgba(147,51,234,.32)',borderBottom:'1px solid rgba(147,51,234,.32)',pointerEvents:'none'}}/>
          <div style={{display:'flex',gap:8,justifyContent:'center'}}>
            {[0,1,2].map(ci=>(
              <div key={ci} style={{width:90,height:252,overflow:'hidden',borderRadius:10,background:'rgba(0,0,0,.3)',border:'1px solid rgba(147,51,234,.17)',display:'flex',flexDirection:'column'}}>
                {rows[ci].map((sym,si)=>(
                  <div key={si} style={{height:84,display:'flex',alignItems:'center',justifyContent:'center',fontSize:46,filter:spin?'blur(5px)':'none',transition:spin?'none':'filter .3s'}}>{sym}</div>
                ))}
              </div>
            ))}
          </div>
        </div>
        <MsgBox ok={msg?.ok} msg={msg?.txt}/>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={doSpin} disabled={spin||bet>credits}>
          {spin?<><span className="spina">⏳</span> Girando...</>:'🎰 GIRAR'}
        </button>
        <div style={{display:'flex',justifyContent:'space-between',marginTop:10,fontSize:11,color:'var(--t3)'}}>
          <span>Rodadas: {spins}</span><span style={{color:'var(--pb)'}}>Ganhos: +{fmt(totalW)}</span>
        </div>
      </div>
    </div>
  );
}

/* ══════════ BLACKJACK ══════════ */
function BJGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [phase,setPhase]=useState('bet');
  const [player,setPlayer]=useState([]);
  const [dealer,setDealer]=useState([]);
  const [dRev,setDRev]=useState(false);
  const [res,setRes]=useState(null);

  const showRes = useCallback((p,d,natural) => {
    setDRev(true);
    const pv=hVal(p), dv=hVal(d);
    let result;
    if(natural){const w=Math.floor(bet*2.5);onWin(w);addN('win',`Blackjack! +${fmt(w)}`);result={t:'win',msg:`🎉 BLACKJACK! +${fmt(w)} créditos!`};}
    else if(pv>21){result={t:'lose',msg:`💥 Passou de 21! Você perdeu ${fmt(bet)} créditos.`};}
    else if(dv>21||pv>dv){const w=bet*2;onWin(w);addN('win',`+${fmt(w)}`);result={t:'win',msg:`✅ Você ganhou! +${fmt(w)} créditos!`};}
    else if(pv===dv){onWin(bet);result={t:'push',msg:`🤝 Empate! Créditos devolvidos.`};}
    else{result={t:'lose',msg:`❌ Dealer ganhou com ${dv}. Você perdeu.`};}
    setRes(result); setPhase('result');
  },[bet,onWin,addN]);

  const deal=()=>{
    if(bet>credits) return;
    onLose(bet); track('blackjack');
    const p=[mkCard(),mkCard()], d=[mkCard(),mkCard()];
    setPlayer(p); setDealer(d); setDRev(false); setRes(null);
    if(hVal(p)===21){setTimeout(()=>showRes(p,d,true),300);}
    else setPhase('play');
  };

  const hit=()=>{
    const np=[...player,mkCard()]; setPlayer(np);
    if(hVal(np)>=21) showRes(np,dealer,false);
  };
  const stand=()=>{ let d=[...dealer]; while(hVal(d)<17)d.push(mkCard()); showRes(player,d,false); };
  const dbl=()=>{
    if(bet>credits) return;
    onLose(bet);
    const np=[...player,mkCard()]; setPlayer(np);
    let d=[...dealer]; while(hVal(d)<17)d.push(mkCard());
    showRes(np,d,false);
  };
  const reset=()=>{setPhase('bet');setPlayer([]);setDealer([]);setRes(null);};

  const CardV=({c,down})=>(
    <div className={`bjc ${down?'dn':isRed(c?.s)?'red':''}`}>
      {!down&&c&&<><div>{c.r}{c.s}</div><div style={{position:'absolute',bottom:4,right:4,transform:'rotate(180deg)',fontSize:12}}>{c.r}{c.s}</div></>}
    </div>
  );

  return (
    <div>
      <GHdr title="Blackjack" emoji="🃏" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{marginBottom:14}}>
          <div style={{fontSize:11,color:'var(--t2)',fontWeight:700,marginBottom:7,fontFamily:'Orbitron'}}>DEALER {dRev?`— ${hVal(dealer)} pts`:'— ?'}</div>
          <div style={{display:'flex',gap:6,flexWrap:'wrap',minHeight:80}}>
            {dealer.map((c,i)=><CardV key={i} c={c} down={!dRev&&i===1}/>)}
          </div>
        </div>
        <div style={{height:1,background:'rgba(255,255,255,.07)',margin:'10px 0'}}/>
        <div style={{marginBottom:14}}>
          <div style={{fontSize:11,color:'var(--t2)',fontWeight:700,marginBottom:7,fontFamily:'Orbitron'}}>VOCÊ — {player.length>0?hVal(player)+' pts':'...'}</div>
          <div style={{display:'flex',gap:6,flexWrap:'wrap',minHeight:80}}>
            {player.map((c,i)=><CardV key={i} c={c}/>)}
            {player.length===0&&<div style={{color:'var(--t3)',fontSize:12,paddingTop:8}}>Aperte "Distribuir" para começar</div>}
          </div>
        </div>
        {res&&(
          <div style={{padding:'11px 14px',borderRadius:9,textAlign:'center',fontWeight:700,fontSize:13,marginBottom:12,background:res.t==='win'?'rgba(34,197,94,.14)':res.t==='push'?'rgba(6,182,212,.11)':'rgba(239,68,68,.12)',border:`1px solid ${res.t==='win'?'rgba(34,197,94,.4)':res.t==='push'?'rgba(6,182,212,.3)':'rgba(239,68,68,.35)'}`,color:res.t==='win'?'#86efac':res.t==='push'?'var(--cb)':'#fca5a5'}}>
            {res.msg}
          </div>
        )}
        {phase==='bet'&&(<>
          <BetRow bet={bet} setBet={setBet} credits={credits}/>
          <button className="btn bgld blg" style={{width:'100%'}} onClick={deal} disabled={bet>credits}>🃏 DISTRIBUIR ({fmt(bet)} créditos)</button>
        </>)}
        {phase==='play'&&(
          <div style={{display:'flex',gap:8}}>
            <button className="btn bgn" style={{flex:1}} onClick={hit}>✅ HIT</button>
            <button className="btn brd" style={{flex:1}} onClick={stand}>🚫 STAND</button>
            <button className="btn bc" style={{flex:1}} onClick={dbl} disabled={bet>credits} title="Dobra aposta, 1 carta">⚡ DBL</button>
          </div>
        )}
        {phase==='result'&&<button className="btn bp blg" style={{width:'100%',marginTop:4}} onClick={reset}>🔄 Nova Mão</button>}
      </div>
    </div>
  );
}

/* ══════════ ROULETTE ══════════ */
function RouletteGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [btype,setBtype]=useState(null);
  const [spin,setSpin]=useState(false);
  const [res,setRes]=useState(null);
  const [num,setNum]=useState(null);

  const BETS = [
    {id:'red',   lb:'🔴 Vermelho',m:2, chk:n=>n>0&&RED_N.has(n)},
    {id:'black', lb:'⚫ Preto',   m:2, chk:n=>n>0&&!RED_N.has(n)},
    {id:'odd',   lb:'Ímpar',     m:2, chk:n=>n>0&&n%2!==0},
    {id:'even',  lb:'Par',       m:2, chk:n=>n>0&&n%2===0},
    {id:'low',   lb:'1–18',      m:2, chk:n=>n>=1&&n<=18},
    {id:'high',  lb:'19–36',     m:2, chk:n=>n>=19&&n<=36},
    {id:'d1',    lb:'1ª Dúzia',  m:3, chk:n=>n>=1&&n<=12},
    {id:'d2',    lb:'2ª Dúzia',  m:3, chk:n=>n>=13&&n<=24},
    {id:'d3',    lb:'3ª Dúzia',  m:3, chk:n=>n>=25&&n<=36},
    {id:'zero',  lb:'0 Verde',   m:35,chk:n=>n===0},
  ];

  const doSpin = () => {
    if(!btype||spin||bet>credits) return;
    setSpin(true); setRes(null); onLose(bet); track('roulette');
    const n=rnd(0,36);
    setTimeout(()=>{
      setNum(n); setSpin(false);
      const bt=BETS.find(b=>b.id===btype);
      if(bt&&bt.chk(n)){const w=bet*bt.m;onWin(w);addN('win',`Roleta: ${n} — +${fmt(w)} créditos!`);setRes({ok:true,msg:`✅ Número ${n}! +${fmt(w)} créditos!`,n});if(bt.m>=10)blastConfetti();}
      else{addN('lose',`Roleta: ${n} — sem sorte`);setRes({ok:false,msg:`❌ Número ${n} — Sem sorte desta vez!`,n});}
    },1600);
  };

  const btnStyle = (id) => {
    const sel = btype===id;
    if(id==='red') return {background:sel?'rgba(239,68,68,.4)':'rgba(239,68,68,.1)',borderColor:sel?'rgba(239,68,68,.8)':'rgba(239,68,68,.35)',color:'#fca5a5'};
    if(id==='black') return {background:sel?'rgba(100,116,139,.4)':'rgba(100,116,139,.1)',borderColor:sel?'rgba(148,163,184,.7)':'rgba(100,116,139,.35)',color:'#e2e8f0'};
    if(id==='zero') return {background:sel?'rgba(34,197,94,.35)':'rgba(34,197,94,.1)',borderColor:sel?'rgba(34,197,94,.7)':'rgba(34,197,94,.35)',color:'#86efac'};
    return {background:sel?'rgba(147,51,234,.3)':'var(--ps)',borderColor:sel?'rgba(147,51,234,.8)':'rgba(147,51,234,.4)',color:'var(--pb)'};
  };

  const numColor = n===null?'rgba(9,9,26,.5)':n===0?'rgba(34,197,94,.3)':RED_N.has(n)?'rgba(239,68,68,.3)':'rgba(30,41,59,.6)';

  return (
    <div>
      <GHdr title="Roleta Europeia" emoji="🎡" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{display:'flex',justifyContent:'center',marginBottom:16}}>
          <div style={{width:96,height:96,borderRadius:'50%',border:'3px solid rgba(147,51,234,.5)',display:'flex',alignItems:'center',justifyContent:'center',background:numColor,boxShadow:num!=null?`0 0 30px ${num===0?'rgba(34,197,94,.5)':RED_N.has(num)?'rgba(239,68,68,.5)':'rgba(30,41,59,.5)'}`:undefined,transition:'all .5s'}}>
            {spin?<div style={{fontSize:42,animation:'spin360 .5s linear infinite'}}>🎡</div>:num!=null?<div style={{fontFamily:'Orbitron',fontSize:34,fontWeight:900,color:'#fff'}}>{num}</div>:<div style={{fontSize:38,color:'var(--t3)'}}>?</div>}
          </div>
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <div style={{fontFamily:'Orbitron',fontSize:11,color:'var(--t2)',marginBottom:8,fontWeight:700}}>TIPO DE APOSTA</div>
        <div style={{display:'flex',gap:7,flexWrap:'wrap',marginBottom:14}}>
          {BETS.map(b=>(
            <button key={b.id} onClick={()=>setBtype(b.id)}
              style={{padding:'8px 11px',borderRadius:8,border:'1px solid',fontSize:11,fontWeight:700,cursor:'pointer',transition:'all .2s',transform:btype===b.id?'scale(1.06)':'scale(1)',...btnStyle(b.id)}}>
              {b.lb}{b.m>2?` ×${b.m}`:''}
            </button>
          ))}
        </div>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={doSpin} disabled={!btype||spin||bet>credits}>
          {spin?<><span className="spina">🎡</span> Girando...</>:'🎡 GIRAR'}
        </button>
        {!btype&&<div style={{textAlign:'center',fontSize:11,color:'var(--t3)',marginTop:8}}>Selecione um tipo de aposta acima ↑</div>}
      </div>
    </div>
  );
}

/* ══════════ CRASH GAME ══════════ */
function CrashGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [phase,setPhase]=useState('idle');
  const [mult,setMult]=useState(1.00);
  const canvasRef=useRef(null);
  const rafRef=useRef(null);
  const startRef=useRef(0);
  const crashAtRef=useRef(1);
  const multRef=useRef(1);

  const drawGraph=(m,crashed)=>{
    const c=canvasRef.current; if(!c) return;
    const ctx=c.getContext('2d'), W=c.width, H=c.height;
    ctx.clearRect(0,0,W,H);
    const steps=80;
    const pts=Array.from({length:steps+1},(_,i)=>{
      const t=i/steps, x=t*W*0.88+W*0.06;
      const v=1+Math.pow(t*2.2,1.7)*(m-1);
      return {x,y:Math.max(H*0.06,H-((v-1)/(Math.max(m,2.5)-1+0.01))*H*0.82-H*0.06)};
    });
    const grad=ctx.createLinearGradient(0,0,W,0);
    grad.addColorStop(0,crashed?'rgba(239,68,68,.9)':'rgba(34,197,94,.9)');
    grad.addColorStop(1,crashed?'rgba(185,28,28,.7)':'rgba(16,185,129,.7)');
    ctx.beginPath(); ctx.strokeStyle=grad; ctx.lineWidth=3; ctx.lineCap='round';
    pts.forEach((p,i)=>i===0?ctx.moveTo(p.x,p.y):ctx.lineTo(p.x,p.y)); ctx.stroke();
    ctx.beginPath();
    pts.forEach((p,i)=>i===0?ctx.moveTo(p.x,p.y):ctx.lineTo(p.x,p.y));
    ctx.lineTo(pts[pts.length-1].x,H); ctx.lineTo(pts[0].x,H); ctx.closePath();
    ctx.fillStyle=crashed?'rgba(239,68,68,.07)':'rgba(34,197,94,.07)'; ctx.fill();
    if(crashed){
      ctx.font='bold 14px Orbitron,sans-serif'; ctx.fillStyle='rgba(239,68,68,.8)'; ctx.textAlign='center';
      ctx.fillText('💥 CRASHED!',W/2,H*0.55);
    }
  };

  const startGame=()=>{
    if(bet>credits) return;
    onLose(bet); track('crash');
    const crash=Math.random()<.12?1+(Math.random()*.5):1+(Math.random()*Math.random()*9.5);
    crashAtRef.current=parseFloat(crash.toFixed(2));
    setPhase('running'); startRef.current=performance.now(); setMult(1.00); multRef.current=1.00;
    const anim=(now)=>{
      const el=(now-startRef.current)/1000;
      const m=parseFloat((1+Math.pow(el*.75,1.7)).toFixed(2));
      multRef.current=m; setMult(m); drawGraph(m,false);
      if(m>=crashAtRef.current){setMult(parseFloat(crash.toFixed(2)));setPhase('crashed');drawGraph(parseFloat(crash.toFixed(2)),true);addN('lose',`💥 Crash em ${crash.toFixed(2)}×!`);return;}
      rafRef.current=requestAnimationFrame(anim);
    };
    rafRef.current=requestAnimationFrame(anim);
  };

  const cashout=()=>{
    if(phase!=='running') return;
    cancelAnimationFrame(rafRef.current);
    const m=multRef.current, w=Math.floor(bet*m);
    onWin(w); setPhase('won'); addN('win',`🚀 Saiu em ${m.toFixed(2)}×! +${fmt(w)} créditos!`);
    track('crash'); drawGraph(m,false);
    if(m>=5) blastConfetti();
  };

  useEffect(()=>()=>cancelAnimationFrame(rafRef.current),[]);
  useEffect(()=>{if(canvasRef.current) drawGraph(1,false);},[]);

  return (
    <div>
      <GHdr title="Crash" emoji="🚀" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <canvas ref={canvasRef} width={500} height={175} style={{width:'100%',height:175,background:'rgba(0,0,0,.4)',borderRadius:12,border:'1px solid rgba(147,51,234,.22)',display:'block',marginBottom:14}}/>
        {phase==='running'&&(
          <div style={{textAlign:'center',marginBottom:12}}>
            <div style={{fontFamily:'Orbitron',fontSize:40,fontWeight:900,color:'#22c55e',textShadow:'0 0 20px rgba(34,197,94,.6)',letterSpacing:2}}>{mult.toFixed(2)}×</div>
            <button className="btn bgld bxl" style={{marginTop:12,width:'100%',fontSize:17}} onClick={cashout}>
              💰 CASH OUT — {fmt(Math.floor(bet*mult))} créditos!
            </button>
          </div>
        )}
        {phase==='crashed'&&(
          <div style={{padding:'12px',borderRadius:10,background:'rgba(239,68,68,.14)',border:'1px solid rgba(239,68,68,.4)',textAlign:'center',marginBottom:12}}>
            <div style={{fontFamily:'Orbitron',fontSize:22,fontWeight:900,color:'#fca5a5'}}>💥 CRASH em {crashAtRef.current}×</div>
            <div style={{color:'var(--t2)',fontSize:12,marginTop:3}}>Você perdeu {fmt(bet)} créditos virtuais</div>
          </div>
        )}
        {phase==='won'&&(
          <div style={{padding:'12px',borderRadius:10,background:'rgba(34,197,94,.14)',border:'1px solid rgba(34,197,94,.4)',textAlign:'center',marginBottom:12}}>
            <div style={{fontFamily:'Orbitron',fontSize:22,fontWeight:900,color:'#86efac'}}>✅ Cash Out em {mult.toFixed(2)}×!</div>
            <div style={{color:'var(--t2)',fontSize:12,marginTop:3}}>+{fmt(Math.floor(bet*mult))} créditos virtuais!</div>
          </div>
        )}
        {(phase==='idle'||phase==='crashed'||phase==='won')&&(<>
          <BetRow bet={bet} setBet={setBet} credits={credits}/>
          <button className="btn bgld blg" style={{width:'100%'}} onClick={startGame} disabled={bet>credits}>🚀 INICIAR JOGO</button>
        </>)}
      </div>
    </div>
  );
}

/* ══════════ MINES GAME ══════════ */
function MinesGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [phase,setPhase]=useState('bet');
  const [mines,setMines]=useState(new Set());
  const [rev,setRev]=useState(new Set());
  const [gems,setGems]=useState(0);
  const [mineC,setMineC]=useState(5);
  const N=25;

  const mult=useCallback(g=>{
    const safe=N-mineC; let m=1;
    for(let i=0;i<g;i++) m*=(safe-i)/(N-i);
    return Math.max(1,parseFloat((1/m*0.95).toFixed(2)));
  },[mineC]);

  const start=()=>{
    if(bet>credits) return;
    onLose(bet);
    const ms=new Set(); while(ms.size<mineC)ms.add(rnd(0,N-1));
    setMines(ms); setRev(new Set()); setGems(0); setPhase('play');
  };

  const reveal=(i)=>{
    if(phase!=='play'||rev.has(i)) return;
    const nr=new Set(rev); nr.add(i); setRev(nr);
    if(mines.has(i)){
      setRev(new Set(Array(N).keys())); setPhase('lost');
      addN('lose',`💣 Bomba! Perdeu ${fmt(bet)} créditos`);
    } else {
      const ng=gems+1; setGems(ng); track('mines');
      addN('info',`💎 Gema! Mult: ${mult(ng).toFixed(2)}×`);
    }
  };

  const cashout=()=>{
    if(phase!=='play'||gems===0) return;
    const m=mult(gems), w=Math.floor(bet*m);
    onWin(w); setPhase('won'); addN('win',`💎 ${gems} gemas × ${m.toFixed(2)}× = +${fmt(w)} créditos!`);
    if(gems>=15) blastConfetti();
  };

  const m=mult(gems);

  return (
    <div>
      <GHdr title="Mines" emoji="💣" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        {phase==='bet'&&(<>
          <div style={{marginBottom:12}}>
            <div style={{fontSize:11,color:'var(--t2)',fontWeight:600,marginBottom:7}}>MINAS NO CAMPO</div>
            <div style={{display:'flex',gap:6}}>{[3,5,8,12].map(m=>(
              <button key={m} onClick={()=>setMineC(m)}
                style={{padding:'7px 13px',borderRadius:8,border:`1px solid ${mineC===m?'rgba(239,68,68,.7)':'rgba(239,68,68,.25)'}`,background:mineC===m?'rgba(239,68,68,.25)':'rgba(9,9,26,.7)',color:mineC===m?'#fca5a5':'var(--t2)',cursor:'pointer',fontSize:12,fontWeight:700}}>
                {m} 💣
              </button>
            ))}</div>
          </div>
          <BetRow bet={bet} setBet={setBet} credits={credits}/>
          <button className="btn bgld blg" style={{width:'100%'}} onClick={start} disabled={bet>credits}>💣 INICIAR MINES</button>
        </>)}
        {(phase==='play'||phase==='lost'||phase==='won')&&(<>
          <div style={{display:'flex',justifyContent:'space-between',alignItems:'center',marginBottom:12}}>
            <div style={{fontFamily:'Orbitron',fontSize:13,color:'var(--g)'}}>💎 {gems} gemas — {m.toFixed(2)}×</div>
            <div style={{display:'flex',gap:6}}>
              {phase==='play'&&<button className="btn bgn bsm" onClick={cashout} disabled={gems===0}>💰 Cash Out ({fmt(Math.floor(bet*m))})</button>}
              {(phase==='lost'||phase==='won')&&<button className="btn bp bsm" onClick={()=>setPhase('bet')}>🔄 Novo Jogo</button>}
            </div>
          </div>
          {phase!=='play'&&<MsgBox ok={phase==='won'} msg={phase==='won'?`✅ +${fmt(Math.floor(bet*m))} créditos!`:'💥 Você pisou em uma bomba!'}/>}
          <div style={{display:'grid',gridTemplateColumns:'repeat(5,1fr)',gap:7}}>
            {Array(N).fill(0).map((_,i)=>{
              const isR=rev.has(i), isM=mines.has(i);
              return <div key={i} onClick={()=>reveal(i)} className={`mc ${!isR?'ur':isM?'bomb':'gem'}`}>{isR?(isM?'💣':'💎'):'·'}</div>;
            })}
          </div>
        </>)}
      </div>
    </div>
  );
}

/* ══════════ COIN FLIP ══════════ */
function CoinGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [choice,setChoice]=useState(null);
  const [flip,setFlip]=useState(false);
  const [res,setRes]=useState(null);
  const [coin,setCoin]=useState('🪙');
  const [stats,setStats]=useState({w:0,l:0});

  const doFlip=()=>{
    if(!choice||flip||bet>credits) return;
    setFlip(true); setRes(null); onLose(bet); track('coinflip');
    let frames=0; const tot=16;
    const ani=setInterval(()=>{
      setCoin(frames%2===0?'🟡':'⚪'); frames++;
      if(frames>=tot){
        clearInterval(ani);
        const out=Math.random()<.5?'heads':'tails';
        setCoin(out==='heads'?'👑':'🌙');
        setFlip(false);
        if(out===choice){
          const w=bet*2; onWin(w); addN('win',`${out==='heads'?'👑':'🌙'} +${fmt(w)} créditos!`);
          setRes({ok:true,msg:`${out==='heads'?'👑 CARA':'🌙 COROA'}! +${fmt(w)} créditos!`});
          setStats(s=>({...s,w:s.w+1}));
        } else {
          addN('lose',`${out==='heads'?'👑':'🌙'} — sem sorte`);
          setRes({ok:false,msg:`${out==='heads'?'👑 Cara':'🌙 Coroa'} — Você errou!`});
          setStats(s=>({...s,l:s.l+1}));
        }
      }
    },80);
  };

  return (
    <div>
      <GHdr title="Cara ou Coroa" emoji="🪙" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{textAlign:'center',marginBottom:20}}>
          <div style={{fontSize:90,marginBottom:6,transition:'all .1s',filter:flip?'blur(2px)':'none'}}>{coin}</div>
          <div style={{fontSize:12,color:'var(--t3)'}}>Créditos virtuais — sem valor real</div>
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <div style={{fontFamily:'Orbitron',fontSize:11,color:'var(--t2)',marginBottom:8,fontWeight:700}}>ESCOLHA</div>
        <div style={{display:'flex',gap:10,marginBottom:14}}>
          {[{id:'heads',label:'👑 Cara'},{id:'tails',label:'🌙 Coroa'}].map(o=>(
            <button key={o.id} onClick={()=>setChoice(o.id)} style={{flex:1,padding:'14px',borderRadius:12,border:`2px solid ${choice===o.id?'rgba(147,51,234,.8)':'rgba(147,51,234,.25)'}`,background:choice===o.id?'rgba(147,51,234,.22)':'rgba(9,9,26,.5)',color:choice===o.id?'var(--pb)':'var(--t2)',cursor:'pointer',fontFamily:'Orbitron',fontSize:14,fontWeight:700,transition:'all .2s',transform:choice===o.id?'scale(1.04)':'scale(1)'}}>
              {o.label}
            </button>
          ))}
        </div>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={doFlip} disabled={!choice||flip||bet>credits}>
          {flip?<><span className="spina">🪙</span> Girando...</>:'🪙 LANÇAR'}
        </button>
        <div style={{display:'flex',justifyContent:'space-between',marginTop:10,fontSize:11,color:'var(--t3)'}}>
          <span>Vitórias: {stats.w}</span><span>Derrotas: {stats.l}</span>
        </div>
      </div>
    </div>
  );
}

/* ══════════ DICE GAME ══════════ */
function DiceGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [target,setTarget]=useState('over');
  const [pred,setPred]=useState(4);
  const [rolling,setRolling]=useState(false);
  const [res,setRes]=useState(null);
  const [dice,setDice]=useState([3,4]);
  const faces=['⚀','⚁','⚂','⚃','⚄','⚅'];

  const roll=()=>{
    if(rolling||bet>credits) return;
    setRolling(true); setRes(null); onLose(bet); track('dice');
    let f=0; const tot=14;
    const ani=setInterval(()=>{
      setDice([rnd(1,6),rnd(1,6)]); f++;
      if(f>=tot){
        clearInterval(ani); setRolling(false);
        const d1=rnd(1,6), d2=rnd(1,6), sum=d1+d2;
        setDice([d1,d2]);
        const wins = target==='over'?sum>pred:sum<pred;
        const mult2 = target==='over'?(12-pred)/6:(pred-1)/6;
        const m = Math.max(1.1, parseFloat((mult2*1.8).toFixed(2)));
        if(wins){const w=Math.floor(bet*m);onWin(w);addN('win',`🎲 ${sum}! +${fmt(w)} créditos!`);setRes({ok:true,msg:`🎲 Total ${sum}! +${fmt(w)} créditos! (×${m})`});}
        else{addN('lose',`🎲 ${sum} — sem sorte`);setRes({ok:false,msg:`🎲 Total ${sum} — Você perdeu!`});}
      }
    },80);
  };

  return (
    <div>
      <GHdr title="Dados" emoji="🎲" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{display:'flex',gap:16,justifyContent:'center',marginBottom:18}}>
          {dice.map((d,i)=>(
            <div key={i} style={{width:80,height:80,background:'white',borderRadius:14,display:'flex',alignItems:'center',justifyContent:'center',fontSize:52,boxShadow:'0 4px 16px rgba(0,0,0,.6)',filter:rolling?'blur(3px)':'none',transition:'filter .1s'}}>
              {faces[d-1]}
            </div>
          ))}
        </div>
        <div style={{textAlign:'center',fontFamily:'Orbitron',fontSize:22,fontWeight:900,color:'var(--g)',marginBottom:10}}>
          Soma: {dice[0]+dice[1]}
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <div style={{display:'flex',gap:8,marginBottom:14}}>
          <div style={{flex:1}}>
            <div style={{fontSize:11,color:'var(--t2)',fontWeight:600,marginBottom:7}}>PREVISÃO</div>
            <div style={{display:'flex',gap:6,flexWrap:'wrap'}}>
              {[{id:'over',l:'ACIMA'},{id:'under',l:'ABAIXO'}].map(t=>(
                <button key={t.id} onClick={()=>setTarget(t.id)} style={{padding:'8px 16px',borderRadius:9,border:`1px solid ${target===t.id?'rgba(147,51,234,.7)':'rgba(147,51,234,.25)'}`,background:target===t.id?'rgba(147,51,234,.22)':'rgba(9,9,26,.7)',color:target===t.id?'var(--pb)':'var(--t2)',cursor:'pointer',fontFamily:'Orbitron',fontSize:11,fontWeight:700}}>
                  {t.l}
                </button>
              ))}
            </div>
          </div>
          <div style={{flex:1}}>
            <div style={{fontSize:11,color:'var(--t2)',fontWeight:600,marginBottom:7}}>NÚMERO</div>
            <div style={{display:'flex',gap:4,flexWrap:'wrap'}}>
              {[3,5,7,9,11].map(n=>(
                <button key={n} onClick={()=>setPred(n)} style={{padding:'7px 11px',borderRadius:8,border:`1px solid ${pred===n?'rgba(245,158,11,.7)':'rgba(245,158,11,.25)'}`,background:pred===n?'rgba(245,158,11,.22)':'rgba(9,9,26,.7)',color:pred===n?'var(--gb)':'var(--t2)',cursor:'pointer',fontSize:12,fontWeight:700}}>{n}</button>
              ))}
            </div>
          </div>
        </div>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={roll} disabled={rolling||bet>credits}>
          {rolling?<><span className="spina">🎲</span> Rolando...</>:`🎲 ROLAR (${target==='over'?'acima':'abaixo'} de ${pred})`}
        </button>
      </div>
    </div>
  );
}

/* ══════════ HIGH LOW ══════════ */
function HiLoGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [current,setCurrent]=useState(mkCard());
  const [next,setNext]=useState(null);
  const [phase,setPhase]=useState('bet');
  const [res,setRes]=useState(null);
  const [streak,setStreak]=useState(0);

  const guess=(hi)=>{
    const nc=mkCard(); setNext(nc);
    const cv=cVal(current.r), nv=cVal(nc.r);
    const correct = hi ? nv>cv : nv<cv;
    if(nv===cv){
      // Push
      setCurrent(nc); setNext(null); addN('info','Mesmo valor! Carta repetida.');
      return;
    }
    if(correct){
      const w=Math.floor(bet*1.9); onWin(w); const ns=streak+1; setStreak(ns);
      addN('win',`${hi?'Maior':'Menor'}! +${fmt(w)} créditos!`);
      setRes({ok:true,msg:`✅ ${hi?'Mais alto':'Mais baixo'}! +${fmt(w)} créditos!`});
      track('highlow');
    } else {
      addN('lose',`${hi?'Maior':'Menor'} — errou!`); setStreak(0);
      setRes({ok:false,msg:`❌ Você errou! Carta era ${nc.r}${nc.s}`});
    }
    setPhase('result');
  };

  const play=()=>{ if(bet>credits) return; onLose(bet); setPhase('play'); setRes(null); setNext(null); setCurrent(mkCard()); };

  const CardFace=({c})=>(
    <div style={{width:90,height:130,background:'white',borderRadius:12,display:'flex',flexDirection:'column',alignItems:'flex-start',padding:10,boxShadow:'0 8px 24px rgba(0,0,0,.6)',border:'1px solid rgba(0,0,0,.1)',position:'relative',flex:'0 0 auto'}}>
      <div style={{fontSize:24,fontWeight:900,color:isRed(c.s)?'#dc2626':'#111'}}>{c.r}{c.s}</div>
      <div style={{position:'absolute',bottom:8,right:8,transform:'rotate(180deg)',fontSize:20,fontWeight:900,color:isRed(c.s)?'#dc2626':'#111'}}>{c.r}{c.s}</div>
    </div>
  );

  return (
    <div>
      <GHdr title="High Low" emoji="📊" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{display:'flex',gap:16,justifyContent:'center',alignItems:'center',marginBottom:18}}>
          <CardFace c={current}/>
          <div style={{fontSize:30,color:'var(--t3)'}}>→</div>
          {next?<CardFace c={next}/>:<div style={{width:90,height:130,background:'linear-gradient(135deg,#1e1b4b,#312e81)',borderRadius:12,display:'flex',alignItems:'center',justifyContent:'center',fontSize:40,color:'rgba(255,255,255,.3)',boxShadow:'0 8px 24px rgba(0,0,0,.6)',border:'1px solid rgba(147,51,234,.3)'}}>?</div>}
        </div>
        <div style={{textAlign:'center',fontFamily:'Orbitron',fontSize:12,color:'var(--pb)',marginBottom:8}}>
          {current.r}{current.s} — Valor: {cVal(current.r)} pts {streak>0&&`| Sequência: ${streak}🔥`}
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        {phase==='bet'&&(<>
          <BetRow bet={bet} setBet={setBet} credits={credits}/>
          <button className="btn bgld blg" style={{width:'100%'}} onClick={play} disabled={bet>credits}>🃏 INICIAR</button>
        </>)}
        {phase==='play'&&(
          <div style={{display:'flex',gap:10}}>
            <button className="btn bgn blg" style={{flex:1}} onClick={()=>guess(true)}>📈 MAIOR</button>
            <button className="btn brd blg" style={{flex:1}} onClick={()=>guess(false)}>📉 MENOR</button>
          </div>
        )}
        {phase==='result'&&(
          <div style={{display:'flex',gap:8}}>
            {res?.ok&&<button className="btn bgn" style={{flex:1}} onClick={()=>{setPhase('play');setNext(null);setCurrent(next||mkCard());setRes(null);}}>▶ Continuar</button>}
            <button className="btn bp" style={{flex:res?.ok?0.6:1}} onClick={()=>setPhase('bet')}>🔄 Novo Jogo</button>
          </div>
        )}
      </div>
    </div>
  );
}

/* ══════════ WHEEL GAME ══════════ */
function WheelGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [spin,setSpin]=useState(false);
  const [res,setRes]=useState(null);
  const [rot,setRot]=useState(0);
  const canvasRef=useRef(null);
  const rotRef=useRef(0);

  const drawWheel=(angle)=>{
    const c=canvasRef.current; if(!c) return;
    const ctx=c.getContext('2d'), W=c.width, H=c.height, cx=W/2, cy=H/2, r=Math.min(W,H)/2-6;
    ctx.clearRect(0,0,W,H);
    const n=WHEEL_S.length, arc=2*Math.PI/n;
    WHEEL_S.forEach((seg,i)=>{
      const a=angle+i*arc;
      ctx.beginPath(); ctx.moveTo(cx,cy); ctx.arc(cx,cy,r,a,a+arc); ctx.closePath();
      ctx.fillStyle=seg.c; ctx.fill(); ctx.strokeStyle='rgba(0,0,0,.25)'; ctx.lineWidth=2; ctx.stroke();
      ctx.save(); ctx.translate(cx,cy); ctx.rotate(a+arc/2); ctx.textAlign='right';
      ctx.fillStyle='#fff'; ctx.font='bold 12px Orbitron,sans-serif'; ctx.shadowColor=seg.c; ctx.shadowBlur=4;
      ctx.fillText(seg.l,r-10,5); ctx.restore();
    });
    ctx.beginPath(); ctx.arc(cx,cy,20,0,2*Math.PI); ctx.fillStyle='#0d0d26'; ctx.fill();
    ctx.strokeStyle='rgba(147,51,234,.7)'; ctx.lineWidth=3; ctx.stroke();
    ctx.fillStyle='#c084fc'; ctx.font='bold 10px Orbitron,sans-serif'; ctx.textAlign='center'; ctx.textBaseline='middle';
    ctx.fillText('NV',cx,cy);
    // Pointer
    ctx.beginPath(); ctx.moveTo(cx-12,6); ctx.lineTo(cx+12,6); ctx.lineTo(cx,cy-r+5); ctx.closePath();
    ctx.fillStyle='var(--g)||#f59e0b'; ctx.fill();
  };

  useEffect(()=>{drawWheel(0);},[]);

  const doSpin=()=>{
    if(spin||bet>credits) return;
    setSpin(true); setRes(null); onLose(bet); track('wheel');
    const seg=rnd(0,WHEEL_S.length-1);
    const arc=2*Math.PI/WHEEL_S.length;
    const finalAngle=-(seg*arc)-arc/2;
    const totalRot=Math.PI*12+finalAngle-rotRef.current;
    const start=performance.now(); const dur=3500;
    const curRot=rotRef.current;
    const anim=(now)=>{
      const t=Math.min((now-start)/dur,1);
      const ease=1-Math.pow(1-t,4);
      const r=curRot+totalRot*ease;
      rotRef.current=r; drawWheel(r);
      if(t<1){requestAnimationFrame(anim);}
      else{
        setSpin(false);
        const s=WHEEL_S[seg];
        if(s.m===0){addN('lose',`BOOM! Perdeu ${fmt(bet)} créditos`);setRes({ok:false,msg:`💥 BOOM! Você perdeu ${fmt(bet)} créditos!`});}
        else{const w=Math.floor(bet*s.m);onWin(w);addN('win',`${s.l}! +${fmt(w)} créditos!`);setRes({ok:true,msg:`🎪 ${s.l}! +${fmt(w)} créditos!`});if(s.m>=4)blastConfetti();}
      }
    };
    requestAnimationFrame(anim);
  };

  return (
    <div>
      <GHdr title="Roda da Sorte" emoji="🎪" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        <div style={{position:'relative',display:'flex',justifyContent:'center',marginBottom:16}}>
          <canvas ref={canvasRef} width={280} height={280} style={{display:'block',borderRadius:'50%',border:'3px solid rgba(147,51,234,.4)',boxShadow:'0 0 30px rgba(147,51,234,.25)'}}/>
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={doSpin} disabled={spin||bet>credits}>
          {spin?<><span className="spina">🎪</span> Girando...</>:'🎪 GIRAR A RODA'}
        </button>
      </div>
    </div>
  );
}

/* ══════════ SCRATCH CARD ══════════ */
function ScratchGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [phase,setPhase]=useState('bet');
  const [cells,setCells]=useState([]);
  const [scratched,setScratched]=useState(new Set());

  const PRIZES = ['💎','⭐','🔔','🍒','💎','💰','🎯','❌','❌'];

  const buy=()=>{
    if(bet>credits) return;
    onLose(bet); track('scratch');
    // Generate 9 cells with some wins
    const arr = Array(9).fill(null).map(()=>{
      const r=Math.random();
      if(r<.08) return '💎';
      if(r<.2) return '⭐';
      if(r<.35) return '🔔';
      if(r<.5) return '🍒';
      return '❌';
    });
    // Ensure at most 3 matching
    setCells(arr); setScratched(new Set()); setPhase('play');
  };

  const scratch=(i)=>{
    if(phase!=='play'||scratched.has(i)) return;
    const ns=new Set(scratched); ns.add(i); setScratched(ns);
    if(ns.size===9){
      // Calculate winnings
      const counts = {};
      cells.forEach(c=>counts[c]=(counts[c]||0)+1);
      const mult = {'💎':20,'⭐':8,'🔔':4,'🍒':2};
      let totalW=0;
      Object.entries(counts).forEach(([sym,cnt])=>{
        if(sym!=='❌'&&cnt>=3) totalW+=Math.floor(bet*mult[sym]*(cnt-1));
      });
      if(totalW>0){onWin(totalW);addN('win',`🎟️ Raspadinha! +${fmt(totalW)} créditos!`);if(totalW>=bet*8)blastConfetti();}
      else{addN('lose',`🎟️ Sem prêmio desta vez`);}
      setPhase('done');
    }
  };

  const MULT_SHOW = {'💎':'×20','⭐':'×8','🔔':'×4','🍒':'×2','❌':''};

  return (
    <div>
      <GHdr title="Raspadinha Virtual" emoji="🎟️" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        {phase==='bet'&&(<>
          <div style={{textAlign:'center',marginBottom:16}}>
            <div style={{fontSize:13,color:'var(--t2)',lineHeight:1.6}}>Compre uma raspadinha virtual e raspe todos os campos.<br/>3 símbolos iguais = PRÊMIO VIRTUAL!</div>
            <div style={{marginTop:10,display:'flex',gap:8,justifyContent:'center',flexWrap:'wrap'}}>
              {[['💎','×20'],['⭐','×8'],['🔔','×4'],['🍒','×2']].map(([s,m])=>(
                <span key={s} style={{padding:'4px 10px',borderRadius:8,background:'rgba(147,51,234,.12)',border:'1px solid rgba(147,51,234,.3)',fontSize:12,fontWeight:700,color:'var(--pb)'}}>{s} {m}</span>
              ))}
            </div>
          </div>
          <BetRow bet={bet} setBet={setBet} credits={credits}/>
          <button className="btn bgld blg" style={{width:'100%'}} onClick={buy} disabled={bet>credits}>🎟️ COMPRAR RASPADINHA</button>
        </>)}
        {(phase==='play'||phase==='done')&&(<>
          <div style={{textAlign:'center',marginBottom:12,fontSize:12,color:'var(--t3)'}}>
            {phase==='play'?`Raspe os campos! ${9-scratched.size} restantes`:'Raspadinha completa!'}
          </div>
          <div style={{display:'grid',gridTemplateColumns:'repeat(3,1fr)',gap:10,marginBottom:14}}>
            {cells.map((c,i)=>(
              <div key={i} className={`scrc ${scratched.has(i)?'done':''}`} onClick={()=>scratch(i)}>
                <span style={{fontSize:28}}>{c}</span>
                {MULT_SHOW[c]&&<span style={{position:'absolute',bottom:3,right:5,fontSize:9,fontWeight:800,color:'rgba(255,255,255,.5)'}}>{MULT_SHOW[c]}</span>}
                {!scratched.has(i)&&<div className="scrcov">✨</div>}
              </div>
            ))}
          </div>
          {phase==='done'&&<button className="btn bp blg" style={{width:'100%'}} onClick={()=>setPhase('bet')}>🎟️ Nova Raspadinha</button>}
        </>)}
      </div>
    </div>
  );
}

/* ══════════ PLINKO GAME ══════════ */
function PlinkoGame({credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [dropping,setDropping]=useState(false);
  const [ballPos,setBallPos]=useState(null);
  const [res,setRes]=useState(null);
  const MULTS=[10,3,1.5,1,0.5,0,0.5,1,1.5,3,10];
  const ROWS=7;

  const drop=()=>{
    if(dropping||bet>credits) return;
    setDropping(true); setRes(null); onLose(bet); track('plinko');
    let col=5;
    let step=0;
    const totalSteps=ROWS;
    const anim=()=>{
      if(step<totalSteps){
        col=Math.max(0,Math.min(10,col+(Math.random()<.5?-1:1)));
        setBallPos({row:step,col});
        step++;
        setTimeout(anim,220);
      } else {
        setBallPos({row:ROWS,col,final:true});
        setDropping(false);
        const m=MULTS[col];
        if(m>0){const w=Math.floor(bet*m);onWin(w);addN('win',`⚡ Plinko ×${m}! +${fmt(w)} créditos!`);setRes({ok:true,msg:`⚡ Multiplicador ×${m}! +${fmt(w)} créditos!`,col});if(m>=5)blastConfetti();}
        else{addN('lose',`⚡ Plinko — 0×, sem ganhos`);setRes({ok:false,msg:`⚡ Multiplicador ×0 — Sem ganhos!`,col});}
        setTimeout(()=>setBallPos(null),1500);
      }
    };
    anim();
  };

  const MULT_COLORS = {10:'#f59e0b',3:'#9333ea',1.5:'#06b6d4',1:'#22c55e',0.5:'#94a3b8',0:'#ef4444'};

  return (
    <div>
      <GHdr title="Plinko" emoji="⚡" onClose={onClose}/>
      <div style={{padding:'18px 22px'}}>
        {/* Board */}
        <div style={{background:'rgba(0,0,0,.4)',borderRadius:14,padding:'14px 10px',border:'1px solid rgba(147,51,234,.22)',marginBottom:14,minHeight:200}}>
          {Array.from({length:ROWS},(_,row)=>(
            <div key={row} style={{display:'flex',justifyContent:'center',gap:8,marginBottom:10,alignItems:'center'}}>
              {Array.from({length:row+2},(_,col)=>{
                const isBall=ballPos&&ballPos.row===row&&ballPos.col===Math.round(col*(10/(row+1)));
                return (
                  <div key={col} style={{width:10,height:10,borderRadius:'50%',background:isBall?'#fde68a':'rgba(147,51,234,.7)',boxShadow:isBall?'0 0 12px #fde68a':'0 0 4px rgba(147,51,234,.4)',transition:'background .1s'}}/>
                );
              })}
            </div>
          ))}
          {/* Slots */}
          <div style={{display:'flex',gap:4,marginTop:8}}>
            {MULTS.map((m,i)=>{
              const isFinal=res?.ok!==undefined&&res.col===i;
              return (
                <div key={i} style={{flex:1,height:34,borderRadius:6,display:'flex',alignItems:'center',justifyContent:'center',fontSize:9,fontWeight:800,background:isFinal?MULT_COLORS[m]||'#6b7280':'rgba(9,9,26,.7)',border:`1px solid ${MULT_COLORS[m]||'rgba(107,114,128,.5)'}`,color:m===0?'#fca5a5':isFinal?'#000':'var(--t)',transition:'all .3s',transform:isFinal?'scale(1.1)':'scale(1)'}}>
                  {m}×
                </div>
              );
            })}
          </div>
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={drop} disabled={dropping||bet>credits}>
          {dropping?<><span className="spina">⚡</span> Caindo...</>:'⚡ SOLTAR A BOLA'}
        </button>
      </div>
    </div>
  );
}

/* ══════════ QUICK PLAY (for other games) ══════════ */
function QuickGame({g, credits, onWin, onLose, onClose, addN, track}) {
  const [bet,setBet]=useState(10);
  const [playing,setPlaying]=useState(false);
  const [res,setRes]=useState(null);

  const play=()=>{
    if(playing||bet>credits) return;
    setPlaying(true); setRes(null); onLose(bet); track(g.id);
    setTimeout(()=>{
      const r=Math.random();
      let won=false, mult=0;
      if(r<.45){mult=rnd(15,28)/10; won=true;}
      else if(r<.55){mult=1; won=true;}
      setPlaying(false);
      if(won&&mult>1){const w=Math.floor(bet*mult);onWin(w);addN('win',`${g.e} +${fmt(w)} créditos!`);setRes({ok:true,msg:`✅ Você ganhou! +${fmt(w)} créditos! (×${mult})`});}
      else if(won){onWin(bet);setRes({ok:true,msg:`🤝 Empate! Créditos devolvidos.`});}
      else{addN('lose',`${g.e} Sem sorte desta vez`);setRes({ok:false,msg:`❌ Sem sorte desta vez. Tente novamente!`});}
    }, 1200);
  };

  return (
    <div>
      <GHdr title={g.name} emoji={g.e} onClose={onClose}/>
      <div style={{padding:'20px 22px'}}>
        <div style={{textAlign:'center',marginBottom:20,padding:'20px',background:'rgba(0,0,0,.3)',borderRadius:12,border:'1px solid rgba(147,51,234,.2)'}}>
          <div style={{fontSize:72,marginBottom:10,filter:playing?'blur(4px)':'none',transition:'filter .2s'}}>{g.e}</div>
          <div style={{fontFamily:'Orbitron',fontSize:15,color:'var(--pb)',marginBottom:6}}>{g.name}</div>
          <div style={{fontSize:12,color:'var(--t2)',lineHeight:1.5}}>{g.d}</div>
        </div>
        <MsgBox ok={res?.ok} msg={res?.msg}/>
        <BetRow bet={bet} setBet={setBet} credits={credits}/>
        <button className="btn bgld blg" style={{width:'100%'}} onClick={play} disabled={playing||bet>credits}>
          {playing?<><span className="spina">⏳</span> Jogando...</>:`${g.e} JOGAR`}
        </button>
      </div>
    </div>
  );
}

/* ══════════ GAME DISPATCHER ══════════ */
const GAME_COMPS = {
  slots: SlotsGame, slots2: SlotsGame,
  blackjack: BJGame, roulette: RouletteGame, roulette2: RouletteGame,
  crash: CrashGame, mines: MinesGame, coinflip: CoinGame,
  dice: DiceGame, highlow: HiLoGame, wheel: WheelGame,
  scratch: ScratchGame, plinko: PlinkoGame,
};

function GameWindow({gameId, credits, onWin, onLose, onClose, addN, track}) {
  const G=GAMES.find(g=>g.id===gameId);
  if(!G) return null;
  const Comp=GAME_COMPS[gameId];
  return (
    <GMod onClose={onClose}>
      {Comp
        ? <Comp credits={credits} onWin={onWin} onLose={onLose} onClose={onClose} addN={addN} track={track}/>
        : <QuickGame g={G} credits={credits} onWin={onWin} onLose={onLose} onClose={onClose} addN={addN} track={track}/>
      }
    </GMod>
  );
}

/* ══════════ PAGE: HOME ══════════ */
function HomePage({credits, onPlay, favs, onFav}) {
  const featured = GAMES.filter(g=>g.hot).slice(0,4);
  const newest = GAMES.filter(g=>g.nx).slice(0,4);
  const ticker = [...RANK_DATA.slice(0,5).map(r=>`${r.av} ${r.n} ganhou ${fmt(rnd(50,500))} créditos`), '⭐ Jogue com segurança', '💎 Apenas créditos virtuais', '🎰 Sem risco, só diversão'];

  return (
    <div className="pge">
      {/* Hero */}
      <div className="hero">
        <div style={{position:'relative',zIndex:2,maxWidth:680}}>
          <div style={{display:'inline-flex',alignItems:'center',gap:8,padding:'6px 16px',borderRadius:30,background:'rgba(147,51,234,.15)',border:'1px solid rgba(147,51,234,.4)',marginBottom:20}}>
            <span style={{fontSize:14}}>✨</span>
            <span style={{fontFamily:'Orbitron',fontSize:11,color:'var(--pb)',fontWeight:700,letterSpacing:1}}>CASSINO SOCIAL — CRÉDITOS VIRTUAIS</span>
          </div>
          <h1 style={{fontFamily:'Orbitron',fontSize:'clamp(32px,5vw,56px)',fontWeight:900,lineHeight:1.1,marginBottom:18,background:'linear-gradient(135deg,#fff 20%,var(--pb) 50%,var(--cb))',WebkitBackgroundClip:'text',WebkitTextFillColor:'transparent'}}>
            Jogue com<br/>500 créditos grátis
          </h1>
          <p style={{fontSize:'clamp(14px,2vw,17px)',color:'var(--t2)',marginBottom:28,lineHeight:1.65,maxWidth:520,margin:'0 auto 28px'}}>
            Cassino social com créditos virtuais. Sem dinheiro real, sem risco, só diversão.
          </p>
          <div style={{display:'inline-flex',alignItems:'center',gap:8,padding:'8px 18px',borderRadius:30,background:'rgba(239,68,68,.12)',border:'1px solid rgba(239,68,68,.3)',marginBottom:28}}>
            <span>⚠️</span>
            <span style={{fontSize:12,color:'#fca5a5',fontWeight:600}}>Este site usa apenas créditos virtuais sem valor monetário</span>
          </div>
          <div style={{display:'flex',gap:14,justifyContent:'center',flexWrap:'wrap'}}>
            <button className="btn bgld bxl" onClick={()=>onPlay('slots')}>🎰 Começar agora</button>
            <button className="btn bout blg" onClick={()=>document.getElementById('games-section')?.scrollIntoView({behavior:'smooth'})}>🎮 Ver jogos</button>
          </div>
        </div>
      </div>

      {/* Ticker */}
      <div style={{background:'rgba(9,9,26,.9)',borderTop:'1px solid rgba(147,51,234,.2)',borderBottom:'1px solid rgba(147,51,234,.2)',padding:'10px 0',overflow:'hidden'}}>
        <div className="ticker">
          <div className="tick-i">
            {[...ticker,...ticker].map((t,i)=>(
              <span key={i} style={{fontSize:12,color:'var(--t2)',display:'flex',alignItems:'center',gap:8,whiteSpace:'nowrap'}}>
                <span style={{color:'var(--p)',fontSize:8}}>◆</span>{t}
              </span>
            ))}
          </div>
        </div>
      </div>

      {/* Stats */}
      <div style={{maxWidth:1200,margin:'0 auto',padding:'40px 20px'}}>
        <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fit,minmax(140px,1fr))',gap:14,marginBottom:40}}>
          {[['🎮','20+','Jogos','disponíveis'],['👥','10K+','Jogadores','ativos'],['💎','500','Créditos','iniciais grátis'],['🏆','Diário','Bônus','gratuito']].map(([e,v,l,s])=>(
            <div key={l} className="glass" style={{padding:'16px',textAlign:'center'}}>
              <div style={{fontSize:24,marginBottom:6}}>{e}</div>
              <div style={{fontFamily:'Orbitron',fontSize:20,fontWeight:900,color:'var(--g)'}}>{v}</div>
              <div style={{fontSize:11,fontWeight:700,color:'var(--pb)',textTransform:'uppercase',letterSpacing:.5}}>{l}</div>
              <div style={{fontSize:10,color:'var(--t3)',marginTop:2}}>{s}</div>
            </div>
          ))}
        </div>

        {/* Featured */}
        <div id="games-section">
          <div className="stitle">
            <span style={{fontFamily:'Orbitron',fontSize:15,fontWeight:900,color:'var(--t)'}}>🔥 Mais Populares</span>
          </div>
          <div className="ggrid" style={{marginBottom:40}}>
            {featured.map(g=><GCard key={g.id} g={g} onPlay={onPlay} fav={favs.has(g.id)} onFav={onFav}/>)}
          </div>

          <div className="stitle">
            <span style={{fontFamily:'Orbitron',fontSize:15,fontWeight:900,color:'var(--t)'}}>✨ Novidades</span>
          </div>
          <div className="ggrid">
            {newest.map(g=><GCard key={g.id} g={g} onPlay={onPlay} fav={favs.has(g.id)} onFav={onFav}/>)}
          </div>
        </div>
      </div>
    </div>
  );
}

/* ══════════ PAGE: GAMES ══════════ */
function GamesPage({onPlay, favs, onFav, search, setSearch}) {
  const [cat,setCat]=useState('all');
  const cats=[{id:'all',label:'🎮 Todos'},{id:'slots',label:'🎰 Slots'},{id:'table',label:'🃏 Mesa'},{id:'mini',label:'⚡ Mini'},{id:'other',label:'📢 Outros'},{id:'fav',label:'⭐ Favoritos'}];
  const filtered=GAMES.filter(g=>{
    if(cat==='fav') return favs.has(g.id);
    if(cat!=='all'&&g.cat!==cat) return false;
    if(search&&!g.name.toLowerCase().includes(search.toLowerCase())) return false;
    return true;
  });

  return (
    <div className="pge" style={{maxWidth:1200,margin:'0 auto',padding:'30px 20px'}}>
      <div style={{marginBottom:24}}>
        <h1 style={{fontFamily:'Orbitron',fontSize:24,fontWeight:900,marginBottom:6}}>🎮 Todos os Jogos</h1>
        <p style={{fontSize:13,color:'var(--t2)'}}>20 jogos com créditos virtuais — sem dinheiro real</p>
      </div>
      {/* Search + Filters */}
      <div style={{display:'flex',gap:12,marginBottom:20,flexWrap:'wrap',alignItems:'center'}}>
        <input className="nvin" placeholder="🔍 Buscar jogo..." value={search} onChange={e=>setSearch(e.target.value)} style={{maxWidth:260}}/>
        <div style={{display:'flex',gap:6,flexWrap:'wrap'}}>
          {cats.map(c=><button key={c.id} className={`ctab ${cat===c.id?'act':''}`} onClick={()=>setCat(c.id)}>{c.label}</button>)}
        </div>
      </div>
      {filtered.length===0
        ?<div style={{textAlign:'center',padding:'60px 20px',color:'var(--t3)'}}>
           <div style={{fontSize:48,marginBottom:12}}>🔍</div>
           <div style={{fontFamily:'Orbitron',fontSize:14}}>Nenhum jogo encontrado</div>
         </div>
        :<div className="ggrid">
           {filtered.map(g=><GCard key={g.id} g={g} onPlay={onPlay} fav={favs.has(g.id)} onFav={onFav}/>)}
         </div>
      }
    </div>
  );
}

/* ══════════ PAGE: MISSIONS ══════════ */
function MissionsPage({missions, onClaim}) {
  return (
    <div className="pge" style={{maxWidth:800,margin:'0 auto',padding:'30px 20px'}}>
      <div style={{marginBottom:24}}>
        <h1 style={{fontFamily:'Orbitron',fontSize:22,fontWeight:900,marginBottom:6}}>🎯 Missões Diárias</h1>
        <p style={{fontSize:13,color:'var(--t2)'}}>Complete missões para ganhar créditos virtuais bônus</p>
      </div>
      <div style={{display:'flex',flexDirection:'column',gap:12}}>
        {missions.map(m=>{
          const pct=Math.min(100,Math.round(m.p/m.g*100));
          const done=m.p>=m.g;
          return (
            <div key={m.id} className={`mcard ${done&&!m.claimed?'clm':m.claimed?'done':''}`}>
              <div style={{fontSize:32,flexShrink:0}}>{m.e}</div>
              <div style={{flex:1,minWidth:0}}>
                <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',marginBottom:4,gap:10}}>
                  <div style={{fontFamily:'Orbitron',fontSize:13,fontWeight:700,color:m.claimed?'var(--t3)':'var(--t)'}}>{m.n}</div>
                  <span className={`bdg ${m.claimed?'bdgr':done?'bdgg':'bdgp'}`}>{m.claimed?'Resgatado':done?'Pronto!':m.p+'/'+m.g}</span>
                </div>
                <div style={{fontSize:12,color:'var(--t2)',marginBottom:8}}>{m.d}</div>
                <div className="prog"><div className="progb" style={{width:pct+'%',background:m.claimed?'rgba(100,116,139,.4)':done?'linear-gradient(90deg,#22c55e,#16a34a)':'linear-gradient(90deg,var(--p),var(--c))'}}/></div>
              </div>
              <div style={{flexShrink:0,textAlign:'center'}}>
                <div style={{fontFamily:'Orbitron',fontSize:13,fontWeight:900,color:'var(--g)',marginBottom:6}}>+{m.r}</div>
                <div style={{fontSize:10,color:'var(--t3)',marginBottom:8}}>créditos</div>
                <button className={`btn bsm ${done&&!m.claimed?'bgld':m.claimed?'bout':''}`}
                  style={{opacity:(!done||m.claimed)?.4:1,cursor:done&&!m.claimed?'pointer':'not-allowed',fontSize:9}}
                  onClick={()=>done&&!m.claimed&&onClaim(m.id)}
                  disabled={!done||m.claimed}>
                  {m.claimed?'✓ Pego':'Resgatar'}
                </button>
              </div>
            </div>
          );
        })}
      </div>
      {/* Achievements */}
      <div style={{marginTop:36}}>
        <div className="stitle"><span style={{fontFamily:'Orbitron',fontSize:15,fontWeight:900}}>🏆 Conquistas</span></div>
        <div style={{display:'grid',gridTemplateColumns:'repeat(auto-fill,minmax(250px,1fr))',gap:12}}>
          {ACHIEVE0.map(a=>(
            <div key={a.id} className="glass" style={{padding:'14px',display:'flex',gap:12,alignItems:'center',opacity:.5}}>
              <div style={{fontSize:26}}>{a.e}</div>
              <div><div style={{fontFamily:'Orbitron',fontSize:11,fontWeight:700,marginBottom:3}}>{a.n}</div><div style={{fontSize:11,color:'var(--t2)'}}>{a.d}</div></div>
              <div style={{marginLeft:'auto',fontSize:10,color:'var(--t3)',flexShrink:0}}>🔒</div>
            </div>
          ))}
        </div>
      </div>
    </div>
  );
}

/* ══════════ PAGE: RANKING ══════════ */
function RankingPage({credits, user}) {
  const myRank = user ? [...RANK_DATA, {n:user.nick,av:user.av,cr:credits,w:user.wins||0}].sort((a,b)=>b.cr-a.cr).findIndex(r=>r.n===user.nick)+1 : null;
  const rankMedal = i => i===0?'🥇':i===1?'🥈':i===2?'🥉':`#${i+1}`;

  return (
    <div className="pge" style={{maxWidth:700,margin:'0 auto',padding:'30px 20px'}}>
      <div style={{marginBottom:24}}>
        <h1 style={{fontFamily:'Orbitron',fontSize:22,fontWeight:900,marginBottom:6}}>🏆 Ranking Semanal</h1>
        <p style={{fontSize:13,color:'var(--t2)'}}>Os maiores acumuladores de créditos virtuais da semana</p>
      </div>
      {user&&myRank&&(
        <div className="glass" style={{padding:'14px 18px',marginBottom:20,display:'flex',alignItems:'center',gap:12,border:'1px solid rgba(147,51,234,.4)'}}>
          <div style={{fontFamily:'Orbitron',fontSize:20,fontWeight:900,color:'var(--g)',width:40,textAlign:'center'}}>{rankMedal(myRank-1)}</div>
          <div className="av">{user.av}</div>
          <div style={{flex:1}}>
            <div style={{fontFamily:'Orbitron',fontSize:13,fontWeight:700,color:'var(--pb)'}}>{user.nick} <span style={{fontSize:10,color:'var(--t3)'}}>(você)</span></div>
            <div style={{fontSize:11,color:'var(--t2)',marginTop:2}}>{fmt(credits)} créditos virtuais</div>
          </div>
        </div>
      )}
      {RANK_DATA.map((r,i)=>(
        <div key={i} className={`rrow ${i===0?'r1':i===1?'r2':i===2?'r3':''}`}>
          <div style={{fontFamily:'Orbitron',fontSize:18,fontWeight:900,color:i===0?'var(--g)':i===1?'#94a3b8':'#cd7f32',width:36,textAlign:'center',flexShrink:0}}>{rankMedal(i)}</div>
          <div className="av">{r.av}</div>
          <div style={{flex:1,minWidth:0}}>
            <div style={{fontFamily:'Orbitron',fontSize:12,fontWeight:700,color:'var(--t)',overflow:'hidden',textOverflow:'ellipsis',whiteSpace:'nowrap'}}>{r.n}</div>
            <div style={{fontSize:11,color:'var(--t2)',marginTop:2}}>🏆 {r.w} vitórias esta semana</div>
          </div>
          <div style={{textAlign:'right',flexShrink:0}}>
            <div style={{fontFamily:'Orbitron',fontSize:14,fontWeight:900,color:'var(--g)'}}>{fmt(r.cr)}</div>
            <div style={{fontSize:10,color:'var(--t3)'}}>créditos</div>
          </div>
        </div>
      ))}
      <div style={{marginTop:20,padding:'14px',borderRadius:12,background:'rgba(239,68,68,.08)',border:'1px solid rgba(239,68,68,.2)',textAlign:'center',fontSize:12,color:'#fca5a5'}}>
        ⚠️ Créditos sem valor monetário — não podem ser sacados ou trocados
      </div>
    </div>
  );
}

/* ══════════ PAGE: PROFILE ══════════ */
function ProfilePage({credits, user, onAvatarChange, history, onDailyBonus, lastBonus}) {
  const canBonus = !lastBonus || (Date.now()-lastBonus) > 3600000;
  const wins = history.filter(h=>h.won).length;
  const losses = history.filter(h=>!h.won).length;
  const totalBet = history.reduce((a,h)=>a+h.bet,0);
  const totalWon = history.filter(h=>h.won).reduce((a,h)=>a+h.won,0);

  return (
    <div className="pge" style={{maxWidth:700,margin:'0 auto',padding:'30px 20px'}}>
      {/* Profile Card */}
      <div className="glass" style={{padding:'24px',marginBottom:20,display:'flex',alignItems:'center',gap:20,flexWrap:'wrap'}}>
        <div style={{position:'relative'}}>
          <div style={{width:72,height:72,borderRadius:'50%',border:'3px solid rgba(147,51,234,.6)',background:'linear-gradient(135deg,rgba(147,51,234,.3),rgba(6,182,212,.2))',display:'flex',alignItems:'center',justifyContent:'center',fontSize:38,boxShadow:'0 0 20px rgba(147,51,234,.3)'}}>{user?.av||'👤'}</div>
        </div>
        <div style={{flex:1,minWidth:200}}>
          <div style={{fontFamily:'Orbitron',fontSize:20,fontWeight:900,color:'var(--t)',marginBottom:4}}>{user?.nick||'Jogador'}</div>
          <div style={{display:'flex',gap:8,flexWrap:'wrap'}}>
            <span className="bdg bdgp">Nível 1</span>
            <span className="bdgg">🎮 {history.length} jogos</span>
          </div>
          <div style={{marginTop:12}}>
            <div style={{display:'flex',justifyContent:'space-between',fontSize:11,color:'var(--t2)',marginBottom:4}}>
              <span>XP: 0 / 100</span><span>→ Nível 2</span>
            </div>
            <div className="prog"><div className="progb" style={{width:'5%',background:'linear-gradient(90deg,var(--p),var(--c))'}}/></div>
          </div>
        </div>
        <div style={{textAlign:'center'}}>
          <div style={{fontFamily:'Orbitron',fontSize:28,fontWeight:900,color:'var(--g)'}}>{fmt(credits)}</div>
          <div style={{fontSize:11,color:'var(--t2)'}}>créditos virtuais</div>
        </div>
      </div>

      {/* Daily Bonus */}
      <div className="glass" style={{padding:'18px',marginBottom:20,border:canBonus?'1px solid rgba(245,158,11,.5)':'1px solid rgba(147,51,234,.2)',background:canBonus?'rgba(245,158,11,.06)':undefined}}>
        <div style={{display:'flex',alignItems:'center',justifyContent:'space-between',gap:14}}>
          <div>
            <div style={{fontFamily:'Orbitron',fontSize:14,fontWeight:700,color:canBonus?'var(--g)':'var(--t2)',marginBottom:4}}>🎁 Bônus Diário</div>
            <div style={{fontSize:12,color:'var(--t2)'}}>Recompensa: <strong style={{color:'var(--g)'}}>+100 créditos virtuais grátis!</strong></div>
            {!canBonus&&<div style={{fontSize:11,color:'var(--t3)',marginTop:3}}>✓ Coletado hoje — volte em 1 hora</div>}
          </div>
          <button className={`btn ${canBonus?'bgld':'bout'} bsm`} onClick={canBonus?onDailyBonus:undefined} disabled={!canBonus}>
            {canBonus?'🎁 COLETAR':'✓ Coletado'}
          </button>
        </div>
      </div>

      {/* Stats */}
      <div style={{display:'grid',gridTemplateColumns:'repeat(2,1fr)',gap:14,marginBottom:20}}>
        {[['🏆','Vitórias',wins,'#86efac'],['❌','Derrotas',losses,'#fca5a5'],['🎲','Apostas',totalBet+' cr','var(--cb)'],['💰','Ganhos',totalWon+' cr','var(--g)']].map(([e,l,v,c])=>(
          <div key={l} className="glass" style={{padding:'14px',textAlign:'center'}}>
            <div style={{fontSize:22,marginBottom:4}}>{e}</div>
            <div style={{fontFamily:'Orbitron',fontSize:18,fontWeight:900,color:c}}>{fmt_safe(v)}</div>
            <div style={{fontSize:11,color:'var(--t2)'}}>{l}</div>
          </div>
        ))}
      </div>

      {/* Avatar Picker */}
      <div className="glass" style={{padding:'18px'}}>
        <div style={{fontFamily:'Orbitron',fontSize:13,fontWeight:700,marginBottom:12}}>🎭 Escolha seu avatar</div>
        <div style={{display:'flex',gap:8,flexWrap:'wrap'}}>
          {AVS.map(a=>(
            <button key={a} onClick={()=>onAvatarChange(a)}
              style={{width:44,height:44,borderRadius:'50%',border:`2px solid ${user?.av===a?'rgba(147,51,234,.8)':'rgba(147,51,234,.2)'}`,background:user?.av===a?'rgba(147,51,234,.25)':'rgba(9,9,26,.5)',fontSize:22,cursor:'pointer',transition:'all .2s',transform:user?.av===a?'scale(1.1)':'scale(1)'}}>
              {a}
            </button>
          ))}
        </div>
      </div>

      {/* History */}
      {history.length>0&&(
        <div style={{marginTop:20}}>
          <div className="stitle"><span style={{fontFamily:'Orbitron',fontSize:13,fontWeight:900}}>📋 Histórico Recente</span></div>
          <div style={{display:'flex',flexDirection:'column',gap:6}}>
            {history.slice(-8).reverse().map((h,i)=>(
              <div key={i} style={{display:'flex',alignItems:'center',gap:12,padding:'10px 14px',borderRadius:9,background:'rgba(9,9,26,.7)',border:'1px solid rgba(147,51,234,.12)'}}>
                <span style={{fontSize:18}}>{GAMES.find(g=>g.id===h.game)?.e||'🎲'}</span>
                <span style={{flex:1,fontSize:12,color:'var(--t2)'}}>{GAMES.find(g=>g.id===h.game)?.name||h.game}</span>
                <span style={{fontSize:11,color:'var(--t3)'}}>-{h.bet}</span>
                <span style={{fontFamily:'Orbitron',fontSize:12,fontWeight:700,color:h.won>0?'#86efac':'#fca5a5'}}>{h.won>0?'+'+fmt(h.won):'−'+fmt(h.bet)}</span>
              </div>
            ))}
          </div>
        </div>
      )}
      <div style={{marginTop:20,padding:'14px',borderRadius:12,background:'rgba(239,68,68,.08)',border:'1px solid rgba(239,68,68,.2)',textAlign:'center',fontSize:12,color:'#fca5a5'}}>
        ⚠️ Créditos virtuais sem valor monetário. Não podem ser comprados, sacados ou convertidos.
      </div>
    </div>
  );
}

function fmt_safe(v) {
  if(typeof v==='number') return fmt(v);
  const n=parseInt(String(v).replace(/\D/g,''));
  return isNaN(n)?v:fmt(n)+' cr';
}

/* ══════════ PAGE: RULES ══════════ */
function RulesPage() {
  const items = [
    ['🎁','Créditos Virtuais','Todo usuário começa com 500 créditos virtuais gratuitos. Esses créditos não têm valor monetário e não podem ser comprados, vendidos, sacados ou convertidos.'],
    ['🎮','Como Jogar','Escolha qualquer jogo da biblioteca, defina sua aposta em créditos virtuais e jogue. Os créditos ganhos são computados no seu saldo virtual.'],
    ['📅','Bônus Diário','Você pode resgatar 100 créditos virtuais gratuitos a cada 1 hora visitando a página de Perfil. Nenhum pagamento é necessário.'],
    ['🎯','Missões','Complete missões diárias para ganhar créditos virtuais bônus. Missões resetam periodicamente.'],
    ['⚠️','Sem Dinheiro Real','Neon Vault Casino é uma plataforma de entretenimento. NUNCA existe depósito, saque, Pix, cartão, criptomoeda ou qualquer transação financeira.'],
    ['🔒','Segurança','Não coletamos dados financeiros. Este é um jogo social gratuito voltado para entretenimento responsável.'],
  ];
  return (
    <div className="pge" style={{maxWidth:760,margin:'0 auto',padding:'30px 20px'}}>
      <div style={{marginBottom:28}}>
        <h1 style={{fontFamily:'Orbitron',fontSize:22,fontWeight:900,marginBottom:6}}>📋 Regras e Segurança</h1>
        <p style={{fontSize:13,color:'var(--t2)'}}>Neon Vault Casino — plataforma de entretenimento social</p>
      </div>
      <div style={{display:'flex',flexDirection:'column',gap:14}}>
        {items.map(([e,t,d])=>(
          <div key={t} className="glass" style={{padding:'18px',display:'flex',gap:16}}>
            <div style={{fontSize:30,flexShrink:0}}>{e}</div>
            <div><div style={{fontFamily:'Orbitron',fontSize:13,fontWeight:700,marginBottom:6,color:'var(--pb)'}}>{t}</div><div style={{fontSize:13,color:'var(--t2)',lineHeight:1.6}}>{d}</div></div>
          </div>
        ))}
      </div>
      <div style={{marginTop:28,padding:'20px',borderRadius:16,background:'rgba(239,68,68,.08)',border:'2px solid rgba(239,68,68,.3)',textAlign:'center'}}>
        <div style={{fontSize:28,marginBottom:8}}>⚠️</div>
        <div style={{fontFamily:'Orbitron',fontSize:14,fontWeight:900,color:'#fca5a5',marginBottom:8}}>AVISO IMPORTANTE</div>
        <div style={{fontSize:13,color:'#fca5a5',lineHeight:1.6}}>
          Neon Vault Casino é uma plataforma fictícia de entretenimento.<br/>
          Todos os créditos são virtuais, não possuem valor monetário<br/>
          e não podem ser comprados, vendidos, sacados ou trocados por prêmios reais.
        </div>
      </div>
    </div>
  );
}

/* ══════════ REGISTER MODAL ══════════ */
function RegisterModal({onRegister}) {
  const [nick,setNick]=useState('');
  const [av,setAv]=useState(AVS[0]);
  const [err,setErr]=useState('');

  const submit=()=>{
    if(!nick.trim()||nick.length<2){setErr('Nickname deve ter pelo menos 2 caracteres');return;}
    if(nick.length>18){setErr('Nickname deve ter no máximo 18 caracteres');return;}
    onRegister({nick:nick.trim(),av});
  };

  return (
    <div className="regbg">
      <div style={{background:'linear-gradient(155deg,#0b0b1e,#0f0f28)',border:'1px solid rgba(147,51,234,.45)',borderRadius:24,padding:'36px 32px',width:'100%',maxWidth:440,animation:'popin .4s cubic-bezier(.34,1.56,.64,1)',boxShadow:'0 0 60px rgba(147,51,234,.25),0 40px 80px rgba(0,0,0,.7)',textAlign:'center'}}>
        <div style={{fontFamily:'Orbitron',fontSize:28,fontWeight:900,background:'linear-gradient(135deg,var(--g),var(--pb))',WebkitBackgroundClip:'text',WebkitTextFillColor:'transparent',marginBottom:4}}>NEON VAULT</div>
        <div style={{fontFamily:'Orbitron',fontSize:13,color:'var(--pb)',marginBottom:6,letterSpacing:3}}>CASINO</div>
        <div style={{fontSize:12,color:'var(--t3)',marginBottom:24,padding:'8px 16px',background:'rgba(239,68,68,.08)',border:'1px solid rgba(239,68,68,.2)',borderRadius:20}}>⚠️ Apenas créditos virtuais — sem dinheiro real</div>
        <div style={{fontSize:13,color:'var(--t2)',marginBottom:20,lineHeight:1.5}}>Crie seu perfil gratuito e receba<br/><strong style={{color:'var(--g)',fontFamily:'Orbitron',fontSize:16}}>500 créditos virtuais</strong> para começar!</div>
        <div style={{marginBottom:16,textAlign:'left'}}>
          <label style={{fontSize:11,color:'var(--t2)',fontWeight:600,display:'block',marginBottom:6,fontFamily:'Orbitron',textTransform:'uppercase',letterSpacing:.5}}>Seu Nickname</label>
          <input className="nvin" placeholder="ex: LuckyPlayer99" value={nick} onChange={e=>setNick(e.target.value)} onKeyDown={e=>e.key==='Enter'&&submit()} maxLength={18} style={{fontSize:16}}/>
          {err&&<div style={{fontSize:11,color:'#fca5a5',marginTop:6}}>{err}</div>}
        </div>
        <div style={{marginBottom:24,textAlign:'left'}}>
          <label style={{fontSize:11,color:'var(--t2)',fontWeight:600,display:'block',marginBottom:8,fontFamily:'Orbitron',textTransform:'uppercase',letterSpacing:.5}}>Avatar</label>
          <div style={{display:'flex',gap:7,flexWrap:'wrap'}}>
            {AVS.map(a=><button key={a} onClick={()=>setAv(a)} style={{width:40,height:40,borderRadius:'50%',border:`2px solid ${av===a?'rgba(147,51,234,.8)':'rgba(147,51,234,.2)'}`,background:av===a?'rgba(147,51,234,.25)':'rgba(9,9,26,.5)',fontSize:20,cursor:'pointer',transition:'all .2s'}}>{a}</button>)}
          </div>
        </div>
        <button className="btn bgld bxl" style={{width:'100%'}} onClick={submit}>🎰 Começar Agora — Grátis!</button>
        <div style={{fontSize:10,color:'var(--t3)',marginTop:12,lineHeight:1.5}}>Ao continuar, você confirma que entende que estes créditos são virtuais, sem valor monetário.</div>
      </div>
    </div>
  );
}

/* ══════════ MAIN APP ══════════ */
export default function NeonVaultCasino() {
  /* ── Inject CSS ── */
  useEffect(()=>{
    if(!document.getElementById('nv-font')){
      const l=document.createElement('link'); l.id='nv-font'; l.rel='stylesheet';
      l.href='https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;700;900&family=Exo+2:wght@300;400;500;600;700&display=swap';
      document.head.appendChild(l);
    }
    if(!document.getElementById('nv-css')){
      const s=document.createElement('style'); s.id='nv-css'; s.textContent=CSS;
      document.head.appendChild(s);
    }
  },[]);

  /* ── State ── */
  const [user,setUser]=useState(null);
  const [credits,setCredits]=useState(500);
  const [page,setPage]=useState('home');
  const [activeGame,setActiveGame]=useState(null);
  const [notifs,setNotifs]=useState([]);
  const [missions,setMissions]=useState(MISSIONS0.map(m=>({...m})));
  const [favs,setFavs]=useState(new Set());
  const [history,setHistory]=useState([]);
  const [search,setSearch]=useState('');
  const [lastBonus,setLastBonus]=useState(null);
  const [gamesPlayed,setGamesPlayed]=useState(new Set());
  const notifId=useRef(0);
  const creditKeyRef=useRef(null);

  /* ── Notifications ── */
  const addN=useCallback((t,msg)=>{
    const id=++notifId.current;
    setNotifs(ns=>[...ns,{id,t,msg}]);
    setTimeout(()=>setNotifs(ns=>ns.map(n=>n.id===id?{...n,out:true}:n)),3200);
    setTimeout(()=>setNotifs(ns=>ns.filter(n=>n.id!==id)),3600);
  },[]);

  /* ── Credits animation ── */
  const updateCredits=(delta)=>{
    setCredits(c=>Math.max(0,c+delta));
    if(creditKeyRef.current){
      creditKeyRef.current.classList.remove('cpop');
      void creditKeyRef.current.offsetWidth;
      creditKeyRef.current.classList.add('cpop');
    }
  };

  /* ── Game callbacks ── */
  const onWin=useCallback((amt)=>{
    updateCredits(+amt);
    setHistory(h=>[...h.slice(-29),{game:activeGame,won:amt,bet:0,ts:Date.now()}]);
  },[activeGame]);

  const onLose=useCallback((amt)=>{
    updateCredits(-amt);
    setHistory(h=>{
      const last=[...h];
      if(last.length&&!last[last.length-1].bet) last[last.length-1]={...last[last.length-1],bet:amt};
      else last.push({game:activeGame,won:0,bet:amt,ts:Date.now()});
      return last.slice(-30);
    });
  },[activeGame]);

  /* ── Mission tracker ── */
  const track=useCallback((type)=>{
    setGamesPlayed(gp=>{
      const ngp=new Set(gp); ngp.add(type);
      setMissions(ms=>ms.map(m=>{
        if(m.claimed) return m;
        let np=m.p;
        if(m.t===type&&m.p<m.g) np=m.p+1;
        if(m.t==='explore'&&ngp.size>m.p&&m.p<m.g) np=Math.min(m.g,ngp.size);
        return np!==m.p?{...m,p:np}:m;
      }));
      return ngp;
    });
  },[]);

  /* ── Claim mission ── */
  const claimMission=useCallback((id)=>{
    setMissions(ms=>ms.map(m=>m.id===id&&m.p>=m.g&&!m.claimed?{...m,claimed:true}:m));
    const m=missions.find(m=>m.id===id);
    if(m){updateCredits(m.r); addN('bonus',`🎯 Missão "${m.n}" completa! +${m.r} créditos!`);}
  },[missions,addN]);

  /* ── Daily bonus ── */
  const onDailyBonus=useCallback(()=>{
    updateCredits(100); setLastBonus(Date.now());
    addN('bonus','🎁 Bônus diário! +100 créditos virtuais!');
    blastConfetti();
  },[addN]);

  /* ── Play game ── */
  const openGame=useCallback((id)=>{
    setActiveGame(id);
  },[]);

  /* ── Empty credits check ── */
  const noCredits=credits<=0;

  /* ── Nav pages ── */
  const NAV=[
    {id:'home',   label:'Início',    e:'🏠'},
    {id:'games',  label:'Jogos',     e:'🎮'},
    {id:'missions',label:'Missões',  e:'🎯'},
    {id:'ranking',label:'Ranking',   e:'🏆'},
    {id:'profile',label:'Perfil',    e:'👤'},
    {id:'rules',  label:'Regras',    e:'📋'},
  ];

  if(!user) return <RegisterModal onRegister={u=>{setUser(u);addN('bonus',`Bem-vindo, ${u.nick}! +500 créditos virtuais!`);}}/>;

  return (
    <div style={{minHeight:'100vh',position:'relative'}}>
      <Particles/>
      <Notifs ns={notifs}/>

      {/* NAVBAR */}
      <nav className="glass desknav" style={{position:'fixed',top:0,left:0,right:0,z:50,padding:'0 20px',height:62,display:'flex',alignItems:'center',justifyContent:'space-between',gap:16,borderRadius:0,borderTop:'none',borderLeft:'none',borderRight:'none',borderBottom:'1px solid rgba(147,51,234,.2)',zIndex:500}}>
        <div style={{display:'flex',alignItems:'center',gap:14,flexShrink:0}}>
          <div style={{fontFamily:'Orbitron',fontWeight:900,fontSize:16,background:'linear-gradient(135deg,var(--g),var(--pb))',WebkitBackgroundClip:'text',WebkitTextFillColor:'transparent',cursor:'pointer'}} onClick={()=>setPage('home')}>⚡ NEON VAULT</div>
        </div>
        <div style={{display:'flex',gap:4,overflow:'auto',flexWrap:'nowrap'}}>
          {NAV.map(n=><button key={n.id} className={`navi ${page===n.id?'act':''}`} onClick={()=>setPage(n.id)}>{n.e} {n.label}</button>)}
        </div>
        {/* Credits */}
        <div className="cpill" ref={creditKeyRef} style={{flexShrink:0}}>
          <span style={{fontSize:16}}>💰</span>
          <div>
            <div style={{fontFamily:'Orbitron',fontSize:15,fontWeight:900,color:'var(--g)',lineHeight:1}}>{fmt(credits)}</div>
            <div style={{fontSize:9,color:'var(--t3)',letterSpacing:.5,textTransform:'uppercase'}}>créditos</div>
          </div>
          <div className="av" style={{width:30,height:30,fontSize:14}}>{user.av}</div>
        </div>
      </nav>

      {/* BOTTOM NAV (mobile) */}
      <div className="bnav" style={{display:'flex',zIndex:500}}>
        {NAV.slice(0,5).map(n=>(
          <div key={n.id} className={`bni ${page===n.id?'act':''}`} onClick={()=>setPage(n.id)}>
            <span style={{fontSize:20}}>{n.e}</span>
            <span>{n.label}</span>
          </div>
        ))}
      </div>

      {/* MAIN CONTENT */}
      <div className="mainpad" style={{paddingTop:66,position:'relative',zIndex:1}}>
        {noCredits&&!activeGame&&(
          <div style={{position:'fixed',bottom:80,left:'50%',transform:'translateX(-50%)',zIndex:400,maxWidth:360,width:'100%',padding:'0 16px'}}>
            <div style={{background:'linear-gradient(135deg,rgba(245,158,11,.95),rgba(234,88,12,.9))',borderRadius:16,padding:'16px 20px',textAlign:'center',boxShadow:'0 0 30px rgba(245,158,11,.4)'}}>
              <div style={{fontFamily:'Orbitron',fontSize:14,fontWeight:900,color:'#000',marginBottom:6}}>💰 Créditos Zerados!</div>
              <div style={{fontSize:12,color:'rgba(0,0,0,.7)',marginBottom:12}}>Colete seu bônus diário gratuito!</div>
              <button className="btn" style={{background:'#000',color:'var(--g)',padding:'10px 24px',fontSize:12}} onClick={()=>{setPage('profile');onDailyBonus();}}>🎁 Coletar Bônus Agora</button>
            </div>
          </div>
        )}

        {page==='home'&&<HomePage credits={credits} onPlay={openGame} favs={favs} onFav={id=>setFavs(f=>{const nf=new Set(f);nf.has(id)?nf.delete(id):nf.add(id);return nf;})}/>}
        {page==='games'&&<GamesPage onPlay={openGame} favs={favs} onFav={id=>setFavs(f=>{const nf=new Set(f);nf.has(id)?nf.delete(id):nf.add(id);return nf;})} search={search} setSearch={setSearch}/>}
        {page==='missions'&&<MissionsPage missions={missions} onClaim={claimMission}/>}
        {page==='ranking'&&<RankingPage credits={credits} user={user}/>}
        {page==='profile'&&<ProfilePage credits={credits} user={user} onAvatarChange={av=>setUser(u=>({...u,av}))} history={history} onDailyBonus={onDailyBonus} lastBonus={lastBonus}/>}
        {page==='rules'&&<RulesPage/>}
      </div>

      {/* GAME WINDOW */}
      {activeGame&&(
        <GameWindow
          gameId={activeGame}
          credits={credits}
          onWin={onWin}
          onLose={onLose}
          onClose={()=>setActiveGame(null)}
          addN={addN}
          track={track}
        />
      )}

      {/* FOOTER */}
      {!activeGame&&(
        <footer style={{position:'relative',zIndex:1,borderTop:'1px solid rgba(147,51,234,.15)',padding:'24px 20px',textAlign:'center',background:'rgba(6,6,15,.8)',marginTop:40}}>
          <div style={{fontFamily:'Orbitron',fontSize:14,fontWeight:700,color:'var(--pb)',marginBottom:10}}>⚡ NEON VAULT CASINO</div>
          <div style={{fontSize:12,color:'var(--t3)',maxWidth:600,margin:'0 auto',lineHeight:1.7}}>
            Neon Vault Casino é uma plataforma fictícia de entretenimento. Todos os créditos são virtuais, não possuem valor monetário e não podem ser comprados, vendidos, sacados ou trocados por prêmios reais.
          </div>
          <div style={{display:'flex',gap:8,justifyContent:'center',marginTop:14,flexWrap:'wrap'}}>
            {['🎰 Entretenimento Social','💎 Sem Dinheiro Real','🔒 100% Seguro','✅ Créditos Virtuais'].map(t=>(
              <span key={t} className="bdg bdgp" style={{fontSize:10}}>{t}</span>
            ))}
          </div>
        </footer>
      )}
    </div>
  );
}
