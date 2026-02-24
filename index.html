<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TranPolSim — Transit Policy Simulator</title>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,400;9..144,600;9..144,700&family=DM+Sans:opsz,wght@9..40,400;9..40,500;9..40,600;9..40,700&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --cream:#f6f3ec;--white:#fff;--ink:#1a1710;--ink2:#504d44;--ink3:#96928a;
  --line:#e6e2d6;--line2:#ccc8b8;
  --green:#1a7a3e;--green-bg:#edf8f2;--amber:#a85e00;--amber-bg:#fdf4e3;
  --red:#b02820;--red-bg:#fdf0ee;--blue:#155090;--blue-bg:#edf2fb;
  --eu:#003399;--eu-gold:#ffcc00;
  --r:14px;
  --sh:0 2px 12px rgba(0,0,0,.07),0 0 0 1px rgba(0,0,0,.04);
  --sh2:0 8px 28px rgba(0,0,0,.13),0 0 0 1px rgba(0,0,0,.05);
}
body{font-family:'DM Sans',sans-serif;background:var(--cream);color:var(--ink);min-height:100vh}
h1,h2,h3,h4{font-family:'Fraunces',serif;font-weight:600}
::-webkit-scrollbar{width:5px;height:5px}::-webkit-scrollbar-thumb{background:var(--line2);border-radius:3px}
.hdr{background:linear-gradient(135deg,#0a1628 0%,#0d2045 60%,#0f2a5a 100%);color:#fff;position:sticky;top:0;z-index:200;box-shadow:0 2px 20px rgba(0,0,0,.4)}
.hdr-top{display:flex;align-items:center;justify-content:space-between;padding:0 24px;height:52px;border-bottom:1px solid rgba(255,255,255,.07)}
.hdr-bottom{display:flex;align-items:center;justify-content:center;padding:0 24px;height:38px;background:rgba(0,0,0,.25);border-bottom:2px solid rgba(255,204,0,.4);gap:4px}
.hdr-logo{display:flex;align-items:center;gap:12px}
.brand-mark{display:flex;align-items:center;gap:0;background:linear-gradient(135deg,#ffcc00 0%,#ffaa00 100%);border-radius:7px;padding:4px 10px;box-shadow:0 2px 8px rgba(255,170,0,.35)}
.brand-mark .bm-tran{font-family:"Fraunces",serif;font-size:18px;font-weight:700;color:#0a1628;letter-spacing:-.5px}
.brand-mark .bm-pol{font-family:"Fraunces",serif;font-size:18px;font-weight:700;color:#0a1628;letter-spacing:-.5px;opacity:.7}
.brand-mark .bm-sim{font-family:"DM Sans",sans-serif;font-size:10px;font-weight:800;color:#0a1628;letter-spacing:.8px;margin-left:2px;opacity:.5;align-self:flex-end;padding-bottom:2px}
.brand-divider{width:1px;height:28px;background:rgba(255,255,255,.15);margin:0 4px}
.brand-text h1{font-family:"Fraunces",serif;font-size:15px;font-weight:600;color:#fff;letter-spacing:-.2px;line-height:1.15}
.brand-text p{font-size:9px;color:rgba(255,204,0,.6);margin-top:2px;letter-spacing:.5px;text-transform:uppercase;font-weight:600}
.hdr-steps{display:flex;align-items:center}
.hdr-step{display:flex;align-items:center;gap:6px;padding:4px 11px;border-radius:6px;cursor:pointer;transition:all .2s;font-size:11px;font-weight:500;color:rgba(255,255,255,.5)}
.hdr-step.done{color:rgba(255,255,255,.7)}.hdr-step.done:hover{background:rgba(255,255,255,.1)}
.hdr-step.active{background:rgba(255,204,0,.18);color:#ffdd55;border:1px solid rgba(255,204,0,.3)}
.hdr-step-num{width:18px;height:18px;border-radius:50%;background:rgba(255,255,255,.15);display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:700;flex-shrink:0}
.hdr-step.done .hdr-step-num{background:var(--eu-gold);color:#0a1628}
.hdr-step.active .hdr-step-num{background:#ffdd55;color:#0a1628}
.hdr-sep{color:rgba(255,255,255,.2);font-size:11px;padding:0 1px}
.hdr-pop{text-align:right}
.hdr-pop .num{font-family:'Fraunces',serif;font-size:18px;font-weight:700;color:var(--eu-gold);line-height:1}
.hdr-pop .lbl{font-size:9px;color:rgba(255,255,255,.4);letter-spacing:.5px;text-transform:uppercase}
.btn{padding:9px 18px;border-radius:8px;border:none;font-family:'DM Sans',sans-serif;font-size:13px;font-weight:600;cursor:pointer;transition:all .18s;display:inline-flex;align-items:center;gap:6px}
.btn-dark{background:var(--ink);color:#fff}.btn-dark:hover{background:#2d2a20;box-shadow:0 4px 14px rgba(0,0,0,.18)}
.btn-eu{background:var(--eu);color:#fff;border-bottom:2px solid var(--eu-gold)}.btn-eu:hover{background:#002280}
.btn-light{background:var(--white);color:var(--ink2);border:1.5px solid var(--line2)}.btn-light:hover{border-color:var(--ink3)}
.btn-green{background:var(--green);color:#fff}.btn-green:hover{background:#136030}
.btn-sm{padding:6px 12px;font-size:11px;border-radius:7px}
.btn-outline{background:transparent;border:1.5px solid var(--line2);color:var(--ink2)}.btn-outline:hover{border-color:var(--ink3);background:var(--white)}
.page{max-width:1160px;margin:0 auto;padding:32px 28px 60px}
.step-section{display:none;animation:fadeUp .32s ease}.step-section.active{display:block}
@keyframes fadeUp{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}
.step-head{margin-bottom:28px}
.step-head h2{font-size:26px;letter-spacing:-.4px;margin-bottom:5px}
.step-head p{font-size:14px;color:var(--ink2);line-height:1.6;max-width:680px}
.nav-row{display:flex;gap:10px;align-items:center;margin-top:28px;padding-top:20px;border-top:1px solid var(--line)}
.city-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:11px;margin-bottom:20px}
.city-card{background:var(--white);border:2px solid var(--line);border-radius:var(--r);padding:14px 12px;cursor:pointer;transition:all .2s;text-align:center;position:relative;overflow:hidden}
.city-card:hover{border-color:var(--line2);box-shadow:var(--sh);transform:translateY(-2px)}
.city-card.sel{border-color:var(--eu);background:var(--eu);color:#fff}
.city-card.sel .c-pop{color:var(--eu-gold)}.city-card.sel .c-ex{color:rgba(255,255,255,.45)}
.city-card.sel .c-terrain{background:rgba(255,255,255,.15);color:rgba(255,255,255,.85)}
.c-icon{font-size:26px;margin-bottom:5px}.c-name{font-family:'Fraunces',serif;font-size:15px;margin-bottom:2px}
.c-pop{font-size:18px;font-weight:700;color:var(--ink);margin-bottom:2px}.c-ex{font-size:10px;color:var(--ink3)}
.c-terrain{display:inline-flex;align-items:center;gap:4px;padding:2px 8px;border-radius:10px;font-size:9px;font-weight:700;letter-spacing:.3px;margin-top:5px;background:var(--cream);color:var(--ink2)}
/* terrain selector */
.terrain-panel{background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:14px 16px;margin-bottom:14px;box-shadow:var(--sh)}
.terrain-panel h4{font-size:13px;margin-bottom:10px;display:flex;align-items:center;gap:7px}
.terrain-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:7px}
.t-card{background:var(--cream);border:2px solid var(--line);border-radius:10px;padding:10px 8px;cursor:pointer;text-align:center;transition:all .18s}
.t-card:hover{border-color:var(--line2);transform:translateY(-1px)}.t-card.sel{border-color:var(--eu);background:var(--blue-bg)}
.t-icon{font-size:22px;margin-bottom:4px}.t-name{font-size:10px;font-weight:700;margin-bottom:2px}
.t-cost{font-size:9px;color:var(--ink3)}.t-card.sel .t-cost{color:var(--blue)}
.terrain-badge{display:flex;align-items:center;gap:8px;padding:8px 12px;border-radius:8px;font-size:11px;margin-top:8px}
/* micro suburb cards */
.sub-card-micro{background:var(--white);border:1.5px solid var(--line);border-radius:9px;padding:8px 10px;cursor:pointer;transition:all .15s;display:flex;align-items:center;gap:8px;font-size:11px}
.sub-card-micro:hover{border-color:var(--line2);box-shadow:var(--sh)}.sub-card-micro.sel{border-color:var(--blue);background:var(--blue-bg)}
.sub-card-micro .sub-check{width:15px;height:15px;border-radius:4px;border:1.5px solid var(--line2);display:flex;align-items:center;justify-content:center;font-size:8px;flex-shrink:0}
.sub-card-micro.sel .sub-check{background:var(--blue);border-color:var(--blue);color:#fff}
.smico-icon{font-size:16px;flex-shrink:0}
.smico-name{font-weight:600;font-size:11px;line-height:1.3}
.smico-meta{font-size:9px;color:var(--ink3);margin-top:1px}
.smico-badge{display:inline-block;padding:1px 5px;border-radius:5px;font-size:8px;font-weight:700;margin-top:2px}
.suburb-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:7px}
.city-note{background:var(--amber-bg);border:1px solid #f0d080;border-radius:10px;padding:12px 16px;font-size:13px;color:var(--amber);margin-bottom:18px;display:none}
.pop-banner{background:var(--eu);border-bottom:2px solid var(--eu-gold);border-radius:var(--r);padding:20px 24px;display:flex;align-items:center;gap:20px;margin-bottom:20px}
.pb-block{flex:1}.pb-lbl{font-size:9px;font-weight:700;letter-spacing:1.5px;text-transform:uppercase;color:rgba(255,255,255,.4);margin-bottom:4px}
.pb-num{font-family:'Fraunces',serif;font-size:32px;font-weight:700;line-height:1;color:#fff}
.pb-sub{font-size:11px;color:rgba(255,255,255,.45);margin-top:2px}
.pb-div{width:1px;background:rgba(255,255,255,.12);align-self:stretch}
.pb-plus{font-size:20px;color:rgba(255,255,255,.25)}.pb-total .pb-num{color:var(--eu-gold);font-size:26px}
.suburb-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:8px}
.sub-card{background:var(--white);border:2px solid var(--line);border-radius:11px;padding:10px 12px;cursor:pointer;transition:all .2s;display:flex;align-items:flex-start;gap:9px}
.sub-card:hover{border-color:var(--line2);box-shadow:var(--sh);transform:translateY(-1px)}.sub-card.sel{border-color:var(--blue);background:var(--blue-bg)}
.sub-check{width:17px;height:17px;border-radius:4px;border:2px solid var(--line2);display:flex;align-items:center;justify-content:center;font-size:9px;flex-shrink:0;margin-top:2px}
.sub-card.sel .sub-check{background:var(--blue);border-color:var(--blue);color:#fff}
.sub-icon{font-size:18px;flex-shrink:0;margin-top:1px}.sub-name{font-size:12px;font-weight:700;line-height:1.3}
.sub-meta{font-size:10px;color:var(--ink3);margin-top:2px}
.sub-type{display:inline-block;padding:1px 6px;border-radius:7px;font-size:8px;font-weight:700;text-transform:uppercase;letter-spacing:.3px;margin-top:3px}
.sub-filter{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:10px}
.sub-filt-btn{padding:4px 10px;border:1.5px solid var(--line2);border-radius:20px;font-size:10px;font-weight:600;cursor:pointer;background:var(--white);color:var(--ink2);transition:all .15s;font-family:"DM Sans",sans-serif}
.sub-filt-btn:hover{border-color:var(--ink3)}.sub-filt-btn.active{background:var(--ink);color:#fff;border-color:var(--ink)}
/* terrain selector */
.terrain-section{margin-bottom:14px}
.terrain-section h4{font-size:12px;font-weight:700;color:var(--ink3);text-transform:uppercase;letter-spacing:.8px;margin-bottom:8px;display:flex;align-items:center;gap:6px}
.terrain-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:7px;margin-bottom:8px}
.t-card{background:var(--white);border:2px solid var(--line);border-radius:10px;padding:10px 6px;cursor:pointer;text-align:center;transition:all .18s}
.t-card:hover{border-color:var(--line2);box-shadow:var(--sh);transform:translateY(-1px)}.t-card.sel{border-width:2.5px}
.t-icon{font-size:20px;margin-bottom:4px}.t-name{font-size:10px;font-weight:700;margin-bottom:2px}
.t-cost{font-size:9px;color:var(--ink3);line-height:1.3}.t-card.sel .t-cost{font-weight:600}
.terrain-info{border-radius:9px;padding:9px 13px;font-size:11px;line-height:1.5;display:flex;gap:8px;align-items:flex-start}
.terrain-info .ti-ico{font-size:18px;flex-shrink:0}
.mode-selector{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;margin-bottom:22px}
.mode-pick{background:var(--white);border:2px solid var(--line);border-radius:var(--r);padding:12px 12px;cursor:pointer;transition:all .2s;text-align:left;display:flex;flex-direction:column;gap:3px}
.mode-pick:hover{border-color:var(--line2);box-shadow:var(--sh);transform:translateY(-2px)}.mode-pick.sel{border-width:2.5px}
.mp-top{display:flex;align-items:center;gap:8px;margin-bottom:1px}
.mp-icon{font-size:20px;flex-shrink:0}.mp-name{font-size:12px;font-weight:700;line-height:1.3;flex:1}
.mp-cat{font-size:8px;font-weight:700;letter-spacing:.5px;text-transform:uppercase;padding:1px 6px;border-radius:4px;align-self:flex-start;margin-bottom:2px}
.mp-desc{font-size:9.5px;color:var(--ink3);line-height:1.45;flex:1;margin-bottom:3px}
.mp-bottom{display:flex;align-items:center;justify-content:space-between}
.mp-fit{font-size:15px;font-weight:700}.mp-badge{display:inline-block;padding:2px 7px;border-radius:9px;font-size:9px;font-weight:700;margin-top:3px}
.rec-compare{background:var(--white);border:1px solid var(--line);border-radius:var(--r);overflow:hidden;box-shadow:var(--sh);margin-bottom:22px}
.rec-compare table{width:100%;border-collapse:collapse;font-size:12px}
.rec-compare th{padding:9px 13px;text-align:left;font-size:9px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--ink3);background:var(--cream);border-bottom:1px solid var(--line)}
.rec-compare th.r{text-align:right}.rec-compare td{padding:11px 13px;border-bottom:1px solid var(--line)}
.rec-compare td.r{text-align:right;font-weight:600}.rec-compare tr:last-child td{border-bottom:none}
.rec-compare tr:hover td{background:var(--cream)}
.mode-cell{display:flex;align-items:center;gap:7px;font-weight:600}
.mdot{width:9px;height:9px;border-radius:50%;flex-shrink:0}
.tbadge{padding:2px 7px;border-radius:7px;font-size:9px;font-weight:700;white-space:nowrap}
.tb-best{background:#fef3c7;color:#8a3c00}.tb-good{background:var(--green-bg);color:var(--green)}
.tb-ok{background:var(--blue-bg);color:var(--blue)}.tb-no{background:var(--line);color:var(--ink3)}
.best-v{color:var(--green);font-weight:700}
.sim-layout{display:grid;grid-template-columns:320px 1fr;gap:18px;align-items:start}
.sim-controls{background:var(--white);border:1px solid var(--line);border-radius:var(--r);box-shadow:var(--sh);overflow:hidden;position:sticky;top:74px}
.sc-header{padding:14px 16px;border-bottom:1px solid var(--line);background:var(--cream)}
.sc-header h3{font-size:14px;margin-bottom:1px}.sc-header p{font-size:10px;color:var(--ink3)}
.sc-body{padding:14px 16px;display:flex;flex-direction:column;gap:11px;max-height:calc(100vh - 220px);overflow-y:auto}
.ctrl-sec-hd{font-size:9px;font-weight:700;letter-spacing:1.2px;text-transform:uppercase;color:var(--ink3);padding:8px 0 5px;border-bottom:1px solid var(--line);margin-bottom:-2px}
.ctrl-top{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:5px}
.ctrl-name{font-size:11px;font-weight:600;color:var(--ink)}.ctrl-val{font-size:15px;font-weight:700;color:var(--ink);text-align:right;line-height:1}
.ctrl-hint{font-size:9px;color:var(--ink3);margin-top:1px}
input[type=range]{-webkit-appearance:none;width:100%;height:4px;background:var(--line);border-radius:2px;outline:none;cursor:pointer}
input[type=range]::-webkit-slider-thumb{-webkit-appearance:none;width:15px;height:15px;background:var(--ink);border-radius:50%;cursor:pointer;box-shadow:0 1px 4px rgba(0,0,0,.2);transition:transform .12s}
input[type=range]::-webkit-slider-thumb:hover{transform:scale(1.2)}
.ctrl-ends{display:flex;justify-content:space-between;font-size:9px;color:var(--ink3);margin-top:2px}
.sc-select select{width:100%;padding:7px 10px;background:var(--cream);border:1.5px solid var(--line);border-radius:7px;font-family:'DM Sans',sans-serif;font-size:11px;color:var(--ink);outline:none;cursor:pointer;appearance:none;background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='10' height='6'%3E%3Cpath d='M1 1l4 4 4-4' stroke='%2396928a' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");background-repeat:no-repeat;background-position:right 9px center}
.sc-select .ctrl-name{margin-bottom:5px;display:block}
.toggle-row{display:flex;gap:6px}
.tog-opt{flex:1;padding:7px 6px;border-radius:8px;border:1.5px solid var(--line);background:var(--cream);text-align:center;cursor:pointer;transition:all .15s;font-size:11px;font-weight:600;color:var(--ink2)}
.tog-opt:hover{border-color:var(--ink3)}.tog-opt.active{border-color:var(--eu);background:var(--eu);color:#fff}
.tog-icon{font-size:16px;display:block;margin-bottom:2px}
.eu-fund-bar{background:linear-gradient(90deg,var(--eu) 0%,#1a40b8 100%);border-radius:9px;padding:11px 13px;display:flex;gap:11px;align-items:center}
.eu-fund-stars{font-size:14px;letter-spacing:-2px;flex-shrink:0;color:var(--eu-gold)}
.eu-fund-body{flex:1}.eu-fund-title{font-size:11px;font-weight:700;color:var(--eu-gold);margin-bottom:1px}
.eu-fund-desc{font-size:9px;color:rgba(255,255,255,.6);line-height:1.4}
.eu-fund-pct{font-family:'Fraunces',serif;font-size:20px;font-weight:700;color:var(--eu-gold);flex-shrink:0}
.sim-results{display:flex;flex-direction:column;gap:15px}
.verdict{border-radius:var(--r);padding:14px 18px;display:flex;align-items:flex-start;gap:12px;border:1.5px solid}
.verdict.good{background:var(--green-bg);border-color:#8ed4aa}.verdict.warn{background:var(--amber-bg);border-color:#f0d080}.verdict.bad{background:var(--red-bg);border-color:#efb0a8}
.v-icon{font-size:22px;flex-shrink:0;margin-top:1px}.v-title{font-size:15px;font-weight:700;margin-bottom:2px}
.verdict.good .v-title{color:var(--green)}.verdict.warn .v-title{color:var(--amber)}.verdict.bad .v-title{color:var(--red)}
.v-desc{font-size:12px;color:var(--ink2);line-height:1.5}
.kpi-row{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
.kpi{background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:13px;box-shadow:var(--sh)}
.kpi-icon{font-size:15px;margin-bottom:6px}.kpi-lbl{font-size:9px;color:var(--ink3);font-weight:600;letter-spacing:.5px;margin-bottom:3px;text-transform:uppercase}
.kpi-val{font-size:21px;font-weight:700;line-height:1}.kpi-sub{font-size:10px;color:var(--ink3);margin-top:3px}
.cv-blue{color:var(--blue)}.cv-green{color:var(--green)}.cv-amber{color:var(--amber)}.cv-red{color:var(--red)}.cv-eu{color:var(--eu)}
.chart-card{background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:17px;box-shadow:var(--sh)}
.cc-title{font-family:'Fraunces',serif;font-size:15px;margin-bottom:2px}.cc-sub{font-size:10px;color:var(--ink3);margin-bottom:12px}
canvas{display:block;width:100%!important}.charts-2{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.cap-warn{background:#fff7ee;border:1.5px solid #f5c880;border-radius:10px;padding:11px 14px;font-size:12px;color:var(--amber);display:none;align-items:flex-start;gap:9px}
.cap-warn.show{display:flex}
.eu-breakdown{background:linear-gradient(135deg,#001f80,#003399);border-radius:var(--r);padding:16px 18px;color:#fff}
.eu-breakdown h4{font-size:13px;color:var(--eu-gold);margin-bottom:10px;display:flex;align-items:center;gap:7px}
.eu-fund-row{display:flex;align-items:center;gap:9px;margin-bottom:7px}
.eu-fund-name{font-size:11px;color:rgba(255,255,255,.75);width:165px;flex-shrink:0}
.eu-fund-track{flex:1;height:14px;background:rgba(255,255,255,.12);border-radius:7px;overflow:hidden}
.eu-fund-fill{height:100%;border-radius:7px;display:flex;align-items:center;padding-left:5px;font-size:9px;font-weight:700;color:rgba(0,0,60,.8)}
.eu-fund-val{font-size:11px;font-weight:700;color:var(--eu-gold);width:64px;text-align:right;flex-shrink:0}
.gantt-rows{display:flex;flex-direction:column;gap:5px;padding:3px 0}
.g-row{display:flex;align-items:center;gap:9px}
.g-lbl{width:134px;font-size:10px;color:var(--ink2);text-align:right;flex-shrink:0}
.g-track{flex:1;height:22px;background:var(--cream);border-radius:5px;position:relative;overflow:hidden}
.g-bar{position:absolute;top:0;height:100%;border-radius:5px;display:flex;align-items:center;padding:0 7px}
.g-bar span{font-size:9px;font-weight:600;color:rgba(255,255,255,.9);white-space:nowrap;overflow:hidden}
.g-dur{width:38px;font-size:10px;color:var(--ink3);text-align:right;flex-shrink:0}
.g-axis{display:flex;padding:2px 0 0 143px}.g-ticks{flex:1;display:flex;justify-content:space-between;font-size:9px;color:var(--ink3)}
.impact-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:9px}
.impact-item{background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:13px;display:flex;gap:9px;align-items:flex-start;box-shadow:var(--sh)}
.imp-ico{font-size:19px;flex-shrink:0}.imp-lbl{font-size:9px;color:var(--ink3);text-transform:uppercase;letter-spacing:.5px;margin-bottom:2px}
.imp-val{font-size:17px;font-weight:700}.imp-note{font-size:10px;color:var(--ink3);margin-top:2px;line-height:1.4}
.network-scheme{background:var(--white);border:1px solid var(--line);border-radius:var(--r);box-shadow:var(--sh);overflow:hidden}
.ns-header{background:var(--ink);padding:13px 17px;display:flex;align-items:center;justify-content:space-between;gap:12px}
.ns-header h4{color:#fff;font-size:14px}.ns-header p{color:rgba(255,255,255,.5);font-size:10px;margin-top:1px}
.ns-legend{padding:11px 17px;border-top:1px solid var(--line);display:flex;gap:14px;flex-wrap:wrap;background:var(--cream)}
.ns-leg-item{display:flex;align-items:center;gap:6px;font-size:11px;color:var(--ink2)}
.ns-leg-swatch{width:22px;height:6px;border-radius:3px;flex-shrink:0}
.ns-tool{padding:5px 10px;border:1.5px solid var(--line2);background:var(--white);border-radius:6px;font-family:"DM Sans",sans-serif;font-size:11px;font-weight:600;cursor:pointer;color:var(--ink2);transition:all .15s}
.ns-tool:hover{border-color:var(--ink3);background:var(--cream);color:var(--ink)}
.ns-tool.active{background:var(--ink);color:#fff;border-color:var(--ink)}
.sc-bar{background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:12px 15px;display:flex;align-items:center;gap:10px;flex-wrap:wrap;box-shadow:var(--sh)}
.sc-bar-lbl{font-size:11px;color:var(--ink3);font-weight:600;flex-shrink:0}
.sc-chips{display:flex;gap:7px;flex:1;flex-wrap:wrap;align-items:center}
.sc-chip{display:flex;align-items:center;gap:5px;padding:4px 11px;border-radius:20px;border:1.5px solid var(--line2);font-size:11px;font-weight:500;color:var(--ink2);cursor:pointer;transition:all .15s;background:var(--cream)}
.sc-chip:hover{border-color:var(--ink3)}.sc-chip.cur{background:var(--ink);color:#fff;border-color:var(--ink)}
.sc-chip-dot{width:7px;height:7px;border-radius:50%;flex-shrink:0}
.sc-del{opacity:.5;margin-left:2px;cursor:pointer;font-size:13px}.sc-del:hover{opacity:1}
.sc-save-row{display:flex;gap:6px;align-items:center;flex-shrink:0}
.sc-input{padding:6px 11px;border:1.5px solid var(--line2);border-radius:7px;font-family:'DM Sans',sans-serif;font-size:11px;color:var(--ink);background:var(--cream);outline:none;width:140px}
.sc-input:focus{border-color:var(--ink2);background:var(--white)}.sc-input::placeholder{color:var(--ink3)}
.cmp-panel{background:var(--white);border:1px solid var(--line);border-radius:var(--r);box-shadow:var(--sh);overflow:hidden}
.cmp-panel table{width:100%;border-collapse:collapse;font-size:11px}
.cmp-panel th{padding:8px 12px;text-align:left;font-size:9px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--ink3);background:var(--cream);border-bottom:1px solid var(--line)}
.cmp-panel th.r{text-align:right}.cmp-panel td{padding:9px 12px;border-bottom:1px solid var(--line)}
.cmp-panel td.r{text-align:right;font-weight:600}.cmp-panel tr:last-child td{border-bottom:none}
.cmp-panel tr:hover td{background:var(--cream)}
.sec-lbl{font-size:10px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--ink3);display:flex;align-items:center;gap:9px;margin-bottom:10px}
.sec-lbl::after{content:'';flex:1;height:1px;background:var(--line)}
.footnote{font-size:10px;color:var(--ink3);line-height:1.7;margin-top:6px}

/* ── fictional city map ── */
.city-map-wrap{position:relative;overflow:hidden;border-radius:var(--r);border:1px solid var(--line);background:#d4e8c2;margin-bottom:0}
#c-citymap{display:block;width:100%!important}
/* ── suburb scope toggle ── */
.scope-toggle{display:flex;gap:0;border:1.5px solid var(--line2);border-radius:8px;overflow:hidden;margin-bottom:0}
.scope-btn{flex:1;padding:6px 0;text-align:center;font-size:10px;font-weight:700;background:var(--white);color:var(--ink2);cursor:pointer;border:none;font-family:"DM Sans",sans-serif;transition:all .15s}
.scope-btn.active{background:var(--ink);color:#fff}
/* ── sequential progress bar ── */
.seq-progress{display:flex;align-items:stretch;gap:0;border-radius:8px;overflow:hidden;border:1px solid var(--line);margin-bottom:8px}
.seq-phase{flex:1;padding:9px 12px;background:var(--cream);cursor:pointer;transition:all .18s;position:relative;text-align:center;border-right:1px solid var(--line)}
.seq-phase:last-child{border-right:none}
.seq-phase.done{background:var(--green);color:#fff}
.seq-phase.active{background:var(--blue);color:#fff}
.seq-phase.planned{background:var(--cream);color:var(--ink3)}
.seq-phase .sp-label{font-size:10px;font-weight:700;display:block}
.seq-phase .sp-sub{font-size:9px;opacity:.7;display:block;margin-top:1px}
.seq-phase .sp-check{position:absolute;top:4px;right:6px;font-size:12px}
/* ── add-line panel ── */
.add-line-btn{display:flex;align-items:center;gap:6px;padding:7px 12px;border:2px dashed var(--line2);border-radius:8px;background:none;cursor:pointer;font-family:"DM Sans",sans-serif;font-size:11px;font-weight:600;color:var(--ink3);width:100%;transition:all .15s}
.add-line-btn:hover{border-color:var(--blue);color:var(--blue);background:var(--blue-bg)}
/* decision tree */
.dt-panel{background:var(--white);border:1.5px solid var(--line);border-radius:var(--r);padding:18px;box-shadow:var(--sh);margin-bottom:16px}
.dt-winner{background:linear-gradient(135deg,#f0faf4 0%,#e8f5ff 100%);border:2px solid #8ed4aa;border-radius:var(--r);padding:16px 18px;margin-bottom:14px;display:flex;gap:14px;align-items:flex-start}
.dt-winner-crown{font-size:32px;flex-shrink:0;line-height:1}
.dt-winner-body{flex:1;min-width:0}
.dt-winner-title{font-family:"Fraunces",serif;font-size:18px;font-weight:700;color:#1a7a3e;margin-bottom:2px}
.dt-winner-sub{font-size:11px;color:#504d44;line-height:1.5;margin-bottom:8px}
.dt-score-bar{display:flex;gap:0;border-radius:8px;overflow:hidden;height:22px;margin-bottom:8px}
.dt-score-seg{display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:700;color:#fff;transition:width .4s}
.dt-criteria{display:grid;grid-template-columns:repeat(4,1fr);gap:6px;margin-top:8px}
.dt-crit{background:rgba(0,0,0,.04);border-radius:7px;padding:6px 8px;text-align:center}
.dt-crit-val{font-size:13px;font-weight:700;margin-bottom:1px}
.dt-crit-lbl{font-size:8px;color:var(--ink3);text-transform:uppercase;letter-spacing:.4px}
.dt-tree{display:flex;flex-direction:column;gap:8px;margin-bottom:12px}
.dt-node{border:1.5px solid var(--line);border-radius:9px;overflow:hidden}
.dt-node-q{background:#f8f6f0;padding:8px 12px;font-size:11px;font-weight:700;display:flex;align-items:center;gap:6px}
.dt-node-ans{padding:6px 12px 8px;display:flex;flex-direction:column;gap:4px}
.dt-ans-row{display:flex;align-items:center;gap:7px;font-size:11px}
.dt-ans-dot{width:10px;height:10px;border-radius:50%;flex-shrink:0}
.dt-rank-table{width:100%;border-collapse:collapse;font-size:11px}
.dt-rank-table th{text-align:left;font-size:10px;color:var(--ink3);font-weight:600;padding:4px 8px;border-bottom:1px solid var(--line)}
.dt-rank-table td{padding:5px 8px;border-bottom:1px solid var(--line2)}
.dt-rank-table tr:last-child td{border-bottom:none}
.dt-rank-table tr.winner-row td{background:#f0faf4;font-weight:700}
.dt-score-pill{display:inline-flex;align-items:center;justify-content:center;width:30px;height:18px;border-radius:6px;font-size:9px;font-weight:700;color:#fff}
/* risk panel */
.risk-item{display:flex;gap:11px;padding:10px 13px;border-radius:10px;border:1.5px solid var(--line);background:var(--white);align-items:flex-start}
.risk-item.hi{border-color:#f5c0c0;background:#fff5f5}
.risk-item.med{border-color:#f5dfa0;background:#fffaee}
.risk-item.lo{border-color:#c0dfc8;background:#f4fbf6}
.risk-lvl{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:16px;flex-shrink:0}
.risk-item.hi .risk-lvl{background:#f5c0c055}
.risk-item.med .risk-lvl{background:#f5dfa055}
.risk-item.lo .risk-lvl{background:#c0dfc855}
.risk-title{font-size:12px;font-weight:700;margin-bottom:2px}
.risk-item.hi .risk-title{color:#b02020}
.risk-item.med .risk-title{color:#8a5800}
.risk-item.lo .risk-title{color:#1a6030}
.risk-desc{font-size:11px;color:var(--ink2);line-height:1.5}
.risk-mitigation{font-size:10px;margin-top:4px;padding:4px 8px;border-radius:6px;background:rgba(0,0,0,.04);color:var(--ink3)}
.risk-mitigation strong{color:var(--ink2)}
.risk-badges{display:flex;gap:5px;margin-top:5px;flex-wrap:wrap}
.risk-badge{padding:2px 7px;border-radius:8px;font-size:9px;font-weight:700}
.risk-matrix-grid{display:grid;grid-template-columns:repeat(5,1fr);gap:3px;margin-bottom:6px}
.rmg-cell{border-radius:4px;height:18px;display:flex;align-items:center;justify-content:center;font-size:8px;font-weight:700}
#toast{position:fixed;bottom:22px;left:50%;transform:translateX(-50%) translateY(20px);background:var(--ink);color:#fff;padding:9px 18px;border-radius:18px;font-size:12px;font-weight:500;opacity:0;transition:all .25s;z-index:999;white-space:nowrap;pointer-events:none;box-shadow:0 4px 18px rgba(0,0,0,.22)}
/* chart tooltip */
.chart-wrap{position:relative}
.ch-tip{position:absolute;pointer-events:none;display:none;background:rgba(26,23,16,.92);color:#fff;font-size:11px;font-weight:500;padding:6px 10px;border-radius:7px;white-space:nowrap;box-shadow:0 4px 14px rgba(0,0,0,.22);z-index:50;transform:translate(-50%,-100%);margin-top:-8px}
.ch-tip::after{content:'';position:absolute;left:50%;bottom:-5px;transform:translateX(-50%);border:5px solid transparent;border-bottom:none;border-top-color:rgba(26,23,16,.92)}
/* plain-language summary */
.plain-card{background:linear-gradient(135deg,#1a1710 0%,#2d2a20 100%);border-radius:var(--r);padding:20px 22px;color:#fff;margin-bottom:4px}
.plain-card h3{font-size:17px;color:var(--eu-gold);margin-bottom:12px;display:flex;align-items:center;gap:8px}
.plain-bullets{display:flex;flex-direction:column;gap:7px}
.plain-bullet{display:flex;align-items:flex-start;gap:10px;font-size:13px;line-height:1.5;color:rgba(255,255,255,.85)}
.plain-bullet .pb-ico{font-size:18px;flex-shrink:0;margin-top:1px}
.plain-bullet strong{color:#fff}
/* network line manager */
.nl-manager{background:var(--white);border:1px solid var(--line);border-radius:var(--r);overflow:hidden;margin-bottom:12px}
.nl-header{background:var(--cream);padding:10px 14px;border-bottom:1px solid var(--line);display:flex;align-items:center;justify-content:space-between}
.nl-header h4{font-size:13px}.nl-header p{font-size:10px;color:var(--ink3);margin-top:1px}
.nl-lines{padding:10px 14px;display:flex;flex-direction:column;gap:7px}
.nl-row{display:flex;align-items:center;gap:8px;padding:8px 10px;border-radius:9px;border:1.5px solid var(--line);background:var(--cream);transition:border-color .15s}
.nl-row:hover{border-color:var(--line2)}
.nl-swatch{width:16px;height:16px;border-radius:4px;flex-shrink:0}
.nl-name{font-size:12px;font-weight:600;flex:1}
.nl-status{font-size:10px;color:var(--ink3);margin-left:4px}
.nl-row select,.nl-row input[type=text]{font-family:'DM Sans',sans-serif;font-size:11px;border:1.5px solid var(--line2);border-radius:6px;padding:3px 7px;background:var(--white);color:var(--ink);outline:none}
.nl-row input[type=text]{width:110px}
.nl-row select:focus,.nl-row input:focus{border-color:var(--ink3)}
.nl-btn{padding:4px 9px;border:1.5px solid var(--line2);background:var(--white);border-radius:6px;font-size:10px;font-weight:600;cursor:pointer;font-family:'DM Sans',sans-serif;color:var(--ink2);white-space:nowrap}
.nl-btn:hover{border-color:var(--ink3);color:var(--ink)}
.nl-btn.danger{color:var(--red)}.nl-btn.danger:hover{border-color:var(--red);background:var(--red-bg)}
/* extra simulation levers */
.lever-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px}
.lever-sm .ctrl-val{font-size:13px}
/* milestone ribbon */
.milestones{display:flex;gap:0;margin-bottom:4px;border-radius:9px;overflow:hidden;border:1px solid var(--line)}
.ms-item{flex:1;text-align:center;padding:8px 4px;background:var(--cream);border-right:1px solid var(--line);font-size:10px}
.ms-item:last-child{border-right:none}
.ms-yr{font-size:16px;font-weight:700;font-family:'Fraunces',serif;color:var(--eu);display:block}
.ms-lbl{color:var(--ink3);font-size:9px;letter-spacing:.3px}
/* extra kpi row */
.kpi-mini{background:var(--white);border:1px solid var(--line);border-radius:11px;padding:10px 12px;box-shadow:var(--sh)}
.kpi-mini .kpi-lbl{font-size:9px;color:var(--ink3);text-transform:uppercase;letter-spacing:.5px;margin-bottom:2px}
.kpi-mini .kpi-val{font-size:17px;font-weight:700}
.kpi-row-5{display:grid;grid-template-columns:repeat(5,1fr);gap:9px}
</style>
</head>
<body>

<div class="hdr">
  <!-- Top row: brand + population -->
  <div class="hdr-top">
    <div class="hdr-logo">
      <div class="brand-mark">
        <span class="bm-tran">Tran</span><span class="bm-pol">Pol</span><span class="bm-sim">SIM</span>
      </div>
      <div class="brand-divider"></div>
      <div class="brand-text">
        <h1>Transit Policy Simulator</h1>
        <p>EU · Evidence-based · Open policy modelling</p>
      </div>
    </div>
    <div style="display:flex;align-items:center;gap:20px">
      <div style="font-size:9px;color:rgba(255,204,0,.45);text-align:right;letter-spacing:.3px;line-height:1.5">v2.0 · TranPolSim<br><span style="color:rgba(255,255,255,.25)">EU Policy Research Tool</span></div>
      <div class="hdr-pop"><div class="num" id="hdr-pop">—</div><div class="lbl">Metro population</div></div>
    </div>
  </div>
  <!-- Bottom row: step navigation -->
  <div class="hdr-bottom">
    <div class="hdr-steps">
      <div class="hdr-step active" id="hs1" onclick="goStep(1)"><div class="hdr-step-num">1</div> City &amp; Geography</div>
      <div class="hdr-sep">›</div>
      <div class="hdr-step" id="hs2" onclick="goStep(2)"><div class="hdr-step-num">2</div> Suburbs</div>
      <div class="hdr-sep">›</div>
      <div class="hdr-step" id="hs3" onclick="goStep(3)"><div class="hdr-step-num">3</div> Recommend</div>
      <div class="hdr-sep">›</div>
      <div class="hdr-step" id="hs4" onclick="goStep(4)"><div class="hdr-step-num">4</div> Simulate &amp; Design</div>
    </div>
  </div>
</div>

<div class="page">

<!-- STEP 1 -->
<div class="step-section active" id="step1">
  <div class="step-head">
    <h2>Step 1 — City size &amp; geography</h2>
    <p>Select your city's population bracket and its geographic setting. Terrain directly affects construction costs — mountains and coastal zones add tunnels, bridges and specialist engineering.</p>
  </div>
  <div class="city-grid" id="city-grid"></div>
  <div class="city-note" id="city-note"></div>

  <div class="terrain-section" style="margin-top:18px">
    <h4>🗺 Geographic setting &amp; terrain</h4>
    <div class="terrain-grid" id="terrain-grid"></div>
    <div class="terrain-info" id="terrain-info" style="display:none"></div>
  </div>

  <div class="nav-row"><button class="btn btn-eu" onclick="goStep(2)">Next: Add suburbs →</button></div>
</div>

<!-- STEP 2 -->
<div class="step-section" id="step2">
  <div class="step-head">
    <h2>Step 2 — Metropolitan area</h2>
    <p>EU cities are defined by their functional urban areas, not administrative borders. Add surrounding communes and suburban zones — each increases the metropolitan population and shifts which transit solution makes sense.</p>
  </div>
  <div class="pop-banner">
    <div class="pb-block"><div class="pb-lbl">City proper</div><div class="pb-num" id="pb-city">—</div><div class="pb-sub" id="pb-city-name">—</div></div>
    <div class="pb-plus">＋</div>
    <div class="pb-block"><div class="pb-lbl">Suburbs / communes</div><div class="pb-num" id="pb-sub">0</div><div class="pb-sub" id="pb-sub-count">None selected</div></div>
    <div class="pb-div"></div>
    <div class="pb-block pb-total"><div class="pb-lbl">Functional Urban Area</div><div class="pb-num" id="pb-total">—</div><div class="pb-sub">People to serve</div></div>
  </div>
  <div class="sub-filter" id="sub-filter"></div>
  <div class="suburb-grid" id="suburb-grid"></div>
  <div class="nav-row">
    <button class="btn btn-light" onclick="goStep(1)">← Back</button>
    <button class="btn btn-eu" onclick="goStep(3)">See transit recommendations →</button>
  </div>
</div>

<!-- STEP 3 -->
<div class="step-section" id="step3">
  <div class="step-head">
    <h2>Step 3 — Which transit fits your city?</h2>
    <p>For a functional urban area of <strong id="rec-metro-pop">—</strong>, here is how each transit mode compares. Click any row to jump into the policy simulator for that mode.</p>
  </div>
  <div class="mode-selector" id="mode-selector"></div>
  <div class="rec-compare"><table><thead><tr id="rec-thead"></tr></thead><tbody id="rec-tbody"></tbody></table></div>
  <div class="charts-2" style="margin-bottom:20px">
    <div class="chart-card"><div class="cc-title">Fit score by transit type</div><div class="cc-sub">How well each mode matches your city's population</div><canvas id="c-fit" height="190"></canvas></div>
    <div class="chart-card"><div class="cc-title">Cost vs Daily Capacity</div><div class="cc-sub">Investment required versus passengers carried daily</div><canvas id="c-costcap" height="190"></canvas></div>
  </div>
  <div class="nav-row">
    <button class="btn btn-light" onclick="goStep(2)">← Adjust suburbs</button>
    <button class="btn btn-eu" id="btn-simulate" onclick="goStep(4)">Simulate policies →</button>
  </div>
</div>

<!-- STEP 4 -->
<div class="step-section" id="step4">
  <div class="step-head">
    <h2>Step 4 — Policy Simulator &amp; Network Design</h2>
    <p>Adjust policy levers, choose EU funding instruments, and design your network — up to <strong>2 simultaneous lines</strong>. All figures in <strong>Euros (€)</strong>. The network scheme updates in real time.</p>
  </div>

  <div style="background:var(--blue-bg);border:1px solid #c0d4f8;border-radius:var(--r);padding:13px 17px;margin-bottom:16px">
    <div style="font-size:9px;font-weight:700;letter-spacing:1px;text-transform:uppercase;color:var(--blue);margin-bottom:8px">💡 Try these policy questions</div>
    <div style="display:flex;gap:7px;flex-wrap:wrap">
      <button class="btn btn-sm btn-light" onclick="preset('affordable')">Low-fare social policy</button>
      <button class="btn btn-sm btn-light" onclick="preset('eu_max')">Maximum EU co-funding</button>
      <button class="btn btn-sm btn-light" onclick="preset('fast')">Accelerated construction</button>
      <button class="btn btn-sm btn-light" onclick="preset('ambitious')">Ambitious long network</button>
      <button class="btn btn-sm btn-light" onclick="preset('free')">Free public transport</button>
      <button class="btn btn-sm btn-light" onclick="preset('twolines')">2 simultaneous lines</button>
      <button class="btn btn-sm btn-light" onclick="preset('sequential')">Sequential: L1 then L2</button>
    </div>
  </div>

  <div style="margin-bottom:14px;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:9px">
    <div style="display:flex;gap:5px;flex-wrap:wrap" id="sim-mode-tabs"></div>
    <div style="display:flex;gap:7px">
      <button class="btn btn-sm btn-outline" onclick="exportCSV()">⬇ Export CSV</button>
      <button class="btn btn-sm btn-light" onclick="goStep(3)">← Recommendations</button>
    </div>
  </div>

  <div class="sim-layout">
    <!-- LEFT CONTROLS -->
    <div class="sim-controls">
      <div class="sc-header"><h3 id="sc-mode-title">Policy Levers</h3><p>All values recalculate instantly · Costs in €</p></div>
      <div class="sc-body">

        <div id="metro-type-block" style="display:none">
          <div class="ctrl-sec-hd">🚇 Metro construction type</div>
          <div class="toggle-row" id="metro-toggle">
            <div class="tog-opt active" id="mt-ug" onclick="setMetroType('underground')"><span class="tog-icon">⬇️</span>Underground<br><span style="font-size:9px;opacity:.7">+60% cost · all-weather</span></div>
            <div class="tog-opt" id="mt-el" onclick="setMetroType('elevated')"><span class="tog-icon">⬆️</span>Elevated<br><span style="font-size:9px;color:var(--ink3)">Standard cost · viaduct</span></div>
          </div>
        </div>

        <div class="ctrl-sec-hd">🗺️ Network lines</div>
        <!-- Line count — rendered as buttons by renderLineCountButtons() -->
        <div class="ctrl-block" style="padding-bottom:4px">
          <div class="ctrl-top"><div><div class="ctrl-name">Number of lines</div><div class="ctrl-hint" id="line-count-hint">How many routes in the network</div></div><div class="ctrl-val" id="v-lines">1 line</div></div>
          <div id="line-count-btns" style="display:flex;flex-wrap:wrap;gap:5px;margin-top:6px"></div>
          <!-- Hidden input kept for legacy JS compatibility -->
          <input type="hidden" id="s-lines" value="1">
        </div>
        <!-- Build strategy (sequential vs simultaneous) — shown when >1 line -->
        <div id="build-strategy-block" style="display:none;margin-top:4px">
          <div style="font-size:10px;font-weight:700;color:var(--ink3);margin-bottom:5px;text-transform:uppercase;letter-spacing:.4px">Build strategy</div>
          <div style="display:flex;flex-direction:column;gap:5px">
            <div class="tog-opt active" id="bs-sim" onclick="setBuildStrategy('sim')" style="text-align:left;padding:8px 10px;display:flex;align-items:center;gap:8px">
              <span style="font-size:14px;flex-shrink:0">━━</span>
              <div><div style="font-size:11px;font-weight:700">All lines simultaneously</div><div style="font-size:9px;color:var(--ink3)">All open together · higher upfront cost</div></div>
            </div>
            <div class="tog-opt" id="bs-seq" onclick="setBuildStrategy('seq')" style="text-align:left;padding:8px 10px;display:flex;align-items:center;gap:8px">
              <span style="font-size:13px;flex-shrink:0">━→━</span>
              <div><div style="font-size:11px;font-weight:700">Sequential (one at a time)</div><div style="font-size:9px;color:var(--ink3)">Each line opens before next starts</div></div>
            </div>
          </div>
        </div>
        <!-- Line context note -->
        <div id="line-note" style="margin-top:6px;font-size:10px;border-radius:7px;padding:7px 10px;display:none"></div>
        <!-- Mode-aware length guidance -->
        <div id="length-guidance" style="margin-top:6px;font-size:10px;border-radius:7px;padding:8px 10px;background:var(--blue-bg);color:var(--blue);display:none"></div>

        <div class="ctrl-sec-hd">🎟️ Fare policy</div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Ticket price</div><div class="ctrl-hint">Cost per single journey</div></div><div class="ctrl-val" id="v-ticket">€1.20</div></div>
          <input type="range" id="s-ticket" min="0.1" max="5" step="0.05" value="1.2" oninput="upd()">
          <div class="ctrl-ends"><span>Nearly free</span><span>€5.00</span></div>
        </div>
        <div class="sc-select">
          <div class="ctrl-name">Fare structure</div>
          <select id="s-fare" onchange="upd()">
            <option value="flat">Flat — same price everywhere</option>
            <option value="zone" selected>Zone-based — closer = cheaper</option>
            <option value="dist">Distance-based</option>
            <option value="peak">Peak/off-peak differential</option>
            <option value="free">Fully free — tax-funded</option>
          </select>
        </div>

        <div class="ctrl-sec-hd">🏛️ Public funding &amp; EU co-financing</div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Operating subsidy</div><div class="ctrl-hint">National/local share of annual running costs</div></div><div class="ctrl-val" id="v-sub">40%</div></div>
          <input type="range" id="s-sub" min="0" max="90" value="40" oninput="upd()">
          <div class="ctrl-ends"><span>None</span><span>90%</span></div>
        </div>
        <div class="sc-select">
          <div class="ctrl-name">Capital funding model</div>
          <select id="s-fund" onchange="upd()">
            <option value="public">Municipal / national debt</option>
            <option value="ppp" selected>Public-Private Partnership (PPP)</option>
            <option value="cohesion">EU Cohesion Fund (up to 85%)</option>
            <option value="cef">EU Connecting Europe Facility (50%)</option>
            <option value="erdf">EU ERDF + national match (70%)</option>
            <option value="dev">Property value capture</option>
          </select>
        </div>
        <div id="eu-fund-info" style="display:none">
          <div class="eu-fund-bar">
            <div class="eu-fund-stars">★★★</div>
            <div class="eu-fund-body"><div class="eu-fund-title" id="eu-fund-title">EU Fund</div><div class="eu-fund-desc" id="eu-fund-desc"></div></div>
            <div class="eu-fund-pct" id="eu-fund-pct">85%</div>
          </div>
        </div>

        <div class="ctrl-sec-hd">🏗️ Network design</div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Line length (per line)</div><div class="ctrl-hint">km of track per line</div></div><div class="ctrl-val" id="v-length">18 km</div></div>
          <input type="range" id="s-length" min="2" max="60" value="18" oninput="upd()">
          <div class="ctrl-ends"><span id="len-min-lbl">2 km</span><span id="len-max-lbl">60 km</span></div>
        </div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Stops per line</div><div class="ctrl-hint">Number of stations on each line</div></div><div class="ctrl-val" id="v-stations">14</div></div>
          <input type="range" id="s-stations" min="3" max="50" value="14" oninput="upd()">
          <div class="ctrl-ends"><span>3</span><span>50</span></div>
        </div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Service frequency</div><div class="ctrl-hint">Peak hour interval</div></div><div class="ctrl-val" id="v-freq">Every 6 min</div></div>
          <input type="range" id="s-freq" min="2" max="30" value="6" oninput="upd()">
          <div class="ctrl-ends"><span>2 min</span><span>30 min</span></div>
        </div>

        <div class="ctrl-sec-hd">📊 Context assumptions</div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Population growth</div><div class="ctrl-hint">Annual metropolitan growth rate</div></div><div class="ctrl-val" id="v-growth">1.5%/yr</div></div>
          <input type="range" id="s-growth" min="0" max="5" step="0.1" value="1.5" oninput="upd()">
          <div class="ctrl-ends"><span>Shrinking</span><span>5%/yr</span></div>
        </div>
        <div class="ctrl-block">
          <div class="ctrl-top"><div><div class="ctrl-name">Build speed</div><div class="ctrl-hint">Faster = more expensive; slower = cheaper</div></div><div class="ctrl-val" id="v-speed">Standard</div></div>
          <input type="range" id="s-speed" min="1" max="3" step="1" value="2" oninput="upd()">
          <div class="ctrl-ends"><span>Cautious</span><span>Accelerated</span></div>
        </div>
      </div>
    </div>

    <!-- RIGHT RESULTS -->
    <div class="sim-results">

      <!-- PLAIN LANGUAGE SUMMARY -->
      <div class="plain-card">
        <h3>📋 What does this mean in plain language?</h3>
        <div class="plain-bullets" id="plain-bullets">
          <div class="plain-bullet"><span class="pb-ico">⏳</span><span>Run the simulator to see a plain-language summary here.</span></div>
        </div>
      </div>

      <div class="verdict good" id="verdict">
        <div class="v-icon">✅</div>
        <div><div class="v-title" id="v-title">Project looks viable</div><div class="v-desc" id="v-desc">Adjust the levers to explore different policy choices.</div></div>
      </div>
      <div class="cap-warn" id="cap-warn"><span style="font-size:16px;flex-shrink:0">⚠️</span><div>Capacity reached around <strong>Year <span id="cap-yr">22</span></strong>. At current growth rates, a second line or expansion will be needed.</div></div>

      <!-- KEY MILESTONES -->
      <div class="sec-lbl">Key milestones</div>
      <div class="milestones">
        <div class="ms-item"><span class="ms-yr" id="ms-approval">2025</span><span class="ms-lbl">Approval</span></div>
        <div class="ms-item"><span class="ms-yr" id="ms-works">—</span><span class="ms-lbl">Works start</span></div>
        <div class="ms-item"><span class="ms-yr" id="ms-open">—</span><span class="ms-lbl">Opens</span></div>
        <div class="ms-item"><span class="ms-yr" id="ms-be">—</span><span class="ms-lbl">Break-even</span></div>
        <div class="ms-item"><span class="ms-yr" id="ms-mature">—</span><span class="ms-lbl">Full ridership</span></div>
      </div>

      <div class="eu-breakdown" id="eu-breakdown" style="display:none">
        <h4>🇪🇺 EU Co-funding Breakdown</h4>
        <div id="eu-fund-rows"></div>
      </div>

      <div class="sec-lbl">Key figures</div>
      <div class="kpi-row">
        <div class="kpi"><div class="kpi-icon">🏗️</div><div class="kpi-lbl">Total build cost</div><div class="kpi-val cv-blue" id="k-cost">€4.8B</div><div class="kpi-sub" id="k-perkm">€220M/km</div></div>
        <div class="kpi"><div class="kpi-icon">🇪🇺</div><div class="kpi-lbl">EU co-funding</div><div class="kpi-val cv-eu" id="k-eu">€0</div><div class="kpi-sub" id="k-eu-lbl">No EU funds</div></div>
        <div class="kpi"><div class="kpi-icon">🚶</div><div class="kpi-lbl">Daily passengers</div><div class="kpi-val cv-green" id="k-riders">—</div><div class="kpi-sub" id="k-riders-sub">at maturity</div></div>
        <div class="kpi"><div class="kpi-icon">📅</div><div class="kpi-lbl">Years to open</div><div class="kpi-val" id="k-dur">—</div><div class="kpi-sub" id="k-open-yr">Opens ~—</div></div>
      </div>
      <div class="kpi-row">
        <div class="kpi"><div class="kpi-icon">💶</div><div class="kpi-lbl">Fare income / yr</div><div class="kpi-val cv-green" id="k-rev">—</div><div class="kpi-sub">fare box revenue</div></div>
        <div class="kpi"><div class="kpi-icon">🔧</div><div class="kpi-lbl">Running costs / yr</div><div class="kpi-val cv-red" id="k-opex">—</div><div class="kpi-sub">staff, energy, maintenance</div></div>
        <div class="kpi"><div class="kpi-icon">⚖️</div><div class="kpi-lbl">Break-even</div><div class="kpi-val" id="k-be">—</div><div class="kpi-sub">from opening day</div></div>
        <div class="kpi"><div class="kpi-icon">🎯</div><div class="kpi-lbl">Viability score</div><div class="kpi-val" id="k-viab">—</div><div class="kpi-sub" id="k-viab-lbl">—</div></div>
      </div>
      <!-- extra mini KPIs -->
      <div class="kpi-row-5">
        <div class="kpi-mini"><div class="kpi-lbl">Cost per km</div><div class="kpi-val cv-blue" id="k2-cpkm">—</div></div>
        <div class="kpi-mini"><div class="kpi-lbl">Cost per rider/yr</div><div class="kpi-val" id="k2-cpr">—</div></div>
        <div class="kpi-mini"><div class="kpi-lbl">Subsidy per trip</div><div class="kpi-val cv-amber" id="k2-spt">—</div></div>
        <div class="kpi-mini"><div class="kpi-lbl">Revenue ratio</div><div class="kpi-val" id="k2-rr">—</div></div>
        <div class="kpi-mini"><div class="kpi-lbl">Benefit-cost ratio</div><div class="kpi-val cv-green" id="k2-bcr">—</div></div>
      </div>

      <!-- NETWORK SECTION -->
      <div class="sec-lbl">Network map &amp; lines</div>

      <!-- Sequential build progress (shown only for mode 3) -->
      <div id="seq-progress-bar" style="display:none;margin-bottom:8px">
        <div style="font-size:10px;color:var(--ink3);margin-bottom:5px;font-weight:600">⏱ Sequential build — click a phase to mark it complete:</div>
        <div class="seq-progress" id="seq-phases"></div>
      </div>

      <!-- Line manager -->
      <div class="nl-manager">
        <div class="nl-header">
          <div>
            <h4 id="nl-mode-title">Lines</h4>
            <p id="nl-mode-hint">Add lines, set length and scope per line</p>
          </div>
          <button class="nl-btn" onclick="addNetLine()" style="color:var(--blue);font-weight:700">＋ Add line</button>
        </div>
        <div class="nl-lines" id="nl-lines-list"></div>
      </div>

      <!-- City map + network canvas -->
      <div class="network-scheme">
        <div class="ns-header">
          <div><h4 id="ns-title">City &amp; Network Map</h4><p id="ns-subtitle">Drag stations · Double-click to rename · Add stops · Extend lines</p></div>
          <div id="ns-badges" style="display:flex;gap:6px;flex-wrap:wrap"></div>
        </div>
        <!-- Toolbar row 1: map scope + sequential -->
        <div style="display:flex;align-items:center;gap:8px;padding:8px 14px;background:#f8f6f0;border-bottom:1px solid var(--line);flex-wrap:wrap">
          <span style="font-size:10px;font-weight:700;color:var(--ink3);text-transform:uppercase;letter-spacing:.5px">View:</span>
          <div class="scope-toggle">
            <button class="scope-btn active" id="scope-city" onclick="setScope('city')">🏙 City only</button>
            <button class="scope-btn" id="scope-suburbs" onclick="setScope('suburbs')">🗺 With suburbs</button>
          </div>
          <div style="flex:1"></div>
          <button class="ns-tool" onclick="resetNetwork()" style="color:var(--amber)">↺ Reset</button>
        </div>
        <!-- Toolbar row 2: editing tools -->
        <div style="display:flex;align-items:center;gap:6px;padding:6px 14px;background:#f5f3ee;border-bottom:1px solid var(--line);flex-wrap:wrap">
          <span style="font-size:10px;font-weight:700;color:var(--ink3);text-transform:uppercase;letter-spacing:.5px;margin-right:2px">Edit:</span>
          <button class="ns-tool active" id="tool-select" onclick="setTool('select')">☛ Select</button>
          <button class="ns-tool" id="tool-addst" onclick="setTool('addst')">⊕ Add stop</button>
          <button class="ns-tool" id="tool-addline" onclick="setTool('addline')">⊕ New line</button>
          <button class="ns-tool" id="tool-extend" onclick="setTool('extend')">↗ Extend</button>
          <button class="ns-tool" id="tool-delete" onclick="setTool('delete')">✕ Delete</button>
        </div>
        <!-- Canvas -->
        <div style="background:#dce8d0;position:relative;min-height:200px">
          <canvas id="c-network" style="cursor:default;display:block;width:100%"></canvas>
          <div id="ns-tooltip" style="position:absolute;display:none;background:rgba(26,23,16,.88);color:#fff;font-size:10px;font-weight:500;padding:5px 9px;border-radius:5px;pointer-events:none;white-space:nowrap;box-shadow:0 3px 10px rgba(0,0,0,.25)"></div>
        </div>
        <div class="ns-legend" id="ns-legend"></div>
      </div>

      <div class="sec-lbl">📈 How many people will use it? (30-year forecast)</div>
      <div class="chart-card">
        <div class="cc-title">Daily passengers — will demand outgrow capacity?</div>
        <div class="cc-sub">The <strong>coloured area</strong> shows how many people will ride daily as the city grows. The <strong>dashed line</strong> is the maximum the system can carry. If they cross, you'll need to expand. 🖱 Hover for exact numbers.</div>
        <div class="chart-wrap"><canvas id="c-demand" height="200"></canvas><div class="ch-tip" id="tip-demand"></div></div>
      </div>
      <div class="charts-2">
        <div class="chart-card">
          <div class="cc-title">💰 Money in vs money out (each year)</div>
          <div class="cc-sub"><strong>Green bars</strong> = fare revenue collected. <strong>Red bars</strong> = cost to run the system. When green exceeds red, the system pays for itself. 🖱 Hover for exact values.</div>
          <div class="chart-wrap"><canvas id="c-cashflow" height="170"></canvas><div class="ch-tip" id="tip-cashflow"></div></div>
        </div>
        <div class="chart-card">
          <div class="cc-title">📊 Is the total investment worth it?</div>
          <div class="cc-sub">Tracks whether the project has paid back its costs over time. <strong>Crossing zero</strong> = break-even point. Going above zero means the investment has been recovered. 🖱 Hover for yearly value.</div>
          <div class="chart-wrap"><canvas id="c-npv" height="170"></canvas><div class="ch-tip" id="tip-npv"></div></div>
        </div>
      </div>

      <div class="sec-lbl">🏗️ Construction timeline — what happens and when</div>
      <div class="chart-card">
        <div class="cc-title" id="gantt-title">How long does it take to build?</div>
        <div class="cc-sub" id="gantt-total">Each bar is a phase of construction. The wider the bar, the longer that phase takes.</div>
        <div class="gantt-phase-legend" id="gantt-phase-legend" style="display:flex;gap:8px;flex-wrap:wrap;padding:0 0 8px 0;font-size:10px;color:var(--ink3)"></div>
        <div class="gantt-rows" id="gantt-rows"></div>
        <div class="g-axis"><div class="g-ticks" id="gantt-ticks"></div></div>
      </div>

      <div class="sec-lbl">🌍 Community &amp; environmental benefits</div>
      <div class="impact-grid">
        <div class="impact-item"><div class="imp-ico">🌿</div><div><div class="imp-lbl">CO₂ saved / year</div><div class="imp-val cv-green" id="i-co2">—</div><div class="imp-note">Supports EU Green Deal targets</div></div></div>
        <div class="impact-item"><div class="imp-ico">🚗</div><div><div class="imp-lbl">Cars off roads</div><div class="imp-val" id="i-cars">—</div><div class="imp-note">Daily car journeys replaced</div></div></div>
        <div class="impact-item"><div class="imp-ico">💼</div><div><div class="imp-lbl">Jobs created</div><div class="imp-val cv-blue" id="i-jobs">—</div><div class="imp-note">Construction + permanent operations</div></div></div>
        <div class="impact-item"><div class="imp-ico">🏘️</div><div><div class="imp-lbl">Property uplift</div><div class="imp-val cv-amber" id="i-prop">—</div><div class="imp-note">Near stations vs comparable areas</div></div></div>
        <div class="impact-item"><div class="imp-ico">⏱️</div><div><div class="imp-lbl">Time saved / commuter</div><div class="imp-val cv-blue" id="i-time">—</div><div class="imp-note">Vs current road travel</div></div></div>
        <div class="impact-item"><div class="imp-ico">💶</div><div><div class="imp-lbl">Economic benefit / yr</div><div class="imp-val cv-green" id="i-econ">—</div><div class="imp-note">Productivity + congestion savings</div></div></div>
        <div class="impact-item"><div class="imp-ico">🏥</div><div><div class="imp-lbl">Health benefit / yr</div><div class="imp-val cv-green" id="i-health">—</div><div class="imp-note">Reduced air pollution &amp; accidents</div></div></div>
        <div class="impact-item"><div class="imp-ico">♿</div><div><div class="imp-lbl">Accessible trips / day</div><div class="imp-val cv-blue" id="i-access">—</div><div class="imp-note">Mobility-impaired passengers served</div></div></div>
        <div class="impact-item"><div class="imp-ico">🌍</div><div><div class="imp-lbl">Lifetime CO₂ saving</div><div class="imp-val cv-green" id="i-co2life">—</div><div class="imp-note">Over 30-year project life</div></div></div>
      </div>

      <div class="sec-lbl">🎚️ What matters most? — policy levers ranked by impact</div>
      <div class="chart-card">
        <div class="cc-title">Which decisions move the needle most?</div>
        <div class="cc-sub">Each bar shows the range of outcomes if you push that lever from its lowest to highest setting. <strong>Wider bar = bigger impact on the project's total value.</strong> The coloured dot shows where your current setting sits. 🖱 Hover any bar for a plain-language explanation.</div>
        <div class="chart-wrap"><canvas id="c-sensitivity" height="230"></canvas><div class="ch-tip" id="tip-sensitivity"></div></div>
        <div id="sens-plain" style="margin-top:12px;display:flex;flex-direction:column;gap:6px"></div>
      </div>

      <div class="sec-lbl">⚠️ Risk analysis — what could go wrong?</div>
      <div id="risk-panel" style="margin-bottom:14px">
        <div style="background:var(--white);border:1px solid var(--line);border-radius:var(--r);padding:16px;box-shadow:var(--sh)">
          <div style="font-size:13px;font-weight:600;color:var(--ink);margin-bottom:4px">Project risk register</div>
          <div style="font-size:11px;color:var(--ink3);margin-bottom:12px">Updated automatically as you change policy levers. Each risk shows its likelihood, severity, and what you can do about it.</div>
          <div id="risk-matrix" style="margin-bottom:12px"></div>
          <div id="risk-list" style="display:flex;flex-direction:column;gap:7px"></div>
        </div>
      </div>

      <div class="sec-lbl">Save &amp; compare scenarios</div>
      <div style="background:var(--blue-bg);border:1px solid #c0d4f8;border-radius:9px;padding:10px 14px;margin-bottom:9px;font-size:12px;color:var(--blue)">
        💡 <strong>How to compare:</strong> Adjust levers → name scenario → Save. Repeat for other policy options. A comparison table and charts appear automatically.
      </div>
      <div class="sc-bar">
        <div class="sc-bar-lbl">Scenarios:</div>
        <div class="sc-chips" id="sc-chips"><span style="font-size:11px;color:var(--ink3);font-style:italic">None saved yet.</span></div>
        <div class="sc-save-row">
          <input class="sc-input" id="sc-name-in" placeholder="Name this scenario…" maxlength="28">
          <button class="btn btn-sm btn-green" onclick="saveScenario()">Save ＋</button>
        </div>
      </div>
      <div id="cmp-wrap" style="display:none">
        <div class="sec-lbl" style="margin-top:4px">🔀 Scenario comparison &amp; decision analysis</div>
        <!-- Decision tree recommendation -->
        <div class="dt-panel" id="dt-panel">
          <div style="font-size:13px;font-weight:700;margin-bottom:3px;display:flex;align-items:center;gap:7px">🌳 Decision tree recommendation <span style="font-size:10px;color:var(--ink3);font-weight:400">— updated each time you save a scenario</span></div>
          <div style="font-size:11px;color:var(--ink3);margin-bottom:12px">The system scores each scenario across 5 criteria, applies a decision tree to identify the most balanced choice, and explains its reasoning in plain language.</div>
          <div id="dt-winner-box"></div>
          <div id="dt-tree-nodes" class="dt-tree"></div>
          <div id="dt-ranking"></div>
        </div>
        <!-- Raw comparison table -->
        <div class="cmp-panel" style="margin-bottom:12px"><table><thead><tr id="cmp-thead"></tr></thead><tbody id="cmp-tbody"></tbody></table></div>
        <div class="charts-2">
          <div class="chart-card"><div class="cc-title">Daily passenger forecasts</div><div class="cc-sub">How ridership grows over 30 years for each scenario</div><canvas id="c-cmp-r" height="170"></canvas></div>
          <div class="chart-card"><div class="cc-title">Key financial figures compared</div><div class="cc-sub">Build cost, annual revenue, running costs and 30-year value</div><canvas id="c-cmp-f" height="170"></canvas></div>
        </div>
      </div>
            <div class="footnote">All figures in <strong>Euros (€)</strong>, calibrated to EU construction costs (2024 price levels). EU co-funding rates subject to eligibility criteria and national co-financing requirements. Projections are illustrative — always commission a full feasibility study before any public commitment. Sources: ITDP, World Bank, UITP, EU Cohesion Fund guidelines.</div>
    </div>
  </div>
</div>

</div>
<div id="toast"></div>

<script>
// roundRect polyfill for Safari/older browsers
if(!CanvasRenderingContext2D.prototype.roundRect){
  CanvasRenderingContext2D.prototype.roundRect=function(x,y,w,h,r){
    if(Array.isArray(r))r=r[0]||0;
    r=Math.min(Number(r)||0,Math.abs(w)/2,Math.abs(h)/2);
    this.moveTo(x+r,y);this.lineTo(x+w-r,y);this.arcTo(x+w,y,x+w,y+r,r);
    this.lineTo(x+w,y+h-r);this.arcTo(x+w,y+h,x+w-r,y+h,r);
    this.lineTo(x+r,y+h);this.arcTo(x,y+h,x,y+h-r,r);
    this.lineTo(x,y+r);this.arcTo(x,y,x+r,y,r);this.closePath();
  };
}
/* ═══ DATA ═══ */
const TERRAIN_TYPES=[
  {id:'flatland',  name:'Flat plain',     icon:'🌾',color:'#7a9a40',costMul:1.00,durMul:1.00,
   desc:'Flat terrain — standard construction costs. No tunnels or major bridges required.',
   extras:'Standard earthworks only. Minor drainage works.',
   mapBg:'#c8dda8',mapWater:false,mapHills:false,mapSea:false},
  {id:'river',     name:'River valley',   icon:'🌊',color:'#3a78a8',costMul:1.18,durMul:1.12,
   desc:'River crossings add bridge structures. Flood-plain engineering required along embankments.',
   extras:'+15–25% capex for bridges & flood protection. +10% construction time.',
   mapBg:'#c8dda8',mapWater:true,mapHills:false,mapSea:false},
  {id:'coastal',   name:'Coastal / delta',icon:'🏖️',color:'#0a7890',costMul:1.22,durMul:1.15,
   desc:'Soft coastal soils require deep foundations. Sea-facing stations need corrosion protection.',
   extras:'+20% capex. Saline groundwater complicates tunnelling.',
   mapBg:'#c8dde8',mapWater:false,mapHills:false,mapSea:true},
  {id:'hilly',     name:'Hilly terrain',  icon:'⛰️',color:'#8a6830',costMul:1.32,durMul:1.20,
   desc:'Rolling hills require cut-and-fill, retaining walls and occasional short tunnels.',
   extras:'+25–40% capex for earthworks and structures.',
   mapBg:'#c8d8a0',mapWater:false,mapHills:true,mapSea:false},
  {id:'mountain',  name:'Mountain',       icon:'🏔️',color:'#6a7090',costMul:1.65,durMul:1.45,
   desc:'Major mountain tunnels and viaducts dominate costs. Seismic assessment may be required.',
   extras:'+55–80% capex. Long tunnels add years to schedule.',
   mapBg:'#c0cca8',mapWater:false,mapHills:true,mapSea:false},
  {id:'plateau',   name:'High plateau',   icon:'🗻',color:'#8a8860',costMul:1.28,durMul:1.18,
   desc:'High-altitude construction adds logistics costs. Some viaducts for ravine crossings.',
   extras:'+25% capex. Altitude affects equipment performance.',
   mapBg:'#d4d0a0',mapWater:false,mapHills:true,mapSea:false},
  {id:'island',    name:'Island / archipelago',icon:'🏝️',color:'#20889a',costMul:1.45,durMul:1.35,
   desc:'Marine logistics for materials delivery. Causeway or tunnel crossings between islands.',
   extras:'+40–50% capex. Undersea tunnels are major cost drivers.',
   mapBg:'#b8d8e8',mapWater:false,mapHills:false,mapSea:true},
  {id:'delta',     name:'Wetland / marsh',icon:'🌿',color:'#3a8858',costMul:1.38,durMul:1.30,
   desc:'Soft peaty soils require pile foundations throughout. Drainage management is complex.',
   extras:'+35% capex for piling and drainage. Environmental permits add time.',
   mapBg:'#c0d8b0',mapWater:true,mapHills:false,mapSea:false},
];

const CITIES=[
  {id:'tiny',  name:'Small town',   pop:50000,  icon:'🏘️',ex:'Galway, Denia, Bressanone',
   note:'Small towns work best with electric buses or a tram pilot. Underground metro is not economically viable at this scale.',
   defaultTerrain:'flatland'},
  {id:'small', name:'Town',         pop:150000, icon:'🏙️',ex:'Matera, Évora, Jelenia Góra',
   note:'A tram line or quality BRT on the main corridor is the most cost-effective investment at this population.',
   defaultTerrain:'flatland'},
  {id:'medium',name:'City',         pop:400000, icon:'🌆',ex:'Strasbourg, Poznań, Tallinn',
   note:'Trams are the EU standard at this scale. Metro feasibility is justified on the highest-demand corridor.',
   defaultTerrain:'flatland'},
  {id:'large', name:'Large city',   pop:900000, icon:'🌇',ex:'Lyon, Łódź, Oporto, Málaga',
   note:'Metro backbone or expanded tram network make strong economic sense. BRT for suburban feeders.',
   defaultTerrain:'flatland'},
  {id:'metro', name:'Metropolis',   pop:2500000,icon:'🏢',ex:'Warsaw, Bucharest, Budapest',
   note:'Multi-line metro is justified. Commuter rail for outlying areas. Trams and BRT as feeder layers.',
   defaultTerrain:'flatland'},
  {id:'mega',  name:'Major capital',pop:6000000,icon:'🌃',ex:'Madrid, Rome, Berlin, Paris',
   note:'Full metro network with commuter rail integration across the entire functional urban area.',
   defaultTerrain:'flatland'},
];

const SUBURBS={
  tiny:[
    {name:'University campus',pop:12000,dist:'4 km',icon:'🎓',type:'university',dir:'N',color:'#5b4fcf',
     desc:'Students & staff. Strong off-peak ridership. Dense pedestrian area.'},
    {name:'Old hamlet (NW)',pop:2800,dist:'5 km',icon:'🏡',type:'village',dir:'NW',color:'#7a6040',
     desc:'Tiny residential settlement. Low density, 3–4 streets, mostly single-family houses.'},
    {name:'Riverside village',pop:3500,dist:'7 km',icon:'🌊',type:'village',dir:'S',color:'#3a7a8a',
     desc:'Small village by the river. Tourism potential, car-dependent today.'},
    {name:'Farm commune (E)',pop:1800,dist:'9 km',icon:'🌾',type:'village',dir:'E',color:'#8a7040',
     desc:'Dispersed agricultural settlement. Very low density — feeder bus stop only.'},
    {name:'Industrial estate',pop:6000,dist:'8 km',icon:'🏭',type:'industrial',dir:'E',color:'#607080',
     desc:'Manufacturing units. Shift-work generates predictable peak demand.'},
    {name:'Airport & logistics',pop:4000,dist:'12 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090',
     desc:'Regional airport. Staff commuters plus leisure travellers.'},
  ],
  small:[
    {name:'University quarter',pop:22000,dist:'5 km',icon:'🎓',type:'university',dir:'N',color:'#5b4fcf',
     desc:'Major campus with student housing. High ridership outside peak hours.'},
    {name:'Northern residential zone',pop:28000,dist:'9 km',icon:'🏘️',type:'residential',dir:'N',color:'#1a7a3e',
     desc:'Post-war housing estates. Families and commuters, very high car use today.'},
    {name:'Western village cluster',pop:9000,dist:'11 km',icon:'🏡',type:'village',dir:'W',color:'#7a6040',
     desc:'4–5 small villages sharing a commune boundary. Dispersed but collectively significant.'},
    {name:'Hillside hamlets (S)',pop:4200,dist:'8 km',icon:'🌳',type:'village',dir:'S',color:'#8a7040',
     desc:'Small residential hamlets on the southern slopes. Narrow roads, challenging access.'},
    {name:'Industrial belt',pop:16000,dist:'7 km',icon:'🏭',type:'industrial',dir:'E',color:'#607080',
     desc:'Mixed industry, logistics and warehousing. Good transit demand in mornings.'},
    {name:'Airport corridor',pop:14000,dist:'15 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090',
     desc:'Airport and hotel strip. Workers plus frequent flyers.'},
    {name:'Coastal resort town',pop:11000,dist:'14 km',icon:'🏖️',type:'seaside',dir:'SW',color:'#0a7890',
     desc:'Tourist town. Seasonal peak demand, permanent resident base.'},
    {name:'River port & quays',pop:9000,dist:'10 km',icon:'⚓',type:'port',dir:'SE',color:'#2a4070',
     desc:'Working waterfront, mixed residential above the quays.'},
  ],
  medium:[
    {name:'University & research district',pop:32000,dist:'6 km',icon:'🎓',type:'university',dir:'N',color:'#5b4fcf',
     desc:'Research university plus tech spin-off campus. 24/7 activity pattern.'},
    {name:'Northern suburbs',pop:62000,dist:'12 km',icon:'🏘️',type:'residential',dir:'N',color:'#1a7a3e',
     desc:'Large post-1960s residential belt. Very high commuter demand.'},
    {name:'Eastern communes',pop:48000,dist:'10 km',icon:'🏡',type:'residential',dir:'E',color:'#3a7a3e',
     desc:'Mix of older communes and newer residential estates.'},
    {name:'Village arc (NW)',pop:11000,dist:'16 km',icon:'🌳',type:'village',dir:'NW',color:'#7a6040',
     desc:'7–9 small villages in a 10 km arc. Some semi-rural, some dormitory settlements.'},
    {name:'Rural township (SE)',pop:6500,dist:'18 km',icon:'🌾',type:'village',dir:'SE',color:'#8a7040',
     desc:'Small market town surrounded by farmland. Infrequent bus service today.'},
    {name:'Airport & logistics hub',pop:25000,dist:'18 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090',
     desc:'International airport with cargo and logistics zone.'},
    {name:'Southern coastal town',pop:40000,dist:'15 km',icon:'🏖️',type:'seaside',dir:'S',color:'#0a7890',
     desc:'Coastal town with year-round population and summer tourism.'},
    {name:'Sea port & warehousing',pop:28000,dist:'13 km',icon:'🚢',type:'port',dir:'SE',color:'#2a4070',
     desc:'Commercial port. Container terminal plus related services.'},
    {name:'Western industrial',pop:35000,dist:'11 km',icon:'🏭',type:'industrial',dir:'W',color:'#607080',
     desc:'Industrial park and technology zone. Shift and office workers.'},
    {name:'Hospital campus',pop:8000,dist:'5 km',icon:'🏥',type:'institution',dir:'SW',color:'#d03060',
     desc:'Major regional hospital. 24/7 staff travel needs.'},
  ],
  large:[
    {name:'Northern commuter belt',pop:125000,dist:'18 km',icon:'🚉',type:'residential',dir:'N',color:'#1a7a3e',
     desc:'Dense commuter zone. Peak demand exceeds anything in city core.'},
    {name:'Eastern towns',pop:88000,dist:'15 km',icon:'🏙️',type:'residential',dir:'E',color:'#3a5090',
     desc:'Formerly independent towns, now functionally merged with the city.'},
    {name:'International airport',pop:58000,dist:'22 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090',
     desc:'Major hub with 24/7 operations. Direct rail link is high priority.'},
    {name:'Southern coastal area',pop:92000,dist:'20 km',icon:'🌊',type:'seaside',dir:'S',color:'#0a7890',
     desc:'Coastal strip with towns, beaches and ferry terminal.'},
    {name:'Sea port & maritime zone',pop:48000,dist:'22 km',icon:'🚢',type:'port',dir:'SE',color:'#2a4070',
     desc:'Major commercial port and fisheries.'},
    {name:'University cluster',pop:42000,dist:'8 km',icon:'🎓',type:'university',dir:'NW',color:'#5b4fcf',
     desc:'Multi-campus university, science park, student housing.'},
    {name:'Western suburbs',pop:104000,dist:'14 km',icon:'🏘️',type:'residential',dir:'W',color:'#2a7a3e',
     desc:'Post-1970s residential expansion zone.'},
    {name:'Industrial & tech park',pop:52000,dist:'16 km',icon:'🏭',type:'industrial',dir:'SW',color:'#607080',
     desc:'Mixed industry, automotive, data centres.'},
    {name:'Village ring (outer)',pop:28000,dist:'28 km',icon:'🌳',type:'village',dir:'NW',color:'#7a6040',
     desc:'Ring of 12–15 small villages and hamlets in the outer commuter zone.'},
    {name:'Rural dormitory towns',pop:18000,dist:'32 km',icon:'🌾',type:'village',dir:'N',color:'#8a7040',
     desc:'Small towns 25–35 km out. Car-dependent but large enough for rail feeder.'},
    {name:'Hospital & science campus',pop:18000,dist:'7 km',icon:'🏥',type:'institution',dir:'SW',color:'#d03060',
     desc:'University hospital and medical research park.'},
  ],
  metro:[
    {name:'Northern suburb zone',pop:285000,dist:'22 km',icon:'🚉',type:'residential',dir:'N',color:'#1a7a3e',
     desc:'Dense suburban belt across multiple municipalities.'},
    {name:'Eastern satellite cities',pop:215000,dist:'28 km',icon:'🏙️',type:'residential',dir:'E',color:'#3a5090',
     desc:'Formerly independent cities now part of the metro FUA.'},
    {name:'Southern coastal region',pop:185000,dist:'25 km',icon:'🌊',type:'seaside',dir:'S',color:'#0a7890',
     desc:'Coastal strip, tourism infrastructure, ferry ports.'},
    {name:'Western commuter belt',pop:245000,dist:'20 km',icon:'🏡',type:'residential',dir:'W',color:'#2a7a3e',
     desc:'High-frequency commuter corridor.'},
    {name:'International airport hub',pop:125000,dist:'32 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090',
     desc:'Major hub airport with aerotropolis development.'},
    {name:'University & research city',pop:95000,dist:'14 km',icon:'🎓',type:'university',dir:'NW',color:'#5b4fcf',
     desc:'University town and innovation district.'},
    {name:'Container port district',pop:145000,dist:'28 km',icon:'🚢',type:'port',dir:'SE',color:'#2a4070',
     desc:'Major port complex. Maritime and logistics industry.'},
    {name:'Industrial corridor',pop:108000,dist:'24 km',icon:'🏭',type:'industrial',dir:'SW',color:'#607080',
     desc:'Heavy industry, automotive, logistics.'},
    {name:'Rural hinterland towns',pop:82000,dist:'40 km',icon:'🌳',type:'village',dir:'NW',color:'#7a6040',
     desc:'Market towns and villages in the outer ring. 15–25 small settlements.'},
    {name:'Healthcare & biotech zone',pop:38000,dist:'10 km',icon:'🏥',type:'institution',dir:'W',color:'#d03060',
     desc:'Hospital cluster and pharmaceutical R&D campus.'},
  ],
  mega:[
    {name:'North metro zone',pop:820000,dist:'30 km',icon:'🏙️',type:'residential',dir:'N',color:'#1a7a3e'},
    {name:'East industrial corridor',pop:560000,dist:'38 km',icon:'🏭',type:'industrial',dir:'E',color:'#607080'},
    {name:'South coastal region',pop:440000,dist:'35 km',icon:'🌊',type:'seaside',dir:'S',color:'#0a7890'},
    {name:'West commuter suburbs',pop:680000,dist:'28 km',icon:'🚉',type:'residential',dir:'W',color:'#2a7a3e'},
    {name:'Airport super-hub',pop:300000,dist:'45 km',icon:'✈️',type:'airport',dir:'NE',color:'#2a6090'},
    {name:'Port & logistics megazone',pop:250000,dist:'40 km',icon:'🚢',type:'port',dir:'SE',color:'#2a4070'},
    {name:'University region',pop:180000,dist:'20 km',icon:'🎓',type:'university',dir:'NW',color:'#5b4fcf'},
    {name:'Outer ring towns',pop:200000,dist:'55 km',icon:'🌳',type:'village',dir:'NW',color:'#7a6040'},
  ],
}
const MODES=[
  // ── Rail-based ──────────────────────────────────────────────────────────
  {id:'metro',name:'Metro',icon:'🚇',color:'#b0261a',
   desc:'Fully segregated underground or elevated heavy rail. Highest capacity, highest cost. No interaction with road traffic.',
   cpmUg:260,cpmEl:175,sc:55,opkm:4.2,capF:42000,rf:1.00,df:1.00,
   phases:['Planning & DEIA','Land acquisition','Civil works','Systems & rolling stock','Testing & safety'],pp:[14,10,50,19,7],
   fitFn:(t,s)=>{const p=t+s;return p<300000?4:p<600000?28:p<1500000?68:90},
   fitWhy:(t,s)=>{const p=t+s;return p<300000?'Too small — tunnelling costs far exceed realistic ridership.':p<600000?'Possible on one busy corridor. Elevated option reduces cost significantly.':p<1500000?'Metro justified on 1–2 key corridors. Consider elevated sections to control costs.':'Metro is the essential backbone. Underground city centre, elevated suburbs.'}},
  {id:'lrt',name:'Light Rail (LRT)',icon:'🚊',color:'#7a4a00',
   desc:'Runs mainly on dedicated or segregated tracks — tunnels, viaducts or barrier-protected lanes. Signal priority at intersections. Trains of 2–4 coupled carriages, up to 90–110 km/h. Up to 4× the capacity of a tram.',
   cpmUg:null,cpmEl:38,sc:10,opkm:2.4,capF:22000,rf:0.72,df:0.68,
   phases:['Planning & permits','Environmental review','Track & civil works','Systems & electrification','Commissioning'],pp:[14,10,49,20,7],
   fitFn:(t,s)=>{const p=t+s;return p<80000?10:p<300000?58:p<1400000?88:78},
   fitWhy:(t,s)=>{const p=t+s;return p<80000?'Too small — tram or eBus more appropriate.':p<300000?'LRT justified on one high-demand corridor with room for dedicated track.':p<1400000?'LRT is the optimal backbone at this scale — speed, capacity and EU co-funding eligibility align well.':'Use LRT on secondary corridors as metro feeder.'}},
  {id:'tram',name:'Tram',icon:'🚋',color:'#9a6000',
   desc:'Runs on public streets, sharing space with cars and pedestrians. Subject to normal traffic signals. Single or short vehicles, max ~65 km/h. Ideal for city centres and medium-density corridors.',
   cpmUg:null,cpmEl:20,sc:5,opkm:1.6,capF:12000,rf:0.58,df:0.52,
   phases:['Planning & permits','Environmental review','Track & civil works','Systems & electrification','Commissioning'],pp:[12,10,50,21,7],
   fitFn:(t,s)=>{const p=t+s;return p<40000?8:p<150000?60:p<900000?90:68},
   fitWhy:(t,s)=>{const p=t+s;return p<40000?'Too small — eBus or trolleybus more appropriate.':p<150000?'A single tram line on the main street is cost-effective and popular.':p<900000?'Trams are the EU standard backbone for mid-size cities — proven, attractive, walkable.':'Use trams as neighbourhood feeders alongside LRT or metro.'}},
  {id:'commuter',name:'Commuter Rail',icon:'🚆',color:'#105280',
   desc:'Heavy rail linking suburbs and satellite towns to the city centre. Often reuses existing freight or intercity tracks. High capacity, long distances, infrequent stops.',
   cpmUg:null,cpmEl:48,sc:18,opkm:2.8,capF:24000,rf:0.70,df:0.70,
   phases:['Planning & feasibility','Environmental impact','Track & civil','Systems','Commissioning'],pp:[14,10,46,20,10],
   fitFn:(t,s)=>{return s<50000?6:t+s<400000?24:t+s<1200000?60:88},
   fitWhy:(t,s)=>{const p=t+s;return s<50000?'No significant suburb population — not justified yet.':p<400000?'Too small for heavy commuter rail.':p<1200000?'Worth exploring if suburbs are 12km+ from centre. Can reuse freight lines.':'Strongly recommended — transforms metro-wide connectivity.'}},
  // ── Bus-based ───────────────────────────────────────────────────────────
  {id:'brt',name:'Bus Rapid Transit',icon:'🚌',color:'#186840',
   desc:'High-frequency buses on dedicated lanes with level boarding, off-board ticketing and signal priority. Operates on urban and suburban arterials. Closest bus equivalent to a tram in terms of quality.',
   cpmUg:null,cpmEl:7,sc:1.8,opkm:0.85,capF:7000,rf:0.44,df:0.37,
   phases:['Planning','Site prep','Lane & road works','Stations & tech','Testing'],pp:[12,8,57,17,6],
   fitFn:(t,s)=>{const p=t+s;return p<60000?70:p<400000?90:p<1800000?76:58},
   fitWhy:(t,s)=>{const p=t+s;return p<60000?'Excellent value — quality transit at minimal investment.':p<400000?'Best value option — ~80% of tram quality at ~20% of cost. Quick to build.':p<1800000?'Works well on secondary corridors alongside trams or metro.':'Suburban and feeder role at this scale.'}},
  {id:'ebus',name:'Electric Bus',icon:'⚡',color:'#2a6e9a',
   desc:'Zero-emission battery-electric buses operating on standard city routes. No overhead wires needed. Charges at depot overnight and at terminal stops. Lower noise, lower running costs than diesel.',
   cpmUg:null,cpmEl:4,sc:0.8,opkm:0.55,capF:6000,rf:0.38,df:0.24,
   phases:['Planning','Depot & grid upgrade','Road works','Charging infra','Testing'],pp:[10,10,55,19,6],
   fitFn:(t,s)=>{const p=t+s;return p<30000?80:p<200000?90:p<800000?78:60},
   fitWhy:(t,s)=>{const p=t+s;return p<30000?'Ideal starter network — zero emissions, low cost, fast to deploy.':p<200000?'Excellent urban sustainable choice. EU Green Deal funding eligible. Quick wins on air quality.':p<800000?'Strong for neighbourhood and secondary routes. Pair with tram or LRT on main corridors.':'City-wide eBus network as feeder to rail modes.'}},
  {id:'hybrid',name:'Hybrid Bus',icon:'🔋',color:'#4a7a30',
   desc:'Diesel-electric hybrid buses. Combustion engine charges a battery; electric motor powers low-speed urban sections. Significant fuel and emissions savings over pure diesel with no charging infrastructure needed.',
   cpmUg:null,cpmEl:3.5,sc:0.6,opkm:0.50,capF:5500,rf:0.35,df:0.22,
   phases:['Planning','Depot upgrade','Road works','Fleet delivery','Testing'],pp:[8,8,52,26,6],
   fitFn:(t,s)=>{const p=t+s;return p<30000?75:p<200000?82:p<800000?70:50},
   fitWhy:(t,s)=>{const p=t+s;return p<30000?'Good starter option where charging infrastructure is not yet available.':p<200000?'Practical transition solution — reduces emissions now while planning for full electrification.':p<800000?'Works well as interim fleet before full electric transition. Lower EU funding eligibility than eBus.':'Large hybrid fleets are a stepping stone; plan transition to electric within 10 years.'}},
  {id:'biogas',name:'Biogas Bus',icon:'🌿',color:'#3a7a3a',
   desc:'Buses powered by compressed biomethane (biogas) from organic waste. Near-zero net CO₂ emissions. Uses existing gas-engine bus technology. Requires dedicated refuelling stations at depots.',
   cpmUg:null,cpmEl:3.8,sc:0.7,opkm:0.52,capF:5800,rf:0.36,df:0.23,
   phases:['Planning','Depot & fuel infra','Road works','Fleet delivery','Testing'],pp:[10,12,50,22,6],
   fitFn:(t,s)=>{const p=t+s;return p<30000?65:p<200000?78:p<800000?72:52},
   fitWhy:(t,s)=>{const p=t+s;return p<30000?'Viable green option where local biogas supply exists.':p<200000?'Good circular-economy choice — especially where city manages organic waste streams.':p<800000?'Works alongside electric fleet. Strong story for EU Green Deal and rural biogas projects.':'Biogas works best in hybrid fleets alongside electric; not suited as sole solution at scale.'}},
  {id:'trolley',name:'Trolleybus',icon:'🔌',color:'#4a2e90',
   desc:'Electric buses drawing power from overhead wires — like a tram but on rubber tyres. No battery charging needed for main route; some modern models have small batteries for off-wire operation. Very popular in many EU cities (Geneva, Bratislava, Minsk, Athens).',
   cpmUg:null,cpmEl:9,sc:1.5,opkm:0.60,capF:8000,rf:0.45,df:0.28,
   phases:['Planning','Wire & substation works','Road works','Fleet delivery','Testing'],pp:[11,18,48,17,6],
   fitFn:(t,s)=>{const p=t+s;return p<40000?55:p<200000?80:p<900000?86:70},
   fitWhy:(t,s)=>{const p=t+s;return p<40000?'Trolleybus overkill for very small towns — eBus simpler.':p<200000?'Excellent urban choice on fixed high-frequency routes. Lower running costs than diesel or battery.':p<900000?'Trolleybus networks are proven in many EU cities. High reliability, zero tailpipe emissions, lower energy cost than battery.':'Core urban network trolleybus with diesel/electric extensions to suburbs.'}},
];
const FARE_M={flat:1.00,zone:1.08,dist:1.05,peak:1.12,free:0};
const FUND_D={public:0.93,ppp:1.00,cohesion:1.05,cef:1.02,erdf:1.04,dev:1.06};
const EU_SHARE={public:0,ppp:0,cohesion:0.85,cef:0.50,erdf:0.70,dev:0};
const EU_FUNDS={
  cohesion:{name:'EU Cohesion Fund',desc:'For less-developed regions. Covers up to 85% of eligible costs. Requires national co-financing and EU audit compliance.',pct:0.85,col:'#003399'},
  cef:{name:'Connecting Europe Facility (CEF)',desc:'For cross-border and core network corridors. Up to 50% grant for transport projects on the TEN-T network.',pct:0.50,col:'#1a6fbf'},
  erdf:{name:'European Regional Development Fund (ERDF)',desc:'Supports sustainable urban transport. Typically 70% EU share with 30% national/local match required.',pct:0.70,col:'#2a7a9a'},
  dev:{name:'Property Value Capture',desc:'Funding from land value uplift near stations. No EU grant — project self-financed through development levies.',pct:0,col:'#7a6040'},
};
const SPD=['','Cautious','Standard','Accelerated'];
const SC_COLORS=['#155090','#1a7a3e','#b0261a','#9a6000','#4a2e90','#067a70','#8a5800','#4a7a10'];
const LINE_COLS=['#b0261a','#155090','#1a7a3e','#9a6000','#7b3fb0','#c4660f','#0a8a7a','#8a1a3a'];

/* ═══ STATE ═══ */
let selCity=null,selSuburbs=new Set(),selMode=null,selTerrain='flatland';
let metroType='underground',numLines=1;
let scenarios=[],activeScId=null,currentStep=1,lastCalc=null;

const G=id=>document.getElementById(id);
const gv=id=>parseFloat(G(id).value);
const gi=id=>parseInt(G(id).value);
const fP=n=>n>=1e6?(n/1e6).toFixed(n%1e6===0?0:1)+'M':Math.round(n/1000)+'K';
const fPF=n=>n>=1e6?(n/1e6).toFixed(1)+'M':Math.round(n/1000).toLocaleString()+'K';
// Euro formatter — monetary values internally in €M
const fE=v=>{const a=Math.abs(v*1e6),s=v<0?'−':'';if(a>=1e9)return s+'€'+(a/1e9).toFixed(1)+'B';if(a>=1e6)return s+'€'+(a/1e6).toFixed(1)+'M';return s+'€'+Math.round(a/1000)+'K';};

function totalPop(){return selCity?selCity.pop+suburbPop():0;}
function suburbPop(){if(!selCity)return 0;const subs=SUBURBS[selCity.id]||[];let t=0;selSuburbs.forEach(i=>{t+=(subs[i]?.pop||0);});return t;}
function modeCpm(m){if(m.id==='metro')return metroType==='underground'?m.cpmUg:m.cpmEl;return m.cpmEl||20;}

/* ═══ NAV ═══ */
function goStep(n){
  if(n>=2&&!selCity){toast('Please choose a city size first.');return;}
  if(n>=4&&!selMode)selMode=MODES[0];
  currentStep=n;
  document.querySelectorAll('.step-section').forEach((s,i)=>s.classList.toggle('active',i+1===n));
  document.querySelectorAll('.hdr-step').forEach((s,i)=>{s.classList.toggle('active',i+1===n);s.classList.toggle('done',i+1<n);});
  G('hdr-pop').textContent=totalPop()>0?fP(totalPop()):'—';
  if(n===1){renderCityGrid();renderTerrainGrid();}if(n===2)renderSuburbs();if(n===3)renderRecommend();if(n===4){
    renderSimModeTabs();
    // Seed first line with mode-aware length if no lines yet
    if(selMode&&netState.lines&&netState.lines.length===0){
      addNetLine();
      const ln=netState.lines[0];
      ln.seqStatus='open';
      ln.label=selMode.name+' Line 1';
      ln.lineLen=MODE_LEN_DEFAULTS[selMode.id]||10;
      ln.scope='city';
    } else if(selMode&&netState.lines&&netState.lines.length>0){
      // Update existing lines with mode defaults if they lack lineLen
      netState.lines.forEach(ln=>{if(!ln.lineLen)ln.lineLen=MODE_LEN_DEFAULTS[selMode.id]||10;if(!ln.scope)ln.scope='city';});
      renderLineManager();
    }
    applyModeAwareLength();
    setTimeout(upd,30);
  }
  window.scrollTo(0,0);
}

/* ═══ STEP 1 ═══ */
function renderCityGrid(){
  G('city-grid').innerHTML=CITIES.map(c=>{
    const t=TERRAIN_TYPES.find(t=>t.id===selTerrain)||TERRAIN_TYPES[0];
    const isSel=selCity?.id===c.id;
    return`<div class="city-card ${isSel?'sel':''}" onclick="selC('${c.id}')">
      <div class="c-icon">${c.icon}</div>
      <div class="c-name">${c.name}</div>
      <div class="c-pop">${fP(c.pop)}</div>
      <div class="c-ex">${c.ex}</div>
    </div>`;
  }).join('');
}
function renderTerrainGrid(){
  G('terrain-grid').innerHTML=TERRAIN_TYPES.map(t=>{
    const isSel=selTerrain===t.id;
    const pct=Math.round((t.costMul-1)*100);
    return`<div class="t-card ${isSel?'sel':''}" onclick="selT('${t.id}')" style="${isSel?'border-color:'+t.color+';background:'+t.color+'18':''}" >
      <div class="t-icon">${t.icon}</div>
      <div class="t-name" style="${isSel?'color:'+t.color:''}">${t.name}</div>
      <div class="t-cost">${pct===0?'Base cost':'+'+pct+'% cost'}</div>
    </div>`;
  }).join('');
  // Info banner
  const t=TERRAIN_TYPES.find(t=>t.id===selTerrain)||TERRAIN_TYPES[0];
  const pct=Math.round((t.costMul-1)*100);
  const info=G('terrain-info');
  info.style.display='flex';
  info.style.background=t.color+'18';
  info.style.border='1.5px solid '+t.color+'44';
  info.innerHTML=`<div class="ti-ico">${t.icon}</div><div><strong style="color:${t.color}">${t.name}</strong> — ${t.desc}<br><span style="font-size:10px;color:var(--ink3);margin-top:3px;display:block">💡 ${t.extras}</span></div>`;
}
function selC(id){
  selCity=CITIES.find(c=>c.id===id);selSuburbs.clear();selMode=null;
  renderCityGrid();
  const n=G('city-note');n.style.display='block';n.textContent=selCity.note;
}
function selT(id){
  selTerrain=id;
  renderTerrainGrid();
  renderCityGrid();
  // Reset network to recalculate costs
  if(selMode&&selCity){netState.initialized=false;netState.modeId=null;}
}

/* ═══ STEP 2 ═══ */
let subFilter='all';
const SUB_TYPE_LABELS={university:'🎓 University',residential:'🏘️ Residential',industrial:'🏭 Industrial',airport:'✈️ Airport',seaside:'🏖️ Seaside',port:'🚢 Port',village:'🌳 Village',institution:'🏥 Institution',all:'All types'};
function renderSuburbs(){
  G('pb-city').textContent=fP(selCity.pop);G('pb-city-name').textContent=selCity.name;
  const subs=SUBURBS[selCity.id]||[];
  // Build filter buttons
  const types=['all',...new Set(subs.map(s=>s.type))];
  G('sub-filter').innerHTML=types.map(t=>`<button class="sub-filt-btn ${subFilter===t?'active':''}" onclick="setSubFilter('${t}')">${SUB_TYPE_LABELS[t]||t}</button>`).join('');
  // Render suburb cards
  const filtered=subFilter==='all'?subs:subs.filter(s=>s.type===subFilter);
  G('suburb-grid').innerHTML=filtered.map((s)=>{
    const i=subs.indexOf(s);
    const typeCol=s.color||'#888';
    const typeLbl=SUB_TYPE_LABELS[s.type]||s.type;
    const isVillage=s.type==='village'||s.type==='residential';
    const sizeLabel=s.pop<5000?'Hamlet':s.pop<15000?'Village':s.pop<40000?'Small town':'Urban zone';
    return`<div class="sub-card ${selSuburbs.has(i)?'sel':''}" onclick="togSub(${i})">
      <div class="sub-check">${selSuburbs.has(i)?'✓':''}</div>
      <div class="sub-icon">${s.icon}</div>
      <div style="flex:1;min-width:0">
        <div class="sub-name">${s.name}</div>
        <div class="sub-meta">${fP(s.pop)} people · ${s.dist} from centre${s.dir?' · '+s.dir:''}</div>
        ${s.desc?`<div style="font-size:9px;color:var(--ink3);margin-top:2px;line-height:1.4">${s.desc}</div>`:''}
        <div style="margin-top:3px;display:flex;gap:4px;flex-wrap:wrap;align-items:center">
          <span class="sub-type" style="background:${typeCol}20;color:${typeCol}">${typeLbl}</span>
          ${isVillage?`<span style="background:#88880015;color:#886630;font-size:8px;font-weight:700;padding:1px 5px;border-radius:5px">${sizeLabel}</span>`:''}
        </div>
      </div>
    </div>`;
  }).join('');
  updBanner();
}
function setSubFilter(t){subFilter=t;renderSuburbs();}
function togSub(i){selSuburbs.has(i)?selSuburbs.delete(i):selSuburbs.add(i);renderSuburbs();}
function updBanner(){
  const sp=suburbPop(),tot=selCity.pop+sp;
  G('pb-sub').textContent=fP(sp||0);G('pb-sub-count').textContent=selSuburbs.size===0?'None selected':`${selSuburbs.size} area${selSuburbs.size>1?'s':''} selected`;
  G('pb-total').textContent=fP(tot);G('hdr-pop').textContent=fP(tot);
}

/* ═══ STEP 3 ═══ */
function fitScore(m){return m.fitFn(selCity.pop,suburbPop());}
function renderRecommend(){
  const tot=totalPop(),sp=suburbPop();
  const el=G('rec-metro-pop');if(el)el.textContent=fP(tot);
  const ranked=[...MODES].map(m=>({m,s:fitScore(m)})).sort((a,b)=>b.s-a.s);
  if(!selMode)selMode=ranked[0].m;
  G('mode-selector').innerHTML=ranked.map(({m,s})=>{
    const bc=s>=80?'tb-best':s>=60?'tb-good':s>=35?'tb-ok':'tb-no';
    const bl=s>=80?'⭐ Best':s>=60?'✅ Good':s>=35?'⚡ OK':'✗ Poor';
    const col=s>=80?'var(--amber)':s>=60?'var(--green)':s>=35?'var(--blue)':'var(--ink3)';
    const isRail=['metro','lrt','tram','commuter'].includes(m.id);
    const cat=isRail?'🚆 Rail':'🚌 Bus';
    const catBg=isRail?'#e8f0fc':'#e8faf0';
    const catTxt=isRail?'#1a3a8a':'#1a5a3a';
    const leftBorder=selMode?.id===m.id?'border-left:4px solid '+m.color:'border-left:4px solid transparent';
    return`<div class="mode-pick ${selMode?.id===m.id?'sel':''}" style="${selMode?.id===m.id?'border-color:'+m.color+';':''};${leftBorder}" onclick="pickMode('${m.id}')">`
      +`<div class="mp-top"><span class="mp-icon">${m.icon}</span><span class="mp-name" style="color:${selMode?.id===m.id?m.color:'var(--ink)'}">${m.name}</span></div>`
      +`<span class="mp-cat" style="background:${catBg};color:${catTxt}">${cat}</span>`
      +`<div class="mp-desc">${m.desc||''}</div>`
      +`<div class="mp-bottom"><span class="mp-fit" style="color:${col}">${s}%</span><span class="mp-badge ${bc}">${bl}</span></div>`
    +`</div>`;
  }).join('');
  G('btn-simulate').textContent=`Simulate ${selMode.name} →`;
  G('rec-thead').innerHTML=['Transit type','Fit for city','Daily riders','Build cost','Build time','30-yr value'].map((c,i)=>`<th ${i>0?'class="r"':''}>${c}</th>`).join('');
  const best=Math.max(...ranked.map(r=>r.s));
  G('rec-tbody').innerHTML=ranked.map(({m,s})=>{
    const calc=qcalc(m,tot,sp,1.2,0.4,18,14,2,6,'ppp','zone',0.04,0.015,'underground',1);
    const bc=s>=80?'tb-best':s>=60?'tb-good':s>=35?'tb-ok':'tb-no';
    const bt=s>=80?'Best fit':s>=60?'Good':s>=35?'Possible':'Not recommended';
    return`<tr style="cursor:pointer" onclick="pickMode('${m.id}');goStep(4)"><td><div class="mode-cell"><span class="mdot" style="background:${m.color}"></span>${m.icon} ${m.name}</div></td><td class="r"><span class="tbadge ${bc}">${bt}</span> <strong style="color:${s>=60?'var(--green)':s>=35?'var(--amber)':'var(--ink3)'}">${s}%</strong></td><td class="r ${s===best?'best-v':''}">${fPF(calc.riders)}${s===best?' ✓':''}</td><td class="r">${fE(calc.capex)}</td><td class="r">${calc.dur.toFixed(1)} yr</td><td class="r" style="color:${calc.npv>=0?'var(--green)':'var(--red)'}">${calc.npv>=0?'+':''}${fE(calc.npv)}</td></tr>`;
  }).join('');
  setTimeout(()=>{drawFit(ranked);drawCostCap(ranked,tot,sp);},60);
}
function pickMode(id){selMode=MODES.find(m=>m.id===id);renderRecommend();}

/* ═══ CALC ENGINE (monetary values in €M) ═══ */
function qcalc(m,cityPop,subPop,ticket,subsidy,length,stations,speed,freq,funding,fare,discount,growth,mt,lines){
  growth=growth||0.015;mt=mt||'underground';lines=lines||1;
  const cpm=(m.id==='metro')?(mt==='underground'?m.cpmUg:m.cpmEl):(m.cpmEl||20);
  const fD=FUND_D[funding]||1,fM2=FARE_M[fare]||1;
  const sMul=[0,.88,1.00,1.18][speed]||1,dMul=[0,1.45,1.00,0.65][speed]||1;
  // lineFactor: simultaneous = each line adds 80% of first line cost; sequential = 100% per line (funded/built separately)
  const isSeq=typeof buildStrategy!=='undefined'&&buildStrategy==='seq';
  const lineFactor=lines<=1?1:isSeq?lines:(1+(lines-1)*0.80);
  // Sequential build: lines open at different times — stagger ridership and revenue
  const lineOpenStagger=isSeq&&lines>1?1.2:0; // extra years before full network ridership

  const terrain=TERRAIN_TYPES.find(t=>t.id===selTerrain)||TERRAIN_TYPES[0];
  const tCostMul=terrain.costMul,tDurMul=terrain.durMul;
  const capex=(length*cpm+stations*m.sc)*sMul*fD*lineFactor*tCostMul;
  const dur=(3+length*0.17)*m.df*dMul*tDurMul;
  const tot=cityPop+subPop;
  const di=Math.min(5,Math.max(1,Math.round(tot/600000)+1));
  const densM=[0,.35,.58,1.0,1.50,2.0][di];
  const tElast=fare==='free'?1.38:Math.max(.2,1-(ticket-.4)*.14);
  const fBonus=Math.max(.55,1-(freq-5)*.018);
  const baseR=length*10500*m.rf*densM*tElast*fM2*fBonus*(1+subPop/(tot||1)*0.28)*lines;
  const dailyCap=m.capF*(length/10)*(stations/12)*sMul*lines;
  const euShare=EU_SHARE[funding]||0;
  const years=[];let cumNPV=-capex,capSatYr=null;
  for(let y=0;y<=30;y++){
    const yO=y-dur,ramp=yO<=0?0:Math.min(1,.17+yO*.077);
    const riders=baseR*ramp*Math.pow(1+growth,Math.max(0,yO));
    const cap=dailyCap*(1+y*.009);
    if(!capSatYr&&cap>0&&riders/cap>1)capSatYr=Math.round(y);
    const effT=fare==='free'?0:ticket*Math.pow(1.02,Math.max(0,yO));
    const fareRev=riders*effT*365/1e6;
    const opex=(length*m.opkm+stations*m.opkm*.13)*Math.pow(1.025,Math.max(0,yO))*lines;
    const net=fareRev+opex*subsidy-opex;
    if(yO>0)cumNPV+=net/Math.pow(1+discount,y);
    years.push({y,riders:Math.round(riders),cap:Math.round(cap),fareRev,opex,net,cumNPV});
  }
  const riders=years[30].riders;
  const be=(()=>{for(let i=0;i<years.length;i++)if(years[i].cumNPV>0)return years[i].y;return 99;})();
  const viab=Math.min(100,Math.max(0,18+(years[30].net/capex*1100)+subsidy*44+(euShare*20)));
  const co2=Math.round(riders*.48/1000);
  const cars=Math.round(riders*.13);
  const jpm={metro:520,lrt:260,brt:72,ber:88,commuter:300};
  const jobs=+(length*(jpm[m.id]||250)/1000*lines).toFixed(1);
  const prop=Math.min(28,Math.round(densM*7+(m.id==='metro'?6:3)));
  const tSaved=Math.round(18+length*.9+densM*5);
  const econ=Math.round(riders*tSaved*365*.00013);
  return{capex,dur,capSatYr,riders,annRev:years[30].fareRev,annOpex:years[30].opex,be,npv:cumNPV,cpkm:cpm*fD*sMul*tCostMul,viab,co2,cars,jobs,prop,tSaved,econ,years,dailyCap,euShare,euAmt:capex*euShare,terrain};
}

/* ═══ STEP 4 UI ═══ */
// How many line buttons to show per mode
function maxLinesForMode(m){
  if(!m)return 3;
  if(isSurfaceMode(m))return 8;
  if(m.id==='commuter')return 4;
  return 3;
}

function renderLineCountButtons(){
  const el=G('line-count-btns');if(!el)return;
  const max=maxLinesForMode(selMode);
  el.innerHTML='';
  for(let n=1;n<=max;n++){
    const btn=document.createElement('button');
    const active=numLines===n;
    btn.textContent=n==1?'1 line':n+' lines';
    btn.title=n===1?'Single route':(n<=3?'Add a '+(n===2?'second':'third')+' corridor':n+' routes covering the city');
    btn.style.cssText='padding:4px 11px;border-radius:6px;border:1.5px solid '+(active?'var(--eu)':'var(--line)')+';'
      +'background:'+(active?'var(--eu)':'var(--white)')+';color:'+(active?'#fff':'var(--ink2)')+';'
      +'font-size:11px;font-weight:'+(active?'700':'500')+';cursor:pointer;transition:all .15s;';
    btn.onclick=(()=>{const x=n;return()=>setLinesSlider(x);})();
    el.appendChild(btn);
  }
}

function renderSimModeTabs(){
  G('sim-mode-tabs').innerHTML=MODES.map(m=>`<button class="btn btn-sm ${selMode?.id===m.id?'btn-dark':'btn-light'}" onclick="switchSimMode('${m.id}')" style="${selMode?.id===m.id?'border-bottom:2px solid '+m.color+';':''}">${m.icon} ${m.name}</button>`).join('');
  G('sc-mode-title').textContent=(selMode?.name||'Transit')+' — Policy Levers';
  G('metro-type-block').style.display=selMode?.id==='metro'?'block':'none';
  // Update line manager header
  const nlTitle=G('nl-mode-title'),nlHint=G('nl-mode-hint');
  if(nlTitle&&selMode){
    const isSurf=isSurfaceMode(selMode);
    nlTitle.textContent=selMode.icon+' '+selMode.name+' Lines';
    if(nlHint)nlHint.textContent=isSurf
      ?'Urban lines — set length and reach (city-only or suburb extension) per line'
      :'Configure corridor count and interchange connections';
  }
  // Render correct number of line-count buttons for this mode
  renderLineCountButtons();
}
function switchSimMode(id){
  selMode=MODES.find(m=>m.id===id);
  // Apply mode-aware defaults for line length and line count
  if(selMode){
    const defLen=MODE_LEN_DEFAULTS[selMode.id]||12;
    const sl=G('s-length');if(sl){sl.value=defLen;G('v-length').textContent=defLen+' km';}
    // Clamp numLines to max allowed by new mode
    const maxLines=maxLinesForMode(selMode);
    if(numLines>maxLines){numLines=maxLines;}
    applyModeAwareLength();
  }
  renderSimModeTabs();upd();
}
function setMetroType(t){
  metroType=t;
  ['ug','el'].forEach(x=>{const el=G('mt-'+x);if(el){el.classList.toggle('active',x===(t==='underground'?'ug':'el'));}});
  upd();
}
// Surface (urban) modes — shorter default lines, more lines possible
const SURFACE_MODES=['tram','ebus','hybrid','biogas','trolley','brt'];
// Typical line length defaults per mode category (km)
const MODE_LEN_DEFAULTS={metro:18,lrt:14,tram:8,commuter:30,brt:10,ebus:7,hybrid:7,biogas:7,trolley:8};
const MODE_LEN_MAX={metro:60,lrt:50,tram:25,commuter:80,brt:30,ebus:20,hybrid:20,biogas:20,trolley:25};
const MODE_LEN_MIN={metro:5,lrt:4,tram:2,commuter:10,brt:2,ebus:1,hybrid:1,biogas:1,trolley:2};

let buildStrategy='sim'; // 'sim' = simultaneous, 'seq' = sequential

function isSurfaceMode(m){return m&&SURFACE_MODES.includes(m.id);}

function setBuildStrategy(s){
  buildStrategy=s;
  ['sim','seq'].forEach(x=>{const el=G('bs-'+x);if(el)el.classList.toggle('active',x===s);});
  if(selMode&&selCity)upd();
}

function setLinesSlider(n){
  n=parseInt(n);
  setLines(n);
  const sl=G('s-lines');if(sl)sl.value=n;
  // Sync netState lines count to match slider
  if(netState&&netState.lines){
    while(netState.lines.length<n)addNetLine();
    while(netState.lines.length>n&&n>0)netState.lines.pop();
    if(netState.lines.length!==n)renderLineManager();
  }
}

function setLines(n){
  numLines=n;
  // Update slider if it exists
  const sl=G('s-lines');if(sl&&parseInt(sl.value)!==n)sl.value=n;
  // Update old ln-x buttons (legacy compat)
  [1,2,3].forEach(x=>{const el=G('ln-'+x);if(el)el.classList.toggle('active',x===n);});
  // Show/hide build strategy block
  const bsBlock=G('build-strategy-block');
  if(bsBlock)bsBlock.style.display=n>1?'block':'none';
  // Label
  const vl=G('v-lines');if(vl)vl.textContent=n+' line'+(n>1?'s':'');
  // Re-render buttons so active state updates
  renderLineCountButtons();
  // Line-count hint
  const hint=G('line-count-hint');
  if(hint){
    const isSurf=isSurfaceMode(selMode);
    if(isSurf&&n>1)hint.textContent=n>4?'Extensive urban network — simulates full city coverage':'Urban network — lines cover city corridors';
    else if(!isSurf&&n>1)hint.textContent=n>2?'Multi-corridor rail network':'Second line builds metro/LRT cross-network';
    else hint.textContent='Single route — start small, expand later';
  }
  // Note
  const note=G('line-note');
  if(note){
    if(n>1&&buildStrategy==='sim'){
      const costMul=(1+(n-1)*0.80).toFixed(2);
      note.style.display='block';note.style.background='var(--amber-bg)';note.style.color='var(--amber)';
      note.textContent='⚠️ '+n+' simultaneous lines ≈ '+Math.round((1+(n-1)*0.80)*100)+'% of single-line cost. All lines open together — higher upfront investment, maximum network effect.';
    } else if(n>1&&buildStrategy==='seq'){
      note.style.display='block';note.style.background='var(--blue-bg)';note.style.color='var(--blue)';
      note.textContent='ℹ️ Sequential build: each line opens before the next starts construction. Lower risk, more manageable funding, but network completes later.';
    } else {
      note.style.display='none';
    }
  }
  netState.buildMode=n;
  netState.initialized=false;
  netState.modeId=null;
  // Apply mode-aware length guidance
  applyModeAwareLength();
  if(selMode&&selCity)upd();
}

function applyModeAwareLength(){
  if(!selMode)return;
  const m=selMode;
  const isSurf=isSurfaceMode(m);
  const lenSlider=G('s-length');
  const minLbl=G('len-min-lbl'),maxLbl=G('len-max-lbl');
  const guide=G('length-guidance');
  const minLen=MODE_LEN_MIN[m.id]||2;
  const maxLen=MODE_LEN_MAX[m.id]||60;
  const defLen=MODE_LEN_DEFAULTS[m.id]||12;
  if(lenSlider){
    lenSlider.min=minLen;lenSlider.max=maxLen;
    if(parseFloat(lenSlider.value)>maxLen)lenSlider.value=defLen;
    if(parseFloat(lenSlider.value)<minLen)lenSlider.value=defLen;
  }
  if(minLbl)minLbl.textContent=minLen+' km';
  if(maxLbl)maxLbl.textContent=maxLen+' km';
  if(guide){
    if(isSurf){
      const cityKm=Math.round((selCity?.pop||300000)/50000*1.5+4);
      const suburbNote=numLines>2?' Additional lines can extend to suburbs.':'';
      guide.style.display='block';
      guide.innerHTML='🏙️ <strong>Urban mode:</strong> Typical line length for '+m.name+' is <strong>'+defLen+'–'+Math.min(defLen+5,maxLen)+' km</strong> within city limits.'+suburbNote+' Extend slider beyond '+Math.round(maxLen*0.7)+' km to reach suburbs.';
    } else {
      guide.style.display='none';
    }
  }
}
function updEuUI(funding,capex){
  const ef=EU_FUNDS[funding];
  G('eu-fund-info').style.display=ef?'block':'none';
  G('eu-breakdown').style.display=ef?'block':'none';
  if(!ef)return;
  G('eu-fund-title').textContent=ef.name;G('eu-fund-desc').textContent=ef.desc;G('eu-fund-pct').textContent=Math.round(ef.pct*100)+'%';
  const euA=capex*ef.pct,natA=capex*(1-ef.pct);
  G('eu-fund-rows').innerHTML=[{n:'EU contribution',a:euA,p:ef.pct,col:ef.col},{n:'National / local match',a:natA,p:1-ef.pct,col:'rgba(255,255,255,.3)'}].map(r=>`<div class="eu-fund-row"><div class="eu-fund-name">${r.n}</div><div class="eu-fund-track"><div class="eu-fund-fill" style="width:${Math.round(r.p*100)}%;background:${r.n.startsWith('EU')?'var(--eu-gold)':r.col}">${Math.round(r.p*100)}%</div></div><div class="eu-fund-val">${fE(r.a)}</div></div>`).join('');
}

function upd(){
  if(!selMode||!selCity)return;
  const m=selMode;
  applyModeAwareLength();
  const ticket=gv('s-ticket'),subsidy=gv('s-sub')/100,length=gv('s-length');
  const stations=gi('s-stations'),speed=gi('s-speed'),freq=gv('s-freq');
  const funding=G('s-fund').value,fare=G('s-fare').value,growth=gv('s-growth')/100;
  G('v-ticket').textContent=fare==='free'?'Free':'€'+ticket.toFixed(2);
  G('v-sub').textContent=Math.round(subsidy*100)+'%';G('v-length').textContent=length+' km';
  G('v-stations').textContent=stations;G('v-freq').textContent='Every '+freq+' min';
  G('v-growth').textContent=(growth*100).toFixed(1)+'%/yr';G('v-speed').textContent=SPD[speed];
  const effectiveLines=numLines; // all lines count; lineFactor in qcalc handles cost scaling
  const r=qcalc(m,selCity.pop,suburbPop(),ticket,subsidy,length,stations,speed,freq,funding,fare,0.04,growth,metroType,effectiveLines);
  lastCalc={r,m,params:{ticket,subsidy,length,stations,speed,freq,funding,fare,growth,metroType,numLines}};
  G('k-cost').textContent=fE(r.capex);
  const tInfo=r.terrain||TERRAIN_TYPES[0];
  const terrPct=Math.round((tInfo.costMul-1)*100);
  G('k-perkm').textContent='€'+Math.round(r.cpkm)+'M/km'+(numLines===2?' · 2 lines':'')+(terrPct>0?' · '+tInfo.icon+' +'+terrPct+'% terrain':'');
  G('k-eu').textContent=r.euAmt>0?fE(r.euAmt):'€0';G('k-eu-lbl').textContent=r.euShare>0?Math.round(r.euShare*100)+'% of total capex':'No EU co-funding';
  G('k-riders').textContent=fPF(r.riders);G('k-riders-sub').textContent='at maturity'+(numLines===2?' (both lines)':'');
  G('k-dur').textContent=r.dur.toFixed(1)+' yr';G('k-open-yr').textContent='Opens ~'+(2025+Math.ceil(r.dur));
  G('k-be').textContent=r.be>=99?'>30 yr':r.be+' yr';G('k-be').className='kpi-val '+(r.be<15?'cv-green':r.be<25?'cv-amber':'cv-red');
  G('k-rev').textContent=fE(r.annRev);G('k-opex').textContent=fE(r.annOpex);
  G('k-viab').textContent=Math.round(r.viab)+'%';G('k-viab').className='kpi-val '+(r.viab>70?'cv-green':r.viab>45?'cv-amber':'cv-red');
  G('k-viab-lbl').textContent=r.viab>70?'Financially sound':r.viab>45?'Needs support':'Challenging viability';
  const euB=r.euShare>0.6?' EU co-funding significantly improves viability.':'';
  let vc,vi,vt,vd;
  if(r.viab>70){vc='good';vi='✅';vt='Project looks viable';vd=`Viability: ${Math.round(r.viab)}%.${euB} Ridership and revenue look healthy for ${m.name}.`;}
  else if(r.viab>45){vc='warn';vi='⚠️';vt='Viable with policy support';vd=`Score: ${Math.round(r.viab)}%.${euB} Consider higher subsidy, EU co-funding, or revised fares.`;}
  else{vc='bad';vi='❌';vt='Financially challenging';vd=`Score: ${Math.round(r.viab)}%. Try EU co-funding (Cohesion Fund), higher subsidy, or a more affordable mode like Tram, Electric Bus or Trolleybus.`;}
  G('verdict').className='verdict '+vc;G('verdict').querySelector('.v-icon').textContent=vi;G('v-title').textContent=vt;G('v-desc').textContent=vd;
  const cw=G('cap-warn');if(r.capSatYr){G('cap-yr').textContent=r.capSatYr;cw.classList.add('show');}else cw.classList.remove('show');
  updEuUI(funding,r.capex);
  // Basic impacts
  G('i-co2').textContent=(r.co2*1000).toLocaleString()+' t';G('i-cars').textContent=r.cars.toLocaleString();
  G('i-jobs').textContent=(r.jobs*1000).toLocaleString();G('i-prop').textContent='+'+r.prop+'%';
  G('i-time').textContent=r.tSaved+' min/day';G('i-econ').textContent=fE(r.econ);
  // New impacts
  G('i-health').textContent=fE(r.co2*1000*0.18/1e6); // health cost of air pollution saved
  G('i-access').textContent=Math.round(r.riders*0.08).toLocaleString();
  G('i-co2life').textContent=(r.co2*1000*30/1000).toFixed(0)+'K t';
  // Extra mini KPIs
  G('k2-cpkm').textContent='€'+Math.round(r.cpkm)+'M/km';
  const cpr=r.annOpex/Math.max(1,r.riders/1000);G('k2-cpr').textContent='€'+cpr.toFixed(0)+'/yr';
  const subAmt=r.annOpex*(subsidy);const tripsYr=r.riders*365;const spt=tripsYr>0?subAmt*1e6/tripsYr:0;
  G('k2-spt').textContent=spt<0.01?'<1¢':'€'+spt.toFixed(2);G('k2-spt').className='kpi-val '+(spt<0.5?'cv-green':spt<2?'cv-amber':'cv-red');
  const rr=r.annOpex>0?r.annRev/r.annOpex:0;G('k2-rr').textContent=(rr*100).toFixed(0)+'%';G('k2-rr').className='kpi-val '+(rr>0.7?'cv-green':rr>0.4?'cv-amber':'cv-red');
  const bcr=r.capex>0?(r.econ/1e6+r.npv)/(r.capex):0;G('k2-bcr').textContent=bcr.toFixed(2)+'x';G('k2-bcr').className='kpi-val '+(bcr>1?'cv-green':bcr>0.5?'cv-amber':'cv-red');
  // Milestones
  const yr0=2025;
  G('ms-approval').textContent=yr0;
  G('ms-works').textContent=yr0+1;
  G('ms-open').textContent=yr0+Math.ceil(r.dur);
  G('ms-be').textContent=r.be>=99?'>2055':(yr0+Math.ceil(r.dur)+r.be);
  G('ms-mature').textContent=yr0+Math.ceil(r.dur)+8;
  // Plain language summary
  updPlain(r,m,ticket,subsidy,length,stations,funding,fare,growth);
  // Network line manager
  renderLineManager();
  const stratLabel=numLines===2?' — both lines built at the same time (more expensive but opens together)':numLines===3?' — Line 2 starts only after Line 1 is running':'';
  G('gantt-total').textContent='Total construction time: '+r.dur.toFixed(1)+' years'+stratLabel;
  const phCols=['#3b5bdb','#1c7ed6','#0ca678','#f59f00','#f03e3e'];
  const phDescs={
    'Planning & DEIA':       'Detailed design, environmental impact assessment (DEIA), public consultations and formal sign-off from city and national authorities. No digging yet.',
    'Planning & permits':    'Surveying the route, applying for planning permits, holding public hearings and responding to objections. No physical work on site yet.',
    'Planning':              'Finalising the route design, obtaining planning permission and securing political approval to proceed.',
    'Planning & feasibility':'Commissioning feasibility studies, preparing business cases and applying for EU or national funding. A go/no-go decision point.',
    'Land acquisition':      'Purchasing or leasing every plot of land and property along the route. Can be slow and expensive in dense urban areas — residents and businesses may challenge compulsory purchases in court.',
    'Environmental review':  'Independent assessment of how the project affects air quality, noise, wildlife, water and historic buildings. Required by EU law before construction can start.',
    'Environmental impact':  'Statutory environmental impact study covering habitats, flood risk, noise and air quality. Results are published for public comment before construction is approved.',
    'Civil works':           'The biggest phase: excavating tunnels, building viaducts and bridges, laying foundations, constructing stations and pouring concrete. The most expensive and most visible part.',
    'Track & civil works':   'Laying the track, constructing stations, building bridges or cuttings and completing all groundworks along the route.',
    'Track & civil':         'Road modifications, track-laying and building station foundations. The main physical construction on the street.',
    'Lane & road works':     'Creating dedicated transit lanes, upgrading junctions, relocating utilities underground and resurfacing roads along the corridor.',
    'Site prep':             'Clearing the ground, relocating underground pipes and cables, setting up site compounds and access roads. Prepares the route so heavy construction machinery can move in safely.',
    'Depot & grid upgrade':  'Building the vehicle depot (where buses or trams are stored, cleaned and maintained overnight) and upgrading the electricity grid to supply charging points or overhead wires.',
    'Road works':            'Upgrading roads, pavements and junctions along the route to accommodate the new vehicles and passenger flows.',
    'Systems & rolling stock':'Installing all the technology that makes the system run: signalling, passenger information screens, ticketing gates, CCTV and control room — plus manufacturing and delivering the trains or buses.',
    'Systems & electrification':'Erecting overhead wires or third rail, installing substations and connecting the power supply. Without this, electric vehicles cannot run.',
    'Systems':               'Setting up signalling, IT systems, real-time passenger information and the control room from which operators manage the whole network.',
    'Stations & tech':       'Fitting out station interiors: platforms, lifts, escalators, ticket machines, signage, lighting, security cameras and passenger information screens. Also installing onboard technology in vehicles.',
    'Charging infra':        'Installing charging equipment at terminals, stops and the depot so electric buses can recharge between runs without going out of service.',
    'Testing & safety':      'Running vehicles without passengers to test every system — brakes, doors, signals, communications. Regulators inspect the line and issue a safety certificate before public opening.',
    'Commissioning':         'Final checks, staff training on live equipment, a soft-launch period with limited services, and the formal handover from contractor to operator.',
    'Testing':               'Trial runs to check that vehicles, track, signals and stations all work together reliably. Staff learn the route and emergency procedures before the first passenger boards.',
    'Depot upgrade':         'Upgrading the existing bus depot with new maintenance equipment, washing facilities and workshop space to handle the new fleet type.',
    'Fleet delivery':        'Manufacturing and delivering the vehicles. Includes factory acceptance tests, driver training and commissioning individual units into service.',
    'Depot & fuel infra':    'Building or upgrading the depot and installing dedicated fuel infrastructure — CNG/biomethane filling stations for biogas buses, or high-power chargers for electric fleets.',
    'Wire & substation works':'Installing the overhead contact wire system (catenary), traction substations and feeder cables along the full route. The most visible element of a trolleybus network.',
  };
  let cum=0;
  G('gantt-rows').innerHTML=m.phases.map((ph,i)=>{
    const d=(r.dur*m.pp[i]/100).toFixed(1);
    const desc=phDescs[ph]||'';
    const h=`<div class="g-row" title="${desc}" style="cursor:help">
      <div class="g-lbl" style="font-size:9px;line-height:1.3;white-space:normal">${ph}</div>
      <div class="g-track">
        <div class="g-bar" style="left:${cum}%;width:${m.pp[i]}%;background:${phCols[i]}">
          <span>${d}y</span>
        </div>
      </div>
      <div class="g-dur">${d}y</div>
    </div>`;
    cum+=m.pp[i];return h;
  }).join('');
  G('gantt-ticks').innerHTML=[0,.25,.5,.75,1].map(t=>`<span>${t===0?'Start':t===1?'Opens':'Y'+(r.dur*t).toFixed(1)}</span>`).join('');
  G('gantt-phase-legend').innerHTML=m.phases.map((ph,i)=>{
    const desc=phDescs[ph]||'No description available.';
    const d=(r.dur*m.pp[i]/100).toFixed(1);
    const pct=m.pp[i];
    return`<div style="border:1px solid var(--line);border-radius:9px;padding:9px 12px;background:var(--white);display:flex;gap:10px;align-items:flex-start;margin-bottom:6px">
      <div style="width:14px;height:14px;border-radius:4px;background:${phCols[i]};flex-shrink:0;margin-top:1px"></div>
      <div style="flex:1;min-width:0">
        <div style="display:flex;align-items:center;gap:6px;flex-wrap:wrap;margin-bottom:2px">
          <span style="font-size:11px;font-weight:700;color:${phCols[i]}">${ph}</span>
          <span style="font-size:9px;background:${phCols[i]}22;color:${phCols[i]};padding:1px 7px;border-radius:8px;font-weight:600">${d} years · ${pct}% of total</span>
        </div>
        <div style="font-size:11px;color:var(--ink2);line-height:1.5">${desc}</div>
      </div>
    </div>`;
  }).join('');
  drawNetwork(m,length,stations);drawDemand(r,m);drawCashflow(r);drawNPVChart(r);drawSensitivity(r);drawRisk(r,m,{ticket,subsidy,length,stations,funding,fare,growth,metroType,numLines});
  if(scenarios.length>=2)renderCmpPanel();
}

/* ═══ INTERACTIVE NETWORK EDITOR ═══ */

const netState = {
  lines:[],buildMode:1,dragNode:null,dragOffset:{x:0,y:0},
  initialized:false,modeId:null,stCnt:0,
  tool:'select',extendLine:null,newLineStart:null,
  hoveredNode:null,scope:'city', // 'city' | 'suburbs'
  seqPhase:1, // which sequential phase is currently active/complete (1..N)
};
let _netW=0,_netH=0;

// ── scope toggle ──────────────────────────────────────────────
function setScope(s){
  netState.scope=s;
  ['city','suburbs'].forEach(x=>{const el=G('scope-'+x);if(el)el.classList.toggle('active',x===s);});
  redrawNet();
}

// ── tool select ───────────────────────────────────────────────
function setTool(t){
  netState.tool=t;netState.extendLine=null;netState.newLineStart=null;
  ['select','addst','addline','extend','delete'].forEach(x=>{
    const el=G('tool-'+x);if(el)el.classList.toggle('active',x===t);
  });
  const cv=G('c-network');
  if(cv)cv.style.cursor=t==='select'?'default':'crosshair';
  redrawNet();
}

// ── sequential phase progress ─────────────────────────────────
function renderSeqProgress(){
  const bar=G('seq-progress-bar');
  if(!bar)return;
  if(netState.buildMode!==3){bar.style.display='none';return;}
  bar.style.display='block';
  const phases=netState.lines.map((ln,i)=>({
    label:'Line '+(i+1),sub:ln.seqStatus==='open'?'✅ Open':ln.seqStatus==='construction'?'🔨 Building':'📋 Planned',
    status:ln.seqStatus||'planned',id:ln.id
  }));
  G('seq-phases').innerHTML=phases.map((ph,i)=>`
    <div class="seq-phase ${ph.status==='open'?'done':ph.status==='construction'?'active':'planned'}"
         onclick="advanceSeqPhase('${ph.id}')" title="Click to advance this line's status">
      <span class="sp-label">${ph.label}</span>
      <span class="sp-sub">${ph.sub}</span>
      <span class="sp-check">${ph.status==='open'?'✓':ph.status==='construction'?'→':''}</span>
    </div>`).join('');
}
function advanceSeqPhase(lineId){
  const ln=netState.lines.find(l=>l.id===lineId);
  if(!ln)return;
  const cycle={planned:'construction',construction:'open',open:'planned'};
  ln.seqStatus=cycle[ln.seqStatus||'planned'];
  ln.label=ln.baseLabel+(ln.seqStatus==='planned'?' (planned)':ln.seqStatus==='construction'?' (under construction)':'');
  renderSeqProgress();renderLineManager();redrawNet();
  toast(`${ln.baseLabel}: ${ln.seqStatus}`);
}

// ── line manager ──────────────────────────────────────────────
const LINE_STATUS_OPTS=['open','construction','planned'];
const LINE_STATUS_LABELS={open:'✅ Open',construction:'🔨 Building',planned:'📋 Planned'};
function renderLineManager(){
  const el=G('nl-lines-list');if(!el)return;
  if(!netState.lines||netState.lines.length===0){
    el.innerHTML='<div style="padding:10px;font-size:12px;color:var(--ink3);font-style:italic">No lines yet — pick a strategy above.</div>';
    return;
  }
  const isSurf=isSurfaceMode(selMode);
  el.innerHTML=netState.lines.map((ln,i)=>{
    const statusOpts=LINE_STATUS_OPTS.map(s=>`<option value="${s}" ${(ln.seqStatus||'open')===s?'selected':''}>${LINE_STATUS_LABELS[s]}</option>`).join('');
    const removeBtn=`<button class="nl-btn danger" onclick="removeNetLine('${ln.id}')" title="Delete this line">✕</button>`;
    const scope=ln.scope||'city';
    const lineLen=ln.lineLen||(selMode?MODE_LEN_DEFAULTS[selMode.id]:10)||10;
    const maxLen=selMode?MODE_LEN_MAX[selMode.id]:60;
    const minLen=selMode?MODE_LEN_MIN[selMode.id]:2;
    const scopeIcon=scope==='suburb'?'🌆':'🏙️';
    const scopeLabel=scope==='suburb'?'City + suburbs':'City only';
    // Compute effective length for this line
    const effLen=scope==='suburb'?Math.min(maxLen,Math.round(lineLen*1.6)):lineLen;
    return `<div class="nl-row" style="flex-wrap:wrap;gap:5px;border:1px solid var(--line);border-radius:8px;padding:8px 10px;background:var(--cream)">
      <div style="display:flex;align-items:center;gap:6px;width:100%">
        <div style="width:12px;height:12px;border-radius:3px;background:${ln.col};flex-shrink:0"></div>
        <input type="text" value="${ln.label.replace(/\s*\(.*\)$/,'')}" onchange="renameNetLine(${i},this.value)" style="width:80px;font-size:11px;font-weight:600">
        <select onchange="setLineStatus('${ln.id}',this.value)" style="font-size:10px">${statusOpts}</select>
        ${removeBtn}
      </div>
      ${isSurf?`
      <div style="display:flex;align-items:center;gap:6px;width:100%;margin-top:3px">
        <span style="font-size:10px;color:var(--ink3);flex-shrink:0">Length:</span>
        <input type="range" min="${minLen}" max="${maxLen}" value="${lineLen}" step="1"
          oninput="setLineLen('${ln.id}',this.value,this)" style="flex:1;height:3px">
        <span class="ll-val-${ln.id}" style="font-size:10px;font-weight:700;color:var(--ink2);min-width:32px">${lineLen} km</span>
      </div>
      <div style="display:flex;align-items:center;gap:5px;width:100%;margin-top:2px">
        <button onclick="setLineScope('${ln.id}','city')" style="font-size:9px;padding:2px 7px;border-radius:5px;border:1px solid var(--line);background:${scope==='city'?'var(--blue)':'var(--cream)'};color:${scope==='city'?'#fff':'var(--ink3)'};cursor:pointer">🏙️ City only</button>
        <button onclick="setLineScope('${ln.id}','suburb')" style="font-size:9px;padding:2px 7px;border-radius:5px;border:1px solid var(--line);background:${scope==='suburb'?'var(--green)':'var(--cream)'};color:${scope==='suburb'?'#fff':'var(--ink3)'};cursor:pointer">🌆 Extend to suburbs</button>
        <span style="font-size:9px;color:var(--ink3);margin-left:4px">→ <strong>${effLen} km</strong> effective</span>
      </div>`:
      `<div style="font-size:10px;color:var(--ink3)">
        <select onchange="setLineIntercon('${ln.id}',this.value)" style="font-size:10px">
          <option value="interconnected" ${ln.intercon!=='separate'?'selected':''}>🔗 Interchange</option>
          <option value="separate" ${ln.intercon==='separate'?'selected':''}>━ Separate</option>
        </select>
        <span style="margin-left:6px">${ln.nodes?ln.nodes.length+' stops':''}</span>
      </div>`}
    </div>`;
  }).join('');
  el.innerHTML+=`<button class="add-line-btn" onclick="addNetLine()">＋ Add line</button>`;
  renderSeqProgress();
}
function renameNetLine(i,name){
  if(netState.lines[i]){netState.lines[i].baseLabel=name;netState.lines[i].label=name;}
  redrawNet();
}
function setLineStatus(id,status){
  const ln=netState.lines.find(l=>l.id===id);
  if(!ln)return;
  ln.seqStatus=status;
  ln.label=(ln.baseLabel||ln.label.replace(/\s*\(.*\)$/,''))+(status==='planned'?' (planned)':status==='construction'?' (under construction)':'');
  renderSeqProgress();renderLineManager();redrawNet();
}
function setLineIntercon(id,val){
  const ln=netState.lines.find(l=>l.id===id);if(ln){ln.intercon=val;redrawNet();}
}
function removeNetLine(id){
  netState.lines=netState.lines.filter(l=>l.id!==id);
  renderLineManager();redrawNet();updFromNetwork();toast('Line removed — graphs updated');
}
function addNetLine(){
  const idx=netState.lines.length;
  const col=LINE_COLS[idx%LINE_COLS.length];
  const id='L'+(idx+1);
  const W=getNetW()||700,H=_netH||460;
  const angle=Math.PI*(0.25+idx*0.18);
  const cx=W*0.5,cy=H*0.5,len=Math.min(W,H)*0.38;
  const nodes=[];
  for(let s=0;s<8;s++){
    const t=s/7-0.5;
    nodes.push({
      id:id+'_'+s,
      x:Math.round(cx+Math.cos(angle)*len*t+Math.sin(angle)*len*t*0.2),
      y:Math.round(cy+Math.sin(angle)*len*t-Math.cos(angle)*len*t*0.2),
      name:s===0?'Terminus A':s===7?'Terminus B':'Stop '+(s),
      isEnd:s===0||s===7
    });
  }
  const lbl='Line '+(idx+1);
  // Determine default scope: urban modes start inside city, can extend
  const isSurf=isSurfaceMode(selMode);
  const defLen=selMode?Math.max(MODE_LEN_MIN[selMode.id]||2, MODE_LEN_DEFAULTS[selMode.id]||10):10;
  const scope=idx===0?'city':'city'; // first lines are urban; user can change to suburb
  netState.lines.push({id,col,label:lbl,baseLabel:lbl,nodes,seqStatus:'planned',intercon:'interconnected',seqPhase:idx+1,scope,lineLen:defLen});
  // Sync numLines slider
  numLines=netState.lines.length;
  const sl=G('s-lines');if(sl){sl.value=numLines;G('v-lines').textContent=numLines+' line'+(numLines>1?'s':'');}
  renderLineManager();redrawNet();updFromNetwork();toast(lbl+' added');
}
function setLineLen(id,val,el){
  const ln=netState.lines.find(l=>l.id===id);if(!ln)return;
  ln.lineLen=parseInt(val);
  const vEl=document.querySelector('.ll-val-'+id);if(vEl)vEl.textContent=val+' km';
  updFromNetwork();
}
function setLineScope(id,scope){
  const ln=netState.lines.find(l=>l.id===id);if(!ln)return;
  ln.scope=scope;
  renderLineManager();updFromNetwork();
}

// ── build default network ─────────────────────────────────────
function buildDefaultNetwork(m,length,stations,lnCount){
  const cv=G('c-network');if(!cv)return;
  const W=getNetW(),H=460;
  if(W<50){return;}
  _netW=W;_netH=H;
  const p=(fx,fy)=>({x:Math.round(fx*W),y:Math.round(fy*H)});
  const stCnt=Math.max(3,Math.round(stations));
  const mid=m.id;

  const geo1={
    metro:   [p(.05,.68),p(.18,.57),p(.32,.47),p(.46,.40),p(.60,.36),p(.74,.31),p(.88,.26),p(.96,.22)],
    lrt:     [p(.05,.72),p(.20,.58),p(.35,.47),p(.50,.40),p(.65,.37),p(.80,.33),p(.95,.28)],
    brt:     [p(.05,.66),p(.22,.55),p(.40,.47),p(.55,.43),p(.70,.40),p(.85,.37),p(.96,.33)],
    ber:     [p(.05,.64),p(.23,.54),p(.41,.46),p(.56,.42),p(.71,.39),p(.86,.36),p(.96,.33)],
    commuter:[p(.05,.26),p(.18,.27),p(.32,.33),p(.47,.40),p(.62,.40),p(.76,.34),p(.90,.26),p(.96,.20)],
  };
  const geo2a={
    metro:   [p(.05,.20),p(.17,.27),p(.30,.35),p(.44,.44),p(.58,.53),p(.72,.60),p(.86,.67),p(.96,.73)],
    lrt:     [p(.05,.18),p(.19,.27),p(.33,.36),p(.46,.44),p(.60,.52),p(.74,.59),p(.96,.68)],
    brt:     [p(.05,.20),p(.22,.29),p(.37,.37),p(.50,.44),p(.63,.51),p(.78,.58),p(.96,.65)],
    ber:     [p(.05,.22),p(.22,.30),p(.37,.38),p(.50,.44),p(.63,.50),p(.78,.57),p(.96,.63)],
    commuter:[p(.05,.14),p(.17,.20),p(.30,.28),p(.44,.38),p(.58,.44),p(.72,.52),p(.88,.62),p(.96,.70)],
  };
  const geo2b={
    metro:   [p(.05,.78),p(.17,.70),p(.30,.61),p(.44,.44),p(.58,.34),p(.72,.26),p(.86,.18),p(.96,.12)],
    lrt:     [p(.05,.80),p(.19,.70),p(.33,.60),p(.46,.44),p(.60,.34),p(.74,.25),p(.96,.16)],
    brt:     [p(.05,.76),p(.22,.66),p(.37,.57),p(.50,.44),p(.63,.36),p(.78,.27),p(.96,.18)],
    ber:     [p(.05,.74),p(.22,.65),p(.37,.56),p(.50,.44),p(.63,.36),p(.78,.28),p(.96,.20)],
    commuter:[p(.05,.84),p(.17,.74),p(.30,.62),p(.44,.44),p(.58,.33),p(.72,.24),p(.88,.15),p(.96,.10)],
  };

  function nodesAlongPath(waypts,count,lineId){
    let segs=[],total=0;
    for(let i=1;i<waypts.length;i++){
      const dx=waypts[i].x-waypts[i-1].x,dy=waypts[i].y-waypts[i-1].y,l=Math.sqrt(dx*dx+dy*dy);
      segs.push({x0:waypts[i-1].x,y0:waypts[i-1].y,dx,dy,l});total+=l;
    }
    const nodes=[];
    for(let s=0;s<count;s++){
      const t=count===1?0.5:s/(count-1);
      let rem=t*total,pt=null;
      for(const sg of segs){if(rem<=sg.l){const r=rem/sg.l;pt={x:sg.x0+r*sg.dx,y:sg.y0+r*sg.dy};break;}rem-=sg.l;}
      if(!pt){const sg=segs[segs.length-1];pt={x:sg.x0+sg.dx,y:sg.y0+sg.dy};}
      const isEnd=s===0||s===count-1;
      nodes.push({id:lineId+'_'+s,x:Math.round(pt.x),y:Math.round(pt.y),
        name:isEnd?(s===0?'Terminus A':'Terminus B'):'Stop '+(s),isEnd});
    }
    return nodes;
  }

  netState.lines=[];
  if(lnCount===1){
    const w=geo1[mid]||geo1.metro;
    netState.lines.push({id:'L1',col:LINE_COLS[0],label:'Line 1',baseLabel:'Line 1',waypts:w,nodes:nodesAlongPath(w,stCnt,'L1'),seqStatus:'open',intercon:'interconnected',seqPhase:1});
  } else if(lnCount===2){
    const w1=geo2a[mid]||geo2a.metro,w2=geo2b[mid]||geo2b.metro;
    netState.lines.push({id:'L1',col:LINE_COLS[0],label:'Line 1',baseLabel:'Line 1',waypts:w1,nodes:nodesAlongPath(w1,stCnt,'L1'),seqStatus:'open',intercon:'interconnected',seqPhase:1});
    netState.lines.push({id:'L2',col:LINE_COLS[1],label:'Line 2',baseLabel:'Line 2',waypts:w2,nodes:nodesAlongPath(w2,stCnt,'L2'),seqStatus:'open',intercon:'interconnected',seqPhase:1});
  } else if(lnCount===3){
    const w1=geo2a[mid]||geo2a.metro,w2=geo2b[mid]||geo2b.metro;
    netState.lines.push({id:'L1',col:LINE_COLS[0],label:'Line 1',baseLabel:'Line 1',waypts:w1,nodes:nodesAlongPath(w1,stCnt,'L1'),seqStatus:'open',intercon:'interconnected',seqPhase:1});
    netState.lines.push({id:'L2',col:LINE_COLS[1],label:'Line 2 (planned)',baseLabel:'Line 2',waypts:w2,nodes:nodesAlongPath(w2,stCnt,'L2'),seqStatus:'planned',intercon:'interconnected',seqPhase:2});
  }
  netState.initialized=true;
  netState.modeId=m.id;
  renderLineManager();
}

function resetNetwork(){
  netState.initialized=false;netState.modeId=null;
  if(selMode&&selCity)upd();else redrawNet();
}
function getNetW(){
  const cv=G('c-network');if(!cv)return 700;
  return cv.clientWidth||cv.offsetWidth||cv.parentElement?.clientWidth||700;
}
function drawNetwork(m,length,stations){
  const lnCount=numLines;
  const needRebuild=!netState.initialized||netState.modeId!==m.id||netState.buildMode!==lnCount||netState.stCnt!==Math.round(stations);
  if(needRebuild){
    netState.buildMode=lnCount;netState.stCnt=Math.round(stations);
    initNetCanvas();
    const tryBuild=()=>{if(getNetW()<50){requestAnimationFrame(tryBuild);return;}buildDefaultNetwork(m,length,stations,lnCount);redrawNet();};
    tryBuild();
  } else {initNetCanvas();redrawNet();}
}

// ── canvas events ─────────────────────────────────────────────
function initNetCanvas(){
  const cv=G('c-network');if(!cv||cv._netInit)return;
  cv._netInit=true;
  function getPos(e){
    const r=cv.getBoundingClientRect();
    return{x:(e.clientX!=null?e.clientX:e.touches?.[0]?.clientX||0)-r.left,
           y:(e.clientY!=null?e.clientY:e.touches?.[0]?.clientY||0)-r.top};
  }
  function hitNode(pos,rad=14){
    for(const ln of netState.lines)for(const nd of ln.nodes)
      if(Math.hypot(nd.x-pos.x,nd.y-pos.y)<rad)return{node:nd,line:ln};
    return null;
  }
  function hitSeg(pos,thresh=9){
    for(const ln of netState.lines){
      const nds=ln.nodes;
      for(let i=0;i<nds.length-1;i++){
        const ax=nds[i].x,ay=nds[i].y,bx=nds[i+1].x,by=nds[i+1].y;
        const dx=bx-ax,dy=by-ay,len2=dx*dx+dy*dy;if(!len2)continue;
        const t=Math.max(0,Math.min(1,((pos.x-ax)*dx+(pos.y-ay)*dy)/len2));
        const px=ax+t*dx,py=ay+t*dy;
        if(Math.hypot(pos.x-px,pos.y-py)<thresh)return{line:ln,segIdx:i,insertX:Math.round(px),insertY:Math.round(py)};
      }
    }
    return null;
  }
  cv.addEventListener('mousedown',e=>{
    const pos=getPos(e),tool=netState.tool;
    if(tool==='select'||tool==='delete'){
      const hit=hitNode(pos);
      if(hit){
        if(tool==='delete'&&!hit.node.isEnd){
          hit.line.nodes=hit.line.nodes.filter(n=>n.id!==hit.node.id);
          renumberNodes(hit.line);renderLineManager();redrawNet();updFromNetwork();
        } else if(tool==='select'){
          netState.dragNode={node:hit.node,line:hit.line};
          netState.dragOffset={x:pos.x-hit.node.x,y:pos.y-hit.node.y};
          cv.style.cursor='grabbing';
        }
      }
    } else if(tool==='addst'){
      const seg=hitSeg(pos);
      if(seg){
        const nd={id:seg.line.id+'_i'+Date.now(),x:seg.insertX,y:seg.insertY,name:'Stop X',isEnd:false};
        seg.line.nodes.splice(seg.segIdx+1,0,nd);renumberNodes(seg.line);renderLineManager();redrawNet();updFromNetwork();
      }
    } else if(tool==='addline'){
      // Click first point of a brand-new line
      if(!netState.newLineStart){
        netState.newLineStart={x:pos.x,y:pos.y};
        toast('Click second point to draw the new line');
        redrawNet();
      } else {
        const st=netState.newLineStart;netState.newLineStart=null;
        const idx=netState.lines.length;
        const id='L'+(idx+1);const lbl='Line '+(idx+1);
        const dx=pos.x-st.x,dy=pos.y-st.y,len=Math.sqrt(dx*dx+dy*dy)||1;
        const nodes=[];
        for(let s=0;s<8;s++){const t=s/7;nodes.push({id:id+'_'+s,x:Math.round(st.x+t*dx),y:Math.round(st.y+t*dy),name:s===0?'Terminus A':s===7?'Terminus B':'Stop '+s,isEnd:s===0||s===7});}
        // Detect if this new line crosses any existing line → inherit its color
        let col=LINE_COLS[idx%LINE_COLS.length];
        for(const existing of netState.lines){
          const cr=findCrossings(nodes,existing.nodes);
          if(cr.length>0){col=existing.col;break;}
        }
        netState.lines.push({id,col,label:lbl,baseLabel:lbl,nodes,seqStatus:'planned',intercon:'interconnected',seqPhase:idx+1});
        renderLineManager();redrawNet();updFromNetwork();toast(lbl+' drawn! Graphs updated. Switch to Select to reposition stops.');
      }
    } else if(tool==='extend'){
      const hit=hitNode(pos,20);
      if(hit&&hit.node.isEnd){
        netState.extendLine={line:hit.line,endNode:hit.node,mouseX:pos.x,mouseY:pos.y};
        cv.addEventListener('mousemove',onExtMove);cv.addEventListener('mouseup',onExtUp,{once:true});
      }
    }
  });
  cv.addEventListener('mousemove',e=>{
    const pos=getPos(e);
    if(netState.dragNode){
      const nd=netState.dragNode.node;
      nd.x=Math.max(8,Math.min(_netW-8,Math.round(pos.x-netState.dragOffset.x)));
      nd.y=Math.max(8,Math.min(_netH-8,Math.round(pos.y-netState.dragOffset.y)));
      redrawNet();return;
    }
    const hit=hitNode(pos,12);
    if(hit?.node!==netState.hoveredNode){netState.hoveredNode=hit?.node||null;redrawNet();}
    const tip=G('ns-tooltip');
    if(hit&&tip){tip.style.display='block';tip.style.left=(pos.x+12)+'px';tip.style.top=(pos.y-8)+'px';tip.innerHTML=`<strong>${hit.node.name}</strong> · ${hit.line.label}`;}
    else if(tip)tip.style.display='none';
    // new-line draw preview
    if(netState.newLineStart){netState.newLineStart.mx=pos.x;netState.newLineStart.my=pos.y;redrawNet();}
  });
  cv.addEventListener('mouseup',()=>{
    if(netState.dragNode){netState.dragNode=null;cv.style.cursor='default';redrawNet();}
  });
  cv.addEventListener('mouseleave',()=>{
    netState.dragNode=null;netState.hoveredNode=null;
    const tip=G('ns-tooltip');if(tip)tip.style.display='none';redrawNet();
  });
  cv.addEventListener('dblclick',e=>{
    const pos=getPos(e),hit=hitNode(pos);
    if(hit){const name=prompt('Station name:',hit.node.name);if(name&&name.trim()){hit.node.name=name.trim();renderLineManager();redrawNet();updFromNetwork();}}
  });
  cv.addEventListener('touchstart',e=>{e.preventDefault();const t=e.touches[0];cv.dispatchEvent(new MouseEvent('mousedown',{clientX:t.clientX,clientY:t.clientY}));},{passive:false});
  cv.addEventListener('touchmove',e=>{e.preventDefault();const t=e.touches[0];cv.dispatchEvent(new MouseEvent('mousemove',{clientX:t.clientX,clientY:t.clientY}));},{passive:false});
  cv.addEventListener('touchend',e=>{e.preventDefault();cv.dispatchEvent(new MouseEvent('mouseup',{}));},{passive:false});
  if(window.ResizeObserver){
    const ro=new ResizeObserver(()=>{if(!netState.initialized&&selMode&&selCity)upd();else if(netState.initialized)redrawNet();});
    ro.observe(cv);
  }
  window.addEventListener('resize',()=>{_netW=0;if(netState.initialized)redrawNet();});
}
function onExtMove(e){
  const cv=G('c-network');if(!cv)return;
  const r=cv.getBoundingClientRect();
  if(netState.extendLine){netState.extendLine.mouseX=e.clientX-r.left;netState.extendLine.mouseY=e.clientY-r.top;redrawNet();}
}
function onExtUp(e){
  const cv=G('c-network');if(!cv)return;
  cv.removeEventListener('mousemove',onExtMove);
  if(netState.extendLine){
    const r=cv.getBoundingClientRect(),mx=e.clientX-r.left,my=e.clientY-r.top;
    const ln=netState.extendLine.line,endNd=netState.extendLine.endNode;
    const isFirst=ln.nodes[0].id===endNd.id;
    const nn={id:ln.id+'_ext'+Date.now(),x:Math.round(mx),y:Math.round(my),name:'New stop',isEnd:true};
    endNd.isEnd=false;
    if(isFirst)ln.nodes.unshift(nn);else ln.nodes.push(nn);
    renumberNodes(ln);netState.extendLine=null;renderLineManager();redrawNet();updFromNetwork();
  }
}
function renumberNodes(line){
  line.nodes.forEach((n,i)=>{
    const isEnd=i===0||i===line.nodes.length-1;n.isEnd=isEnd;
    if(!n.name||n.name.startsWith('Stop ')||n.name==='New stop'||n.name==='Stop X')
      n.name=isEnd?(i===0?'Terminus A':'Terminus B'):'Stop '+i;
  });
}
// Called after any network edit to recalculate stats + charts
function updFromNetwork(){
  const lines=netState.lines;
  // Update stations slider from average stops per line
  const totalStops=lines.reduce((a,l)=>a+(l.nodes?l.nodes.length:0),0);
  const avgStops=lines.length?Math.round(totalStops/lines.length):14;
  const stEl=G('s-stations');if(stEl&&avgStops>=3&&avgStops<=50)stEl.value=avgStops;
  // Compute average effective line length from per-line data (if available)
  const isSurf=isSurfaceMode(selMode);
  const hasPerLineLens=isSurf&&lines.some(l=>l.lineLen);
  if(hasPerLineLens){
    const maxLen=selMode?MODE_LEN_MAX[selMode.id]:60;
    const avgLen=Math.round(lines.reduce((a,l)=>{
      const base=l.lineLen||(selMode?MODE_LEN_DEFAULTS[selMode.id]:10)||10;
      const eff=l.scope==='suburb'?Math.min(maxLen,Math.round(base*1.6)):base;
      return a+eff;
    },0)/lines.length);
    const lenEl=G('s-length');
    if(lenEl&&avgLen>=parseInt(lenEl.min)&&avgLen<=parseInt(lenEl.max)){
      lenEl.value=avgLen;
      G('v-length').textContent=avgLen+' km';
    }
  }
  // Sync numLines counter
  numLines=Math.max(1,lines.length);
  const sl=G('s-lines');if(sl){sl.value=numLines;G('v-lines').textContent=numLines+' line'+(numLines>1?'s':'');}
  // Trigger full recalculation
  if(selMode&&selCity&&currentStep===4)setTimeout(upd,10);
}

// ── FICTIONAL CITY MAP GENERATOR ──────────────────────────────
// Generates a deterministic "city fabric" based on city size
// Returns an array of features (roads, blocks, parks, waterbody, suburbs)
function genCityMap(cityId,suburbs){
  const seed=cityId.charCodeAt(0)*31+cityId.charCodeAt(1||0)*7;
  function rng(s){let x=Math.sin(s+seed)*10000;return x-Math.floor(x);}
  const sizes={tiny:{r:0.18,gridN:4},small:{r:0.22,gridN:5},medium:{r:0.28,gridN:6},large:{r:0.35,gridN:7},metro:{r:0.42,gridN:8},mega:{r:0.48,gridN:9}};
  const sz=sizes[cityId]||sizes.medium;
  const terrain=TERRAIN_TYPES.find(t=>t.id===selTerrain)||TERRAIN_TYPES[0];
  return{seed,r:sz.r,gridN:sz.gridN,subs:suburbs,rng,terrain};
}
function drawCityFabric(c,W,H,cityMap,showSuburbs){
  const rng=cityMap.rng||(s=>{let x=Math.sin(s+cityMap.seed)*10000;return x-Math.floor(x);});
  const terrain=cityMap.terrain||TERRAIN_TYPES[0];
  const seed=cityMap.seed;

  // ── Terrain-specific background ──────────────────────────────
  c.fillStyle=terrain.mapBg||'#c8dda8';c.fillRect(0,0,W,H);
  const cx=W*0.5,cy=H*0.52,r=Math.min(W,H)*cityMap.r;

  // Sea / coastal
  if(terrain.mapSea||terrain.id==='coastal'||terrain.id==='island'){
    c.fillStyle='#a0c8e8';
    c.beginPath();c.moveTo(0,H*0.70);
    for(let x=0;x<=W;x+=W/14){c.lineTo(x,H*0.70+Math.sin(x*0.05+seed)*H*0.04);}
    c.lineTo(W,H);c.lineTo(0,H);c.closePath();c.fill();
    c.strokeStyle='#78aed0';c.lineWidth=2;c.beginPath();
    for(let x=0;x<=W;x+=W/14){x===0?c.moveTo(x,H*0.70+Math.sin(x*0.05+seed)*H*0.04):c.lineTo(x,H*0.70+Math.sin(x*0.05+seed)*H*0.04);}
    c.stroke();
    if(terrain.id==='island'){
      // Second water body — island channel
      c.fillStyle='#90b8d8aa';
      c.fillRect(W*0.55,0,W*0.15,H*0.45);
      c.strokeStyle='#78aed066';c.lineWidth=1;
      c.strokeRect(W*0.55,0,W*0.15,H*0.45);
    }
  }

  // River
  if(terrain.mapWater||terrain.id==='river'||terrain.id==='delta'){
    const numRivers=terrain.id==='delta'?3:1;
    for(let rv=0;rv<numRivers;rv++){
      const ry=H*(0.45+rng(10+rv*7)*0.25);
      c.strokeStyle='#88b8d8';c.lineWidth=terrain.id==='delta'?W*0.018:W*0.028;c.lineCap='round';
      c.beginPath();c.moveTo(0,ry+rng(11+rv)*H*0.05);
      c.bezierCurveTo(W*0.3,ry-H*0.07+rv*20,W*0.65,ry+H*0.09,W,ry+rng(12+rv)*H*0.05);
      c.stroke();
    }
  }

  // Hills / mountains overlay
  if(terrain.mapHills||terrain.id==='mountain'||terrain.id==='plateau'||terrain.id==='hilly'){
    const hillColor=terrain.id==='mountain'?'#b0b8c0':terrain.id==='plateau'?'#c0b898':'#b8c8a0';
    const numHills=terrain.id==='mountain'?6:terrain.id==='plateau'?3:4;
    for(let h=0;h<numHills;h++){
      const hx=W*(0.05+rng(30+h*5)*0.9),hy=H*(0.05+rng(31+h*5)*0.55);
      const hr=Math.min(W,H)*(terrain.id==='mountain'?0.18:0.12)*(0.6+rng(32+h*5)*0.8);
      c.fillStyle=hillColor+'cc';
      c.beginPath();c.ellipse(hx,hy,hr,hr*0.55,0,0,Math.PI*2);c.fill();
      if(terrain.id==='mountain'){
        // Snow cap
        c.fillStyle='rgba(255,255,255,0.7)';
        c.beginPath();c.ellipse(hx,hy-hr*0.18,hr*0.28,hr*0.18,0,0,Math.PI*2);c.fill();
      }
    }
    // Valley bottom for city
    c.fillStyle=terrain.mapBg+'cc';
    c.beginPath();c.ellipse(cx,cy,r*1.5,r*1.1,0,0,Math.PI*2);c.fill();
  }

  // Wetland patches (delta/marsh)
  if(terrain.id==='delta'){
    for(let w=0;w<8;w++){
      const wx=W*(0.1+rng(50+w*3)*0.8),wy=H*(0.1+rng(51+w*3)*0.8);
      c.fillStyle='#88c89844';
      c.beginPath();c.ellipse(wx,wy,rng(52+w*3)*35+12,rng(53+w*3)*20+8,rng(54+w*3)*Math.PI,0,Math.PI*2);c.fill();
    }
  }

  // Suburbs zones (drawn before city)
  if(showSuburbs&&cityMap.subs&&cityMap.subs.length>0){
    const dirs={N:[0,-.68],NE:[.52,-.48],E:[.72,0],SE:[.52,.48],S:[0,.68],SW:[-.52,.48],W:[-.72,0],NW:[-.52,-.48]};
    cityMap.subs.forEach((sub,i)=>{
      const d=dirs[sub.dir]||[rng(i*3+20)*1.4-0.7,rng(i*3+21)*1.4-0.7];
      const sr=Math.min(W,H)*(0.06+Math.min(sub.pop,50000)/300000);
      const sx=cx+d[0]*r*1.6,sy=cy+d[1]*r*1.6;
      if(sx<0||sx>W||sy<0||sy>H)return; // off-canvas
      c.fillStyle=sub.color+'44';
      c.beginPath();c.arc(sx,sy,sr*1.3,0,Math.PI*2);c.fill();
      c.strokeStyle=sub.color+'99';c.lineWidth=1.5;c.setLineDash([4,3]);
      c.beginPath();c.arc(sx,sy,sr*1.3,0,Math.PI*2);c.stroke();c.setLineDash([]);
      // Label
      c.fillStyle=sub.color;c.font='bold 9px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='middle';
      c.fillText(sub.icon+' '+sub.name.split(' ')[0],sx,sy+sr*1.3+10);
      // Dotted road to city centre
      c.strokeStyle=sub.color+'66';c.lineWidth=1;c.setLineDash([3,4]);
      c.beginPath();c.moveTo(cx,cy);c.lineTo(sx,sy);c.stroke();c.setLineDash([]);
    });
  }

  // Parks / green squares (before grid)
  for(let i=0;i<3+Math.floor(cityMap.gridN/2);i++){
    const px=cx+(rng(i*4)*2-1)*r*0.85,py=cy+(rng(i*4+1)*2-1)*r*0.75;
    const pw=(0.04+rng(i*4+2)*0.07)*r*2;
    c.fillStyle='#88c878';c.fillRect(px-pw/2,py-pw/3,pw,pw*0.6);
  }

  // City block grid — ring of blocks within city radius
  const gN=cityMap.gridN;
  const bSize=r*1.9/gN;
  for(let gx=-gN;gx<=gN;gx++){for(let gy=-gN;gy<=gN;gy++){
    const bx=cx+gx*bSize,by=cy+gy*bSize;
    if(Math.sqrt((gx*bSize)*(gx*bSize)+(gy*bSize*0.85)*(gy*bSize*0.85))>r*1.05)continue;
    const isCentre=Math.abs(gx)<=1&&Math.abs(gy)<=1;
    const isInner=Math.sqrt(gx*gx+gy*gy)<gN*0.3;
    c.fillStyle=isCentre?'#c8b890':isInner?'#d8c8a8':'#e0d4b8';
    c.fillRect(bx-bSize*0.42,by-bSize*0.38,bSize*0.84,bSize*0.76);
    // Inner courtyard for dense blocks
    if(isInner){c.fillStyle='#b8d8a0';c.fillRect(bx-bSize*0.18,by-bSize*0.15,bSize*0.36,bSize*0.3);}
  }}

  // Road grid
  c.strokeStyle='#f0e8d0';c.lineWidth=1.5;
  for(let gx=-gN;gx<=gN+1;gx++){
    const rx=cx+gx*bSize-bSize/2;
    c.beginPath();c.moveTo(rx,cy-r*1.1);c.lineTo(rx,cy+r*1.1);c.stroke();
  }
  for(let gy=-gN;gy<=gN+1;gy++){
    const ry=cy+gy*bSize-bSize/2;
    c.beginPath();c.moveTo(cx-r*1.1,ry);c.lineTo(cx+r*1.1,ry);c.stroke();
  }

  // Ring road
  c.strokeStyle='#e0c880';c.lineWidth=3;
  c.beginPath();c.arc(cx,cy,r*0.92,0,Math.PI*2);c.stroke();
  c.strokeStyle='#f8f4e8';c.lineWidth=1;
  c.beginPath();c.arc(cx,cy,r*0.92,0,Math.PI*2);c.stroke();

  // Main radial roads (diagonal)
  c.strokeStyle='#e8d898';c.lineWidth=3;
  for(let i=0;i<4;i++){
    const a=i*Math.PI/4+Math.PI/8;
    c.beginPath();c.moveTo(cx,cy);c.lineTo(cx+Math.cos(a)*r*1.15,cy+Math.sin(a)*r*1.15);c.stroke();
  }

  // City centre marker
  c.fillStyle='rgba(255,255,255,0.92)';c.beginPath();c.arc(cx,cy,10,0,Math.PI*2);c.fill();
  c.strokeStyle='#c8a830';c.lineWidth=2;c.beginPath();c.arc(cx,cy,10,0,Math.PI*2);c.stroke();
  c.fillStyle='#8a7020';c.font='bold 8px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='middle';c.fillText('CBD',cx,cy);

  // City name label
  const cityName=selCity?selCity.name:'City';
  c.fillStyle='rgba(0,0,0,0.45)';c.font='bold 11px Fraunces,serif';c.textAlign='center';c.textBaseline='top';
  c.fillText(cityName+' metropolitan area',W/2,6);
}

// ── RENDER CANVAS ──────────────────────────────────────────────
function redrawNet(){
  const cv=G('c-network');if(!cv)return;
  const dpr=window.devicePixelRatio||1;
  const W=getNetW(),H=460;
  if(!_netW||Math.abs(cv.width-Math.round(W*dpr))>2){
    cv.width=Math.round(W*dpr);cv.height=Math.round(H*dpr);
    cv.style.width=W+'px';cv.style.height=H+'px';
  }
  _netW=W;_netH=H;
  const c=cv.getContext('2d');c.setTransform(dpr,0,0,dpr,0,0);
  c.clearRect(0,0,W,H);

  const m=selMode||MODES[0];
  const isMet=m.id==='metro',isUg=metroType==='underground';
  const TW=isMet?6:5;
  const bMode=netState.buildMode;
  const showSubs=netState.scope==='suburbs';

  // ── draw city map background ──────────────────────────────────
  if(selCity){
    const activeSubs=showSubs?(SUBURBS[selCity.id]||[]).filter((_,i)=>selSuburbs.has(i)):[];
    const cmap=genCityMap(selCity.id,activeSubs); // terrain included via selTerrain global
    drawCityFabric(c,W,H,cmap,showSubs);
  } else {
    // Fallback grid when no city selected
    c.fillStyle='#dde8cc';c.fillRect(0,0,W,H);
    c.strokeStyle='rgba(0,0,0,0.05)';c.lineWidth=1;
    for(let i=0;i<10;i++){const x=W*i/9;c.beginPath();c.moveTo(x,0);c.lineTo(x,H);c.stroke();}
    for(let i=0;i<7;i++){const y=H*i/6;c.beginPath();c.moveTo(0,y);c.lineTo(W,y);c.stroke();}
  }

  // ── new-line draw preview ────────────────────────────────────
  if(netState.newLineStart&&netState.newLineStart.mx!=null){
    const s=netState.newLineStart;
    c.beginPath();c.moveTo(s.x,s.y);c.lineTo(s.mx,s.my);
    c.strokeStyle=LINE_COLS[netState.lines.length%LINE_COLS.length]+'99';
    c.lineWidth=4;c.setLineDash([8,4]);c.stroke();c.setLineDash([]);
    c.fillStyle='rgba(0,0,0,.55)';c.font='10px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='bottom';
    c.fillText('Click to place terminus',s.mx,s.my-6);
  }

  // ── extend preview ───────────────────────────────────────────
  if(netState.extendLine){
    const en=netState.extendLine.endNode,ex=netState.extendLine;
    c.beginPath();c.moveTo(en.x,en.y);c.lineTo(ex.mouseX,ex.mouseY);
    c.strokeStyle=ex.line.col+'88';c.lineWidth=TW;c.setLineDash([8,4]);c.stroke();c.setLineDash([]);
  }

  // ── draw lines ────────────────────────────────────────────────
  netState.lines.forEach(ln=>{
    const nds=ln.nodes;if(!nds||nds.length<2)return;
    const col=ln.col;
    const isPlanned=ln.seqStatus==='planned';
    const isConstruction=ln.seqStatus==='construction';
    const isOpen=!isPlanned&&!isConstruction;
    const alpha=isPlanned?0.28:isConstruction?0.7:1;

    // Infrastructure shadow (metro only)
    if(isMet){
      c.save();c.globalAlpha=alpha*0.18;
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=isUg?'#333':'#666';c.lineWidth=TW+20;c.lineJoin='round';c.lineCap='round';c.stroke();
      c.restore();
      if(!isUg){
        c.save();c.globalAlpha=alpha*0.14;c.strokeStyle='#000';c.lineWidth=1.5;
        for(let i=0;i<nds.length-1;i++){
          const ax=nds[i].x,ay=nds[i].y,bx=nds[i+1].x,by=nds[i+1].y;
          const dx=bx-ax,dy=by-ay,l=Math.sqrt(dx*dx+dy*dy)||1;
          const nx=-dy/l*9,ny=dx/l*9;let d=0;
          while(d<l){const t=d/l;c.beginPath();c.moveTo(ax+t*dx,ay+t*dy);c.lineTo(ax+t*dx+nx,ay+t*dy+ny);c.stroke();d+=40;}
        }c.restore();
      }
    }

    // Track — visual style differs strongly by status
    c.save();c.globalAlpha=alpha;

    if(isOpen){
      // ── OPEN: Bold glow halo + thick solid track + bright centre stripe ──
      // Outer glow
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=col+'33';c.lineWidth=TW+10;c.lineJoin='round';c.lineCap='round';c.stroke();
      // Shadow/depth band
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle='rgba(0,0,0,0.18)';c.lineWidth=TW+3;c.lineJoin='round';c.lineCap='round';c.stroke();
      // Main track
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=col;c.lineWidth=TW;c.lineJoin='round';c.lineCap='round';c.stroke();
      // Bright centre highlight stripe
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle='rgba(255,255,255,0.45)';c.lineWidth=Math.max(1.5,TW-4);c.lineJoin='round';c.lineCap='round';c.stroke();
    } else if(isConstruction){
      // ── CONSTRUCTION: Dashed amber-tinted track ──
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=col+'88';c.lineWidth=TW+2;c.lineJoin='round';c.lineCap='round';c.setLineDash([14,7]);c.stroke();c.setLineDash([]);
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=col;c.lineWidth=TW-1;c.lineJoin='round';c.lineCap='round';c.setLineDash([14,7]);c.stroke();c.setLineDash([]);
    } else {
      // ── PLANNED: Faint dashed outline only ──
      c.beginPath();nds.forEach((nd,i)=>i===0?c.moveTo(nd.x,nd.y):c.lineTo(nd.x,nd.y));
      c.strokeStyle=col;c.lineWidth=TW-1;c.lineJoin='round';c.lineCap='round';c.setLineDash([5,9]);c.stroke();c.setLineDash([]);
    }
    c.restore();

    // Status pill label
    const midNd=nds[Math.floor(nds.length/2)];
    if(isOpen){
      // Open: small ✅ badge
      c.save();c.globalAlpha=0.85;
      c.fillStyle='rgba(0,0,0,0.55)';c.font='bold 9px DM Sans,sans-serif';
      c.textAlign='center';c.textBaseline='middle';
      c.fillText('✅ Open',midNd.x,midNd.y-16);c.restore();
    } else if(isConstruction){
      c.save();c.globalAlpha=0.9;
      c.fillStyle='rgba(0,0,0,0.65)';c.font='bold 9px DM Sans,sans-serif';
      c.textAlign='center';c.textBaseline='middle';
      c.fillText('🔨 Under construction',midNd.x,midNd.y-15);c.restore();
    } else {
      c.save();c.globalAlpha=0.75;
      c.fillStyle='rgba(0,0,0,0.55)';c.font='bold 9px DM Sans,sans-serif';
      c.textAlign='center';c.textBaseline='middle';
      c.fillText('📋 Planned',midNd.x,midNd.y-15);c.restore();
    }

    // Infra label
    if(isMet&&nds.length>=2){
      const ax=nds[0].x,ay=nds[0].y,bx=nds[1].x,by=nds[1].y;
      c.save();c.globalAlpha=alpha*0.5;c.fillStyle='#222';c.font='8px DM Sans,sans-serif';
      c.textAlign='center';c.textBaseline='middle';
      c.fillText(isUg?'▿ underground':'▵ elevated',(ax+bx)/2,(ay+by)/2-(TW/2+8));c.restore();
    }

    // Stations
    nds.forEach((nd,si)=>{
      const isEnd=nd.isEnd,isHov=netState.hoveredNode&&netState.hoveredNode.id===nd.id;
      const showLbl=isEnd||(nds.length<=8)||(si%Math.ceil(nds.length/6)===0);
      c.save();c.globalAlpha=alpha;
      if(isEnd){
        c.beginPath();c.arc(nd.x,nd.y,9,0,Math.PI*2);c.fillStyle=col;c.fill();
        c.beginPath();c.arc(nd.x,nd.y,4,0,Math.PI*2);c.fillStyle='#fff';c.fill();
        if(isHov){c.beginPath();c.arc(nd.x,nd.y,12,0,Math.PI*2);c.strokeStyle=col+'88';c.lineWidth=2;c.stroke();}
        const bw=Math.max(60,nd.name.length*5.5+14),bh=16,bx2=nd.x-bw/2,by2=(si===0?nd.y-28:nd.y+12);
        c.fillStyle='rgba(0,0,0,.18)';c.beginPath();c.roundRect(bx2+2,by2+2,bw,bh,3);c.fill();
        c.fillStyle=col;c.beginPath();c.roundRect(bx2,by2,bw,bh,3);c.fill();
        c.fillStyle='#fff';c.font='bold 8px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='middle';
        c.fillText(nd.name,nd.x,by2+bh/2);
      } else {
        const rad=isHov?7:5;
        c.beginPath();c.arc(nd.x,nd.y,rad,0,Math.PI*2);c.fillStyle='#fff';c.fill();
        c.beginPath();c.arc(nd.x,nd.y,rad,0,Math.PI*2);c.strokeStyle=col;c.lineWidth=2;c.stroke();
        if(isHov){c.beginPath();c.arc(nd.x,nd.y,9,0,Math.PI*2);c.strokeStyle=col+'55';c.lineWidth=1.5;c.stroke();}
        if(showLbl){c.fillStyle='rgba(26,23,16,.85)';c.font='9px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='middle';c.fillText(nd.name,nd.x,nd.y+(si%2?-13:14));}
      }
      c.restore();
    });

    // Line badge
    const lastNd=nds[nds.length-1];
    const lbl=ln.label;const lbw=lbl.length*5.5+16;
    c.save();c.globalAlpha=alpha;
    c.fillStyle='rgba(0,0,0,.22)';c.beginPath();c.roundRect(lastNd.x+13,lastNd.y-9,lbw,18,4);c.fill();
    c.fillStyle=col;c.beginPath();c.roundRect(lastNd.x+11,lastNd.y-11,lbw,18,4);c.fill();
    c.fillStyle='#fff';c.font='bold 8px DM Sans,sans-serif';c.textAlign='left';c.textBaseline='middle';
    c.fillText(lbl,lastNd.x+18,lastNd.y);c.restore();
  });

  // ── interchanges ──────────────────────────────────────────────
  const visLines=netState.lines.filter(l=>l.intercon!=='separate');
  for(let a=0;a<visLines.length-1;a++){for(let b=a+1;b<visLines.length;b++){
    const cr=findCrossings(visLines[a].nodes,visLines[b].nodes);
    cr.forEach(({x,y})=>{
      c.beginPath();c.arc(x,y,11,0,Math.PI*2);c.fillStyle='#fff';c.fill();
      c.beginPath();c.arc(x,y,11,0,Math.PI*2);c.strokeStyle='#555';c.lineWidth=2.5;c.stroke();
      c.beginPath();c.arc(x,y,4,0,Math.PI*2);c.fillStyle='#555';c.fill();
      c.fillStyle='rgba(0,0,0,.65)';c.font='8px DM Sans,sans-serif';c.textAlign='center';c.textBaseline='top';c.fillText('⇌',x,y+13);
      [visLines[a].col,visLines[b].col].forEach((cl,i)=>{c.fillStyle=cl;c.beginPath();c.arc(x-6+i*12,y-16,3.5,0,Math.PI*2);c.fill();});
    });
  }}

  // ── title bar overlay ─────────────────────────────────────────
  const bL=bMode===2?' · 2 simultaneous':bMode===3?' · Sequential build':' · Single line';
  const infL=isMet?' · '+(isUg?'Underground':'Elevated'):'';
  const terr=TERRAIN_TYPES.find(t=>t.id===selTerrain)||TERRAIN_TYPES[0];
  const terrL=terr.costMul>1?' · '+terr.icon+' '+terr.name:'';
  c.fillStyle='rgba(255,255,255,.88)';c.beginPath();c.roundRect(6,5,W-12,22,4);c.fill();
  c.fillStyle='#1a1710';c.font='bold 11px Fraunces,serif';c.textAlign='left';c.textBaseline='middle';
  c.fillText((selMode||MODES[0]).name+' Network'+infL+bL+terrL,14,16);
  c.fillStyle='#96928a';c.font='9px DM Sans,sans-serif';c.textAlign='right';
  c.fillText('Drag · Dbl-click rename · Schematic only',W-10,16);

  // ── legend ────────────────────────────────────────────────────
  const lns=netState.lines;
  G('ns-title').textContent=(selMode||MODES[0]).name+' Network';
  G('ns-legend').innerHTML=
    lns.map(ln=>`<div class="ns-leg-item"><div class="ns-leg-swatch" style="background:${ln.col};opacity:${ln.seqStatus==='planned'?'.35':'1'}"></div>${ln.label}</div>`).join('')+
    (lns.length>=2&&lns.some(l=>l.intercon!=='separate')&&lns.filter(l=>l.intercon!=='separate').length>=2?'<div class="ns-leg-item"><span style="display:inline-block;width:10px;height:10px;border-radius:50%;border:2px solid #555;vertical-align:middle;margin-right:2px"></span>Interchange</div>':'')+
    (isMet?`<div class="ns-leg-item"><div class="ns-leg-swatch" style="background:${isUg?'#888':'#aaa'};opacity:.4"></div>${isUg?'Underground':'Elevated'}</div>`:'');
  G('ns-badges').innerHTML=lns.map(ln=>`<span style="background:${ln.col}${ln.seqStatus==='planned'?'66':''};color:#fff;font-size:10px;font-weight:700;padding:2px 9px;border-radius:10px">${ln.label}</span>`).join(' ');
}

function findCrossings(n1,n2){
  const out=[];
  for(let i=0;i<n1.length-1;i++)for(let j=0;j<n2.length-1;j++){
    const s=lineIntersect(n1[i].x,n1[i].y,n1[i+1].x,n1[i+1].y,n2[j].x,n2[j].y,n2[j+1].x,n2[j+1].y);
    if(s)out.push(s);
  }
  return out;
}
function lineIntersect(ax,ay,bx,by,cx,cy,dx,dy){
  const dxab=bx-ax,dyab=by-ay,dxcd=dx-cx,dycd=dy-cy;
  const den=dxcd*dyab-dxab*dycd;if(Math.abs(den)<0.01)return null;
  const t=((ax-cx)*dycd-(ay-cy)*dxcd)/den,u=((ax-cx)*dyab-(ay-cy)*dxab)/den;
  if(t>=0&&t<=1&&u>=0&&u<=1)return{x:Math.round(ax+t*dxab),y:Math.round(ay+t*dyab)};
  return null;
}


/* ═══ RISK ANALYSIS ═══ */
function calcRisks(r,m,params){
  const {ticket,subsidy,length,stations,funding,fare,growth,numLines}=params;
  const terrain=r.terrain||TERRAIN_TYPES[0];
  const risks=[];

  // 1. Cost overrun risk — terrain + length + metro underground
  const costRisk=(terrain.costMul>1.4||length>35||(m.id==='metro'&&params.metroType==='underground'));
  const costProb=Math.min(95,20+(terrain.costMul-1)*80+(length>30?20:0)+(m.id==='metro'?15:0));
  risks.push({
    id:'cost_overrun',ico:'💸',level:costProb>60?'hi':costProb>35?'med':'lo',
    title:'Construction cost overrun',
    desc:`Large infrastructure projects in Europe typically run ${costProb>60?'30–80%':'10–40%'} over budget. ${terrain.costMul>1.4?terrain.name+' terrain adds unpredictable ground conditions. ':''}${m.id==='metro'&&params.metroType==='underground'?'Underground tunnelling faces the highest cost uncertainty of any civil engineering. ':''}`,
    prob:costProb,severity:m.id==='metro'?90:65,
    mitigation:'Fix costs early with design-build contracts. Build a 20–30% contingency into your budget from day one.',
    tags:['Financial','Construction'],
  });

  // 2. Ridership shortfall — low growth, high fares, BRT/bus competition
  const ridProb=Math.min(90,20+(ticket>2.5?25:0)+(growth<0.01?20:0)+(fare==='free'?0:0)+(m.id==='brt'||m.id==='ber'?15:0));
  risks.push({
    id:'ridership_shortfall',ico:'👥',level:ridProb>55?'hi':ridProb>30?'med':'lo',
    title:'Lower ridership than projected',
    desc:`Demand forecasts are notoriously optimistic — real ridership is often 20–40% below projections in the first years.${ticket>2?` At €${ticket.toFixed(2)}/trip, fares may deter budget-conscious commuters.`:''}${growth<0.01?' Low population growth reduces the long-term passenger base.':''}`,
    prob:ridProb,severity:70,
    mitigation:`Consider a low introductory fare for the first 2 years. Pair with park-and-ride at termini. Build demand modelling around pessimistic (−20%) and optimistic (+20%) scenarios.`,
    tags:['Demand','Revenue'],
  });

  // 3. Political / approval delay
  const polProb=Math.min(85,25+(length>25?20:0)+(numLines>1?15:0)+(m.id==='metro'?10:0));
  risks.push({
    id:'political_delay',ico:'🏛️',level:polProb>55?'hi':polProb>30?'med':'lo',
    title:'Approval delays or political changes',
    desc:`Planning approval for transit can take 3–8 years in the EU. ${numLines>1?'Multi-line projects face more political opposition. ':''}Large projects often stall after elections when new governments prioritise differently.`,
    prob:polProb,severity:60,
    mitigation:'Cross-party political agreement before formal approval. Publish a clear economic case that survives government change. Stage the project — start with the most popular corridor.',
    tags:['Political','Timeline'],
  });

  // 4. EU funding compliance risk
  const euProb=funding==='cohesion'||funding==='erdf'||funding==='cef'?45:0;
  if(euProb>0){risks.push({
    id:'eu_compliance',ico:'🇪🇺',level:'med',
    title:'EU co-funding compliance or audit risk',
    desc:`EU co-funded projects are subject to strict eligibility rules, procurement regulations, and post-completion audits. Non-compliance can trigger partial repayment of grants — sometimes years after the project opens.`,
    prob:euProb,severity:75,
    mitigation:'Hire a dedicated EU funds compliance officer from day one. Document procurement decisions in full. Build an audit trail for every contract.',
    tags:['EU Funding','Legal'],
  });}

  // 5. Operating subsidy sustainability
  const opRatio=r.annOpex>0?r.annRev/r.annOpex:1;
  const subProb=Math.min(85,opRatio<0.4?70:opRatio<0.7?45:20);
  risks.push({
    id:'subsidy_risk',ico:'📉',level:subProb>55?'hi':subProb>30?'med':'lo',
    title:'Ongoing subsidy becomes unaffordable',
    desc:`The system needs ${fE(Math.max(0,r.annOpex-r.annRev))}/yr in public subsidy to operate. ${opRatio<0.5?'Revenue only covers '+Math.round(opRatio*100)+'% of running costs — this is a significant and permanent public commitment.':opRatio<0.8?'Revenue covers '+Math.round(opRatio*100)+'% of costs. A modest subsidy will always be needed.':'Revenue nearly covers costs — a good outcome for public transit.'}`,
    prob:subProb,severity:65,
    mitigation:`Build multi-year subsidy commitments into law. Ring-fence funding from road-user charges or parking revenues. Review fares every 3 years against inflation.`,
    tags:['Financial','Operations'],
  });

  // 6. Terrain / ground condition risk
  if(terrain.costMul>1.1){risks.push({
    id:'ground_risk',ico:terrain.icon,level:terrain.costMul>1.4?'hi':'med',
    title:`${terrain.name} ground conditions`,
    desc:`${terrain.desc} Unexpected ground conditions are one of the most common causes of cost and schedule overrun in European transit projects.`,
    prob:Math.round(terrain.costMul*40),severity:70,
    mitigation:`Commission full geotechnical surveys before tendering. Use a GBR (Geotechnical Baseline Report) to allocate ground risk between contractor and client. Include geotechnical contingency of 15–20%.`,
    tags:['Engineering','Terrain'],
  });}

  // 7. Climate / environmental objection
  const envProb=terrain.id==='coastal'||terrain.id==='delta'?55:terrain.id==='mountain'?45:25;
  risks.push({
    id:'env_risk',ico:'🌿',level:envProb>45?'med':'lo',
    title:'Environmental objections or protected sites',
    desc:`${envProb>45?'This terrain type is associated with sensitive ecosystems or flood risk zones that may trigger extended environmental impact assessments.':'Transit projects near protected habitats, rivers or coastal areas can face legal challenges from environmental groups.'} EU Habitats Directive and EIA rules can add 1–3 years to approvals.`,
    prob:envProb,severity:45,
    mitigation:'Commission EIA and Habitats Regulations Assessment early. Engage with environmental NGOs before formal planning. Design biodiversity net gain into the project.',
    tags:['Environmental','Legal'],
  });

  // Sort by severity score
  risks.sort((a,b)=>(b.prob*b.severity)-(a.prob*a.severity));
  return risks;
}

function drawRisk(r,m,params){
  const riskEl=G('risk-list');const matEl=G('risk-matrix');
  if(!riskEl||!matEl||!r||!m)return;
  const risks=calcRisks(r,m,params);
  const hiN=risks.filter(x=>x.level==='hi').length;
  const medN=risks.filter(x=>x.level==='med').length;
  const loN=risks.filter(x=>x.level==='lo').length;

  // Risk summary bar
  matEl.innerHTML=`
    <div style="display:flex;gap:8px;margin-bottom:10px;align-items:center;flex-wrap:wrap">
      <span style="font-size:11px;font-weight:700;color:var(--ink2)">Overall profile:</span>
      ${hiN?`<span style="background:#f5c0c0;color:#b02020;padding:3px 10px;border-radius:10px;font-size:11px;font-weight:700">🔴 ${hiN} High risk${hiN>1?'s':''}</span>`:''}
      ${medN?`<span style="background:#f5dfa0;color:#8a5800;padding:3px 10px;border-radius:10px;font-size:11px;font-weight:700">🟡 ${medN} Medium</span>`:''}
      ${loN?`<span style="background:#c0dfc8;color:#1a6030;padding:3px 10px;border-radius:10px;font-size:11px;font-weight:700">🟢 ${loN} Low</span>`:''}
      <span style="font-size:10px;color:var(--ink3);margin-left:4px">Updates as you change policy levers →</span>
    </div>`;

  riskEl.innerHTML=risks.map(risk=>`
    <div class="risk-item ${risk.level}">
      <div class="risk-lvl">${risk.ico}</div>
      <div style="flex:1;min-width:0">
        <div style="display:flex;align-items:center;gap:7px;flex-wrap:wrap;margin-bottom:2px">
          <span class="risk-title">${risk.title}</span>
          <span style="font-size:9px;font-weight:700;padding:1px 6px;border-radius:7px;${risk.level==='hi'?'background:#f5c0c0;color:#b02020':risk.level==='med'?'background:#f5dfa0;color:#8a5800':'background:#c0dfc8;color:#1a6030'}">${risk.level==='hi'?'HIGH RISK':risk.level==='med'?'MEDIUM':'LOW RISK'}</span>
          <span style="font-size:9px;color:var(--ink3)">Likelihood: ${risk.prob}%</span>
        </div>
        <div class="risk-desc">${risk.desc}</div>
        <div class="risk-mitigation"><strong>💡 What to do:</strong> ${risk.mitigation}</div>
        <div class="risk-badges">${risk.tags.map(t=>`<span class="risk-badge" style="background:var(--cream);color:var(--ink3)">${t}</span>`).join('')}</div>
      </div>
    </div>`).join('');
}
/* ═══ PLAIN LANGUAGE SUMMARY ═══ */
function updPlain(r,m,ticket,subsidy,length,stations,funding,fare,growth){
  const bullets=[];
  // Cost framing
  const perPerson=r.capex*1e6/(totalPop()||1);
  const tInfo=r.terrain||TERRAIN_TYPES[0];
  const terrPct=Math.round((tInfo.costMul-1)*100);
  const terrNote=terrPct>0?` The <strong>${tInfo.name.toLowerCase()} terrain</strong> adds ~${terrPct}% in engineering costs (${tInfo.extras.split('.')[0].toLowerCase()}).`:'';
  bullets.push({ico:'🏗️',txt:`This project costs <strong>${fE(r.capex)}</strong> to build — roughly <strong>€${Math.round(perPerson).toLocaleString()} per resident</strong>.${terrNote}`});
  // Opening & ridership
  const openYr=2025+Math.ceil(r.dur);
  bullets.push({ico:'🚉',txt:`The network would open around <strong>${openYr}</strong> and carry approximately <strong>${(r.riders/1000).toFixed(0)},000 passengers per day</strong> at maturity — comparable to ${r.riders>500000?'a major EU metro line':'a busy city tram'}.`});
  // Finance
  if(r.annRev>=r.annOpex){bullets.push({ico:'✅',txt:`Fare revenue (<strong>${fE(r.annRev)}/yr</strong>) is projected to <strong>cover running costs</strong>, making this operationally self-sustaining — a rare achievement in European transit.`});}
  else{const gap=(r.annOpex-r.annRev);bullets.push({ico:'💶',txt:`Running the system costs <strong>${fE(gap)}/yr more</strong> than it earns in fares. Public subsidy covers this gap — typical for EU urban transit, which is seen as a public service.`});}
  // Break-even
  if(r.be<20){bullets.push({ico:'📈',txt:`The overall investment pays back within <strong>${r.be} years of opening</strong> when economic benefits (time savings, property uplift, health) are included.`});}
  else if(r.be<30){bullets.push({ico:'📊',txt:`Full financial break-even takes around <strong>${r.be} years</strong>. This is normal for major infrastructure — governments typically justify it through wider economic and social returns.`});}
  else{bullets.push({ico:'⚠️',txt:`<strong>Full break-even may take over 30 years</strong> under current settings. Consider EU co-funding, higher ridership, or a less expensive transit mode.`});}
  // EU funding plain language
  if(r.euShare>0.5){bullets.push({ico:'🇪🇺',txt:`EU co-financing covers <strong>${Math.round(r.euShare*100)}% of construction costs</strong> (${fE(r.euAmt)}). Your city or region only needs to raise the remaining <strong>${fE(r.capex*(1-r.euShare))}</strong>.`});}
  // Environment
  bullets.push({ico:'🌿',txt:`Over 30 years, this project would save approximately <strong>${(r.co2*30).toLocaleString()} thousand tonnes of CO₂</strong> by replacing car trips — equivalent to taking ${Math.round(r.cars*30*365/10000).toLocaleString()} cars off the road permanently.`});
  // Jobs
  bullets.push({ico:'💼',txt:`Construction and operation would create or sustain around <strong>${(r.jobs*1000).toLocaleString()} jobs</strong>, both directly and in the wider economy.`});
  G('plain-bullets').innerHTML=bullets.map(b=>`<div class="plain-bullet"><span class="pb-ico">${b.ico}</span><span>${b.txt}</span></div>`).join('');
}

/* ═══ CHART HOVER TOOLTIPS ═══ */
// Attach hover listeners to a canvas, calling back with {year, values[]} for tooltip
function makeTipHandler(canvasId, tipId, getDataFn, plotParam){
  const cv=G(canvasId),tip=G(tipId);
  if(!cv||!tip)return;
  if(cv['_tip_'+tipId])return; // already registered
  cv['_tip_'+tipId]=true;
  cv.addEventListener('mousemove',e=>{
    const r2=cv.getBoundingClientRect();
    const mx=e.clientX-r2.left,my=e.clientY-r2.top;
    const info=getDataFn(mx,my,plotParam);
    if(info){
      tip.style.display='block';
      tip.innerHTML=info;
      // Position relative to chart-wrap
      const wrap=cv.parentElement;
      const wr=wrap.getBoundingClientRect();
      const tx=e.clientX-wr.left,ty=e.clientY-wr.top;
      tip.style.left=tx+'px';
      tip.style.top=(ty-10)+'px';
    } else {tip.style.display='none';}
  });
  cv.addEventListener('mouseleave',()=>{tip.style.display='none';});
}

// Store last chart params for tooltip lookups
let _lastChartData={demand:null,cashflow:null,npv:null,sensitivity:null};

function getTipDemand(mx,my,p){
  if(!_lastChartData.demand)return null;
  const {data,p:pp,maxV}=_lastChartData.demand;
  if(mx<pp.l||mx>pp.l+pp.w)return null;
  const yr=Math.round((mx-pp.l)/pp.w*30);
  const d=data[Math.min(yr,data.length-1)];
  if(!d)return null;
  const riders=d.riders>=1e6?(d.riders/1e6).toFixed(2)+'M':Math.round(d.riders/1000)+'K';
  const cap=d.cap>=1e6?(d.cap/1e6).toFixed(2)+'M':Math.round(d.cap/1000)+'K';
  const pct=d.cap>0?Math.min(100,Math.round(d.riders/d.cap*100)):0;
  return `<strong>Year ${yr}</strong><br>Riders: ${riders}/day<br>Capacity: ${cap}/day<br>Used: ${pct}%`;
}
function getTipCashflow(mx,my,p){
  if(!_lastChartData.cashflow)return null;
  const {data,p:pp,maxV}=_lastChartData.cashflow;
  if(mx<pp.l||mx>pp.l+pp.w)return null;
  const idx=Math.round((mx-pp.l)/pp.w*(data.length-1));
  const d=data[Math.min(idx,data.length-1)];if(!d)return null;
  const net=d.fareRev-d.opex;
  return `<strong>Year ${d.y}</strong><br>Revenue: €${d.fareRev.toFixed(1)}M/yr<br>Costs: €${d.opex.toFixed(1)}M/yr<br>Balance: <span style="color:${net>=0?'#7df7a0':'#f77'}">${net>=0?'+':''}€${net.toFixed(1)}M</span>`;
}
function getTipNPV(mx,my,p){
  if(!_lastChartData.npv)return null;
  const {data,p:pp,minV,rng}=_lastChartData.npv;
  if(mx<pp.l||mx>pp.l+pp.w)return null;
  const yr=Math.round((mx-pp.l)/pp.w*30);
  const d=data[Math.min(yr,data.length-1)];if(!d)return null;
  const val=d.cumNPV;const ab=Math.abs(val*1e6);
  const fmt=ab>=1e9?'€'+(val>0?'+':'')+(val*1e3).toFixed(1)+'B':'€'+(val>0?'+':'')+Math.round(val*1000)+'M';
  return `<strong>Year ${yr}</strong><br>Cumulative: <span style="color:${val>=0?'#7df7a0':'#f77'}">${fmt}</span>`;
}
function getTipSensitivity(mx,my,p){
  if(!_lastChartData.sensitivity)return null;
  const {levers,LP,RP,TP,gH,bH,gap,minV,rng,gW}=_lastChartData.sensitivity;
  if(mx<LP)return null;
  const li=Math.floor((my-TP)/(bH+gap));
  if(li<0||li>=levers.length)return null;
  const lv=levers[li];
  const impact=lv.hi-lv.lo;
  const rank=li+1;
  const rankTxt=rank===1?'🥇 Most impactful lever':rank===2?'🥈 2nd most impactful':rank===3?'🥉 3rd most impactful':'Lever #'+rank;
  return `<strong>${lv.ico||''} ${lv.n}</strong> <span style="opacity:.6">(${rankTxt})</span><br>
    <span style="opacity:.8">Worst case:</span> ${fE(lv.lo)}<br>
    <span style="opacity:.8">Best case:</span> ${fE(lv.hi)}<br>
    <span style="opacity:.8">Total swing:</span> <strong>${fE(Math.abs(impact))}</strong><br>
    <span style="color:${impact>0?'#7df7a0':'#f77'}">${impact>0?'↑ Setting this higher improves the outcome':'↓ Lower values produce better outcomes here'}</span><br>
    <span style="opacity:.7;font-size:9px">Your setting: ${lv.curVal||'—'}</span>`;
}

/* ═══ CANVAS HELPERS ═══ */
function getCtx(id,h){
  const el=G(id);if(!el)return null;
  const dpr=window.devicePixelRatio||1;
  const pw=el.parentElement?.clientWidth||el.parentElement?.offsetWidth||600;
  const w=Math.max(200,pw-32);
  el.width=w*dpr;el.height=h*dpr;el.style.width=w+'px';el.style.height=h+'px';
  const c=el.getContext('2d');c.scale(dpr,dpr);c._w=w;c._h=h;return c;
}
function GL(c,p,n=4){c.strokeStyle='#e6e2d6';c.lineWidth=1;for(let i=1;i<=n;i++){const y=p.t+p.h-(i/n)*p.h;c.beginPath();c.moveTo(p.l,y);c.lineTo(p.l+p.w,y);c.stroke();}c.strokeStyle='#ccc8b8';c.beginPath();c.moveTo(p.l,p.t+p.h);c.lineTo(p.l+p.w,p.t+p.h);c.stroke();}
function YA(c,p,max,fmt){c.fillStyle='#96928a';c.font='9px DM Sans';c.textAlign='right';[0,.5,1].forEach(pct=>c.fillText(fmt(max*pct),p.l-5,p.t+p.h-pct*p.h+3));}
function XA(c,p,yr=[0,5,10,15,20,25,30]){c.fillStyle='#96928a';c.font='9px DM Sans';c.textAlign='center';yr.forEach(y=>c.fillText('Y'+y,p.l+(y/30)*p.w,p.t+p.h+15));}

function drawDemand(r,m){
  const cv=getCtx('c-demand',200);if(!cv)return;
  const p={l:52,r:14,t:18,b:24,w:cv._w-66,h:cv._h-42};cv.clearRect(0,0,cv._w,cv._h);
  const data=r.years,col=m.color,maxV=Math.max(...data.map(d=>d.cap))*1.15;
  _lastChartData.demand={data,p,maxV};
  makeTipHandler('c-demand','tip-demand',getTipDemand,p);
  const openX=p.l+(r.dur/30)*p.w;GL(cv,p);
  // capacity dashed
  cv.beginPath();data.forEach((d,i)=>{const x=p.l+(i/30)*p.w,y=p.t+p.h-(d.cap/maxV)*p.h;i===0?cv.moveTo(x,y):cv.lineTo(x,y);});
  cv.strokeStyle='#bbb';cv.lineWidth=1.5;cv.setLineDash([5,3]);cv.stroke();cv.setLineDash([]);
  // ridership fill
  const gr=cv.createLinearGradient(0,p.t,0,p.t+p.h);gr.addColorStop(0,col+'44');gr.addColorStop(1,col+'08');
  cv.beginPath();data.forEach((d,i)=>{const x=p.l+(i/30)*p.w,y=p.t+p.h-(d.riders/maxV)*p.h;i===0?cv.moveTo(x,y):cv.lineTo(x,y);});
  cv.lineTo(p.l+p.w,p.t+p.h);cv.lineTo(p.l,p.t+p.h);cv.closePath();cv.fillStyle=gr;cv.fill();
  cv.beginPath();data.forEach((d,i)=>{const x=p.l+(i/30)*p.w,y=p.t+p.h-(d.riders/maxV)*p.h;i===0?cv.moveTo(x,y):cv.lineTo(x,y);});
  cv.strokeStyle=col;cv.lineWidth=2.5;cv.stroke();
  // legend inline
  cv.fillStyle=col+'88';cv.fillRect(p.l,p.t+2,28,7);cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText('Ridership',p.l+32,p.t+9);
  cv.strokeStyle='#bbb';cv.lineWidth=1.5;cv.setLineDash([5,3]);cv.beginPath();cv.moveTo(p.l+90,p.t+5);cv.lineTo(p.l+118,p.t+5);cv.stroke();cv.setLineDash([]);cv.fillText('Capacity',p.l+122,p.t+9);
  if(r.capSatYr){const sx=p.l+(r.capSatYr/30)*p.w;cv.fillStyle='rgba(255,140,30,.08)';cv.fillRect(sx,p.t,p.l+p.w-sx,p.h);cv.fillStyle='#a85e00';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText('⚠ Capacity reached →',sx+3,p.t+11);}
  cv.strokeStyle='#ccc';cv.lineWidth=1;cv.setLineDash([4,3]);cv.beginPath();cv.moveTo(openX,p.t);cv.lineTo(openX,p.t+p.h);cv.stroke();cv.setLineDash([]);
  cv.fillStyle='#888';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText('Opens',openX+2,p.t+11);
  YA(cv,p,maxV,v=>v>=1e6?(v/1e6).toFixed(1)+'M':Math.round(v/1000)+'K');XA(cv,p);
}
function drawCashflow(r){
  const cv=getCtx('c-cashflow',170);if(!cv)return;
  const p={l:52,r:12,t:14,b:22,w:cv._w-64,h:cv._h-36};cv.clearRect(0,0,cv._w,cv._h);
  const data=r.years.filter(d=>d.y>0),maxV=Math.max(...data.map(d=>Math.max(d.fareRev,d.opex)))*1.25;
  _lastChartData.cashflow={data,p,maxV};
  makeTipHandler('c-cashflow','tip-cashflow',getTipCashflow,p);
  GL(cv,p);const bw=(p.w/data.length)*.32;
  data.forEach((d,i)=>{const x=p.l+(i/data.length)*p.w;
    const net=d.fareRev-d.opex;
    cv.fillStyle='#1a7a3e'+(net>=0?'99':'44');cv.fillRect(x,p.t+p.h-(d.fareRev/maxV)*p.h,bw,(d.fareRev/maxV)*p.h);
    cv.fillStyle='#b0261a66';cv.fillRect(x+bw+1,p.t+p.h-(d.opex/maxV)*p.h,bw,(d.opex/maxV)*p.h);});
  YA(cv,p,maxV,v=>'€'+Math.round(v)+'M');XA(cv,p,[0,10,20,30]);
  cv.fillStyle='#1a7a3e88';cv.fillRect(p.l,p.t+2,9,7);cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText('Revenue',p.l+12,p.t+9);
  cv.fillStyle='#b0261a66';cv.fillRect(p.l+62,p.t+2,9,7);cv.fillText('Costs',p.l+74,p.t+9);
}
function drawNPVChart(r){
  const cv=getCtx('c-npv',170);if(!cv)return;
  const p={l:52,r:12,t:12,b:22,w:cv._w-64,h:cv._h-34};cv.clearRect(0,0,cv._w,cv._h);
  const data=r.years,minV=Math.min(...data.map(d=>d.cumNPV)),maxV=Math.max(...data.map(d=>d.cumNPV)),rng=maxV-minV||1;
  _lastChartData.npv={data,p,minV,rng};
  makeTipHandler('c-npv','tip-npv',getTipNPV,p);
  GL(cv,p);const zy=p.t+p.h-((0-minV)/rng)*p.h;
  if(zy>p.t&&zy<p.t+p.h){
    // shade positive area
    const posGr=cv.createLinearGradient(0,p.t,0,zy);posGr.addColorStop(0,'rgba(26,122,62,.12)');posGr.addColorStop(1,'rgba(26,122,62,0)');
    cv.fillStyle=posGr;cv.fillRect(p.l,p.t,p.w,zy-p.t);
    cv.strokeStyle='#ccc';cv.lineWidth=1;cv.setLineDash([4,3]);cv.beginPath();cv.moveTo(p.l,zy);cv.lineTo(p.l+p.w,zy);cv.stroke();cv.setLineDash([]);
    cv.fillStyle='#96928a';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText('↑ Break-even',p.l+3,zy-3);
  }
  cv.beginPath();data.forEach((d,i)=>{const x=p.l+(i/30)*p.w,y=p.t+p.h-((d.cumNPV-minV)/rng)*p.h;i===0?cv.moveTo(x,y):cv.lineTo(x,y);});
  cv.strokeStyle=r.npv>0?'var(--green)':'var(--red)';cv.lineWidth=2.5;cv.stroke();
  // final value label
  const lastX=p.l+p.w,lastD=data[data.length-1]||data[0],lastY=p.t+p.h-((lastD.cumNPV-minV)/rng)*p.h;
  cv.fillStyle=r.npv>0?'var(--green)':'var(--red)';cv.font='bold 9px DM Sans';cv.textAlign='right';cv.fillText(fE(r.npv),lastX-2,lastY-4);
  YA(cv,p,maxV,v=>fE(v));XA(cv,p,[0,10,20,30]);
}
function drawFit(ranked){
  const cv=getCtx('c-fit',190);if(!cv)return;
  const p={l:145,r:18,t:10,b:10,w:cv._w-163,h:cv._h-20};cv.clearRect(0,0,cv._w,cv._h);
  const bH=Math.min(26,(p.h/ranked.length)-6),gap=(p.h-bH*ranked.length)/(ranked.length+1);
  ranked.forEach(({m,s},i)=>{
    const y=p.t+gap+i*(bH+gap),bW=(s/100)*p.w;
    cv.fillStyle='#f0ede6';cv.beginPath();cv.roundRect(p.l,y,p.w,bH,3);cv.fill();
    cv.fillStyle=m.color+'cc';cv.beginPath();cv.roundRect(p.l,y,bW,bH,3);cv.fill();
    cv.fillStyle='#1a1710';cv.font=`${bH>22?'11px':'10px'} DM Sans`;cv.textAlign='right';cv.fillText(m.icon+' '+m.name,p.l-6,y+bH/2+3);
    if(bW>28){cv.fillStyle='white';cv.font='bold 10px DM Sans';cv.textAlign='left';cv.fillText(s+'%',p.l+bW-30,y+bH/2+3);}
    else{cv.fillStyle='#1a1710';cv.font='10px DM Sans';cv.textAlign='left';cv.fillText(s+'%',p.l+bW+4,y+bH/2+3);}
  });
}
function drawCostCap(ranked,tot,sp){
  const cv=getCtx('c-costcap',190);if(!cv)return;
  const p={l:54,r:16,t:16,b:36,w:cv._w-70,h:cv._h-52};cv.clearRect(0,0,cv._w,cv._h);
  const calcs=ranked.map(({m})=>qcalc(m,tot,sp,1.2,.4,18,14,2,6,'ppp','zone',.04,0.015,'underground',1));
  const maxC=Math.max(...calcs.map(r=>r.capex))*1.2,maxR=Math.max(...calcs.map(r=>r.riders))*1.2;
  GL(cv,p,4);cv.strokeStyle='#ccc8b8';cv.lineWidth=1;cv.beginPath();cv.moveTo(p.l,p.t);cv.lineTo(p.l,p.t+p.h);cv.lineTo(p.l+p.w,p.t+p.h);cv.stroke();
  ranked.forEach(({m,s},i)=>{
    const r=calcs[i],x=p.l+(r.capex/maxC)*p.w,y=p.t+p.h-(r.riders/maxR)*p.h,rad=7+s/20;
    cv.beginPath();cv.arc(x,y,rad,0,Math.PI*2);cv.fillStyle=m.color+'22';cv.fill();cv.strokeStyle=m.color;cv.lineWidth=2;cv.stroke();
    cv.fillStyle=m.color;cv.font='bold 12px DM Sans';cv.textAlign='center';cv.fillText(m.icon,x,y+4);
    cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.fillText(m.name.split(' ')[0],x,y+rad+11);
  });
  YA(cv,p,maxR,v=>v>=1e6?(v/1e6).toFixed(1)+'M':Math.round(v/1000)+'K');
  cv.fillStyle='#96928a';cv.font='9px DM Sans';cv.textAlign='center';
  [0,.5,1].forEach(pct=>cv.fillText(fE(maxC*pct),p.l+pct*p.w,p.t+p.h+20));
  cv.save();cv.translate(13,p.t+p.h/2);cv.rotate(-Math.PI/2);cv.textAlign='center';cv.fillText('Daily riders',0,0);cv.restore();
  cv.textAlign='center';cv.fillText('Build cost (€) →',p.l+p.w/2,p.t+p.h+30);
}
function drawSensitivity(baseR){
  const cv=getCtx('c-sensitivity',230);if(!cv)return;
  const m=selMode;if(!m||!selCity)return;
  const cp=selCity.pop,sp=suburbPop();
  const tk=gv('s-ticket'),sub=gv('s-sub')/100,len=gv('s-length');
  const st=gi('s-stations'),spd=gi('s-speed'),fr=gv('s-freq');
  const fnd=G('s-fund').value,fare=G('s-fare').value,gr=gv('s-growth')/100;
  const Q=ov=>{const pp={ticket:tk,sub,len,st,spd,fr,fnd,fare,gr,mt:metroType,nl:numLines,...ov};
    return qcalc(m,cp,sp,pp.ticket,pp.sub,pp.len,pp.st,pp.spd,pp.fr,pp.fnd,pp.fare,0.04,pp.gr,pp.mt,pp.nl).npv;};

  // Rich lever definitions with plain-language explanations
  const levers=[
    {id:'ticket', ico:'🎫', n:'Ticket price',
     lo:Q({ticket:0.2}), hi:Q({ticket:4.5}), curVal:'€'+tk.toFixed(2)+'/trip',
     loVal:'€0.20 (very cheap)', hiVal:'€4.50 (expensive)',
     plain:(impact,cur)=>`<strong>Ticket price</strong> (currently ${cur}): `+(Math.abs(impact)>baseR.capex*0.3?'This is the <em>biggest financial lever</em> available. ':'')+(impact>0?`Raising fares from €0.20 to €4.50 adds <strong>${fE(impact)}</strong> to the 30-year value — but high fares reduce ridership among lower-income passengers.`:`Fares matter but aren't the primary driver here. The range of outcomes from cheapest to most expensive fares is <strong>${fE(Math.abs(impact))}</strong>.`),
    },
    {id:'subsidy', ico:'🏛️', n:'Public subsidy',
     lo:Q({sub:0}), hi:Q({sub:.9}), curVal:Math.round(sub*100)+'% of running costs',
     loVal:'0% (no subsidy)', hiVal:'90% (heavily subsidised)',
     plain:(impact,cur)=>`<strong>Public subsidy</strong> (currently ${cur}): The government currently covers ${Math.round(sub*100)}% of operating costs. `+(impact>0?`Increasing subsidy to 90% improves viability by <strong>${fE(impact)}</strong> — but costs taxpayers more annually.`:`Subsidy level has limited impact on the 30-year NPV in this scenario, since fare revenue already covers a good share of costs.`),
    },
    {id:'length', ico:'📏', n:'Network length',
     lo:Q({len:5}), hi:Q({len:50}), curVal:len+' km',
     loVal:'5 km (one corridor)', hiVal:'50 km (city-wide network)',
     plain:(impact,cur)=>`<strong>Network length</strong> (currently ${cur}): `+(impact>0?`A longer network (up to 50 km) creates <strong>${fE(impact)}</strong> more long-term value — more stops means more riders, but also much higher build costs.`:`A shorter network is more efficient here. Extending to 50 km adds costs faster than ridership grows.`)+` The current ${len} km appears to be ${Math.abs(impact)<baseR.capex*0.5?'near-optimal':'worth revisiting'} for this city size.`,
    },
    {id:'freq', ico:'⏱️', n:'Service frequency',
     lo:Q({fr:25}), hi:Q({fr:3}), curVal:'every '+fr+' min',
     loVal:'every 25 min (infrequent)', hiVal:'every 3 min (very frequent)',
     plain:(impact,cur)=>`<strong>Service frequency</strong> (currently ${cur}): `+(impact>0?`Running trains every 3 minutes instead of every 25 creates <strong>${fE(impact)}</strong> more value — frequent service is one of the strongest drivers of ridership. People won't check timetables; they just go.`:`Frequency is less critical in this scenario, perhaps because the city is small enough that even 10-minute headways feel acceptable.`),
    },
    {id:'growth', ico:'📈', n:'Population growth',
     lo:Q({gr:0}), hi:Q({gr:.04}), curVal:(gr*100).toFixed(1)+'%/yr assumed',
     loVal:'0% (static population)', hiVal:'4%/yr (rapid growth)',
     plain:(impact,cur)=>`<strong>Population growth</strong> (currently assuming ${cur}): `+(impact>0?`If the city grows faster than expected, the 30-year value improves by <strong>${fE(impact)}</strong>. Transit investment pays off much more when cities grow — it's a bet on the city's future.`:`Growth has limited impact here, suggesting the project's viability doesn't depend heavily on future population increases.`),
    },
    {id:'speed', ico:'⚡', n:'Build speed',
     lo:Q({spd:1}), hi:Q({spd:3}), curVal:SPD[spd]+' pace',
     loVal:'Cautious (slowest)', hiVal:'Accelerated (fastest)',
     plain:(impact,cur)=>`<strong>Build speed</strong> (currently ${cur}): `+(impact>0?`Faster construction adds <strong>${fE(impact)}</strong> over 30 years — mainly because the system opens sooner and starts earning fares years earlier. Every year of delay costs real money.`:`Build speed has modest impact here. The project opens within a reasonable time even at a cautious pace.`),
    },
    {id:'funding', ico:'🇪🇺', n:'EU co-funding',
     lo:Q({fnd:'public'}), hi:Q({fnd:'cohesion'}), curVal:fnd==='public'?'No EU grant':fnd,
     loVal:'Public only (no EU grant)', hiVal:'Cohesion Fund (85% covered)',
     plain:(impact,cur)=>`<strong>EU co-funding</strong> (currently: ${cur}): `+(impact>0?`Securing EU Cohesion Fund support (85% of build cost) versus no EU grant creates <strong>${fE(impact)}</strong> in additional value. This is often the single most impactful financial decision a city can make — it shifts most of the capital risk to the EU.`:`EU co-funding is less impactful here, likely because the project is already viable without it, or because the city may not be eligible for the highest-rate funds.`),
    },
  ];

  // Sort by absolute impact (biggest first)
  const sorted=[...levers].sort((a,b)=>Math.abs(b.hi-b.lo)-Math.abs(a.hi-a.lo));

  const W=cv._w,H=cv._h;cv.clearRect(0,0,W,H);
  const LP=148,RP=18,TP=16,BP=14;
  const gW=W-LP-RP,gH=H-TP-BP;
  const bH=Math.min(23,(gH/sorted.length)-5),gap=(gH-bH*sorted.length)/(sorted.length+1);
  const allV=[...sorted.flatMap(l=>[l.lo,l.hi]),0];
  const minV=Math.min(...allV),maxV=Math.max(...allV),rng=maxV-minV||1;
  const zX=LP+(0-minV)/rng*gW;

  // Zero line
  cv.strokeStyle='#aaa';cv.lineWidth=1.5;cv.setLineDash([5,3]);
  cv.beginPath();cv.moveTo(zX,TP-4);cv.lineTo(zX,TP+gH+4);cv.stroke();cv.setLineDash([]);
  cv.fillStyle='#555';cv.font='bold 9px DM Sans';cv.textAlign='center';
  cv.fillText('Break-even line',zX,TP-6);

  // Rank badge colours
  const rankCols=['#f59f00','#adb5bd','#cd7f32'];

  sorted.forEach((lv,i)=>{
    const y=TP+gap+i*(bH+gap);
    const loX=LP+(lv.lo-minV)/rng*gW,hiX=LP+(lv.hi-minV)/rng*gW;
    const curX=LP+(baseR.npv-minV)/rng*gW;
    const impact=lv.hi-lv.lo;
    const positive=impact>0;
    const col=positive?'#1a7a3e':'#b0261a';
    const rank=i+1;

    // Track background
    cv.fillStyle='#f0ede6';cv.beginPath();cv.roundRect(LP,y,gW,bH,4);cv.fill();

    // Impact bar
    const x1=Math.min(loX,hiX),barW=Math.abs(hiX-loX);
    const barGr=cv.createLinearGradient(x1,0,x1+barW,0);
    barGr.addColorStop(0,col+'44');barGr.addColorStop(1,col+'88');
    cv.fillStyle=barGr;cv.beginPath();cv.roundRect(x1,y,barW,bH,4);cv.fill();
    cv.strokeStyle=col+'99';cv.lineWidth=1.5;cv.beginPath();cv.roundRect(x1,y,barW,bH,4);cv.stroke();

    // Current position dot
    cv.fillStyle=m.color;cv.beginPath();cv.arc(curX,y+bH/2,5,0,Math.PI*2);cv.fill();
    cv.fillStyle='#fff';cv.beginPath();cv.arc(curX,y+bH/2,2.5,0,Math.PI*2);cv.fill();

    // Rank medal on left
    if(rank<=3){
      cv.fillStyle=rankCols[rank-1];cv.beginPath();cv.roundRect(LP-26,y+(bH-14)/2,18,14,3);cv.fill();
      cv.fillStyle='#fff';cv.font='bold 8px DM Sans';cv.textAlign='center';
      cv.fillText('#'+rank,LP-17,y+bH/2+3);
    }

    // Lever name
    cv.fillStyle='#1a1710';cv.font='bold 10px DM Sans';cv.textAlign='right';
    cv.fillText(lv.ico+' '+lv.n,LP-30,y+bH/2+3);

    // End value labels
    cv.fillStyle='#96928a';cv.font='9px DM Sans';cv.textAlign='center';
    cv.fillText(fE(lv.lo),loX,y+(positive?bH+11:-3));
    cv.fillText(fE(lv.hi),hiX,y+(positive?-3:bH+11));

    // Impact label inside bar if wide enough
    if(barW>45){
      cv.fillStyle=col;cv.font='bold 8px DM Sans';cv.textAlign='center';
      cv.fillText('±'+fE(Math.abs(impact)/2),x1+barW/2,y+bH/2+3);
    }
  });

  // Legend
  cv.fillStyle='#1a7a3e55';cv.fillRect(LP,H-11,11,7);
  cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.textAlign='left';
  cv.fillText('Potential gain range',LP+14,H-4);
  cv.fillStyle=m.color;cv.beginPath();cv.arc(LP+150,H-8,5,0,Math.PI*2);cv.fill();
  cv.fillStyle='#fff';cv.beginPath();cv.arc(LP+150,H-8,2.5,0,Math.PI*2);cv.fill();
  cv.fillStyle='#504d44';cv.fillText('Your current setting',LP+158,H-4);

  _lastChartData.sensitivity={levers:sorted,LP,RP,TP,gH,bH,gap,minV,rng,gW};
  makeTipHandler('c-sensitivity','tip-sensitivity',getTipSensitivity,null);

  // ── Plain-language explanations below chart ───────────────────
  const el=G('sens-plain');if(!el)return;

  const rows=sorted.map((lv,i)=>{
    const impact=lv.hi-lv.lo;
    const positive=impact>0;
    const rank=i+1;
    const rankLabel=rank===1?'🥇 Biggest lever':rank===2?'🥈 Second biggest':rank===3?'🥉 Third biggest':'';
    const col=positive?'#1a7a3e':'#b0261a';
    const bg=positive?'#f4fbf6':'#fff5f5';
    const border=positive?'#b8e4c8':'#f5c0c0';
    const explanation=lv.plain(impact,lv.curVal);
    const posNeg=positive
      ?`<span style="color:#1a7a3e;font-weight:700">↑ Higher = better outcome</span>`
      :`<span style="color:#b0261a;font-weight:700">↓ Lower = better outcome</span>`;

    return`<div style="border:1.5px solid ${border};border-radius:10px;padding:10px 13px;background:${bg};display:flex;gap:10px;align-items:flex-start">
      <div style="font-size:20px;flex-shrink:0;line-height:1">${lv.ico}</div>
      <div style="flex:1;min-width:0">
        <div style="display:flex;align-items:center;gap:6px;flex-wrap:wrap;margin-bottom:3px">
          <span style="font-size:12px;font-weight:700;color:${col}">${lv.n}</span>
          ${rankLabel?`<span style="font-size:9px;background:${col}22;color:${col};padding:1px 6px;border-radius:8px;font-weight:700">${rankLabel}</span>`:''}
          ${posNeg}
        </div>
        <div style="font-size:11px;color:#504d44;line-height:1.55">${explanation}</div>
        <div style="margin-top:5px;display:flex;gap:8px;flex-wrap:wrap;font-size:10px">
          <span style="background:#f0ede6;border-radius:5px;padding:2px 7px"><strong>Worst case:</strong> ${lv.loVal} → ${fE(lv.lo)}</span>
          <span style="background:#f0ede6;border-radius:5px;padding:2px 7px"><strong>Best case:</strong> ${lv.hiVal} → ${fE(lv.hi)}</span>
          <span style="background:${m.color}18;border-radius:5px;padding:2px 7px;color:${m.color}"><strong>Your setting:</strong> ${lv.curVal}</span>
        </div>
      </div>
    </div>`;
  });

  const tip2=sorted.length>1
    ?`Focus especially on <strong>${sorted[0].ico} ${sorted[0].n}</strong> and <strong>${sorted[1].ico} ${sorted[1].n}</strong> — together they explain most of the variation in outcomes for this scenario.`
    :`<strong>${sorted[0].ico} ${sorted[0].n}</strong> is the single biggest factor here.`;
  el.innerHTML=`
    <div style="font-size:11px;font-weight:700;color:var(--ink3);text-transform:uppercase;letter-spacing:.6px;margin-bottom:6px">📖 What each lever means in plain language — ranked by impact</div>
    ${rows.join('')}
    <div style="background:#edf2fb;border:1px solid #c0d4f8;border-radius:9px;padding:11px 14px;font-size:11px;color:#155090;line-height:1.6">
      <strong>💡 Where to focus your attention:</strong> The levers are sorted from most to least impactful.
      ${tip2}
      Changes to the bottom-ranked levers will barely move the needle — don't spend political capital fighting over them.
    </div>`;
}

/* ═══ SCENARIO COMPARE CHARTS ═══ */
function drawCmpR(){
  const cv=getCtx('c-cmp-r',170);if(!cv)return;
  const p={l:52,r:14,t:14,b:24,w:cv._w-66,h:cv._h-38};cv.clearRect(0,0,cv._w,cv._h);
  const maxV=Math.max(...scenarios.map(s=>s.r.riders))*1.15;GL(cv,p);
  scenarios.forEach(s=>{cv.beginPath();s.r.years.forEach((d,i)=>{const x=p.l+(i/30)*p.w,y=p.t+p.h-(d.riders/maxV)*p.h;i===0?cv.moveTo(x,y):cv.lineTo(x,y);});cv.strokeStyle=s.col;cv.lineWidth=2;cv.stroke();});
  XA(cv,p,[0,10,20,30]);YA(cv,p,maxV,v=>v>=1e6?(v/1e6).toFixed(1)+'M':Math.round(v/1000)+'K');
  scenarios.forEach((s,i)=>{cv.fillStyle=s.col;cv.fillRect(p.l+i*80,p.t+2,9,5);cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText(s.name.substring(0,11),p.l+i*80+13,p.t+9);});
}
function drawCmpF(){
  const cv=getCtx('c-cmp-f',170);if(!cv)return;
  const p={l:62,r:14,t:14,b:50,w:cv._w-76,h:cv._h-64};cv.clearRect(0,0,cv._w,cv._h);
  const cats=['Build cost','Income/yr','Costs/yr','30yr NPV'];
  const gV=s=>[s.r.capex,s.r.annRev,s.r.annOpex,Math.abs(s.r.npv/10)];
  const maxVs=cats.map((_,ci)=>Math.max(...scenarios.map(s=>gV(s)[ci]))*1.3||1);
  const gW2=p.w/cats.length;GL(cv,p);
  cats.forEach((cat,ci)=>{
    const gx=p.l+ci*gW2+4;
    scenarios.forEach((s,si)=>{const v=gV(s)[ci],bh=(v/maxVs[ci])*p.h*.85;const bx=gx+si*(gW2/scenarios.length*.8),bw=gW2/scenarios.length*.65;cv.fillStyle=s.col+'bb';cv.beginPath();cv.roundRect(bx,p.t+p.h-bh,bw,bh,[3,3,0,0]);cv.fill();});
    cv.fillStyle='#96928a';cv.font='9px DM Sans';cv.textAlign='center';cv.fillText(cat,gx+gW2/2-4,p.t+p.h+18);
  });
  scenarios.forEach((s,i)=>{cv.fillStyle=s.col;cv.fillRect(p.l+i*80,p.t+2,9,7);cv.fillStyle='#504d44';cv.font='9px DM Sans';cv.textAlign='left';cv.fillText(s.name.substring(0,9),p.l+i*80+13,p.t+9);});
}


/* ═══ DECISION TREE SCENARIO ANALYSIS ═══ */

// ── Scoring engine ────────────────────────────────────────────────────
function scoreScenario(s){
  const r=s.r;
  const npvRatio=r.npv/Math.max(1,r.capex);
  const finScore =Math.min(100,Math.max(0,50+npvRatio*30));
  const beScore  =Math.min(100,Math.max(0,100-r.be*2.5));
  const riderEff =r.riders/Math.max(1,r.capex);
  const riderScore=Math.min(100,Math.max(0,riderEff*0.04));
  const envScore =Math.min(100,Math.max(0,r.co2*1000/Math.max(1,r.capex)*8));
  const euScore  =Math.min(100,Math.max(0,r.euShare*80+r.viab*0.2));
  const W={fin:0.30,be:0.20,rider:0.22,env:0.14,eu:0.14};
  const total=finScore*W.fin+beScore*W.be+riderScore*W.rider+envScore*W.env+euScore*W.eu;
  return{total:Math.round(total),fin:Math.round(finScore),be:Math.round(beScore),
         rider:Math.round(riderScore),env:Math.round(envScore),eu:Math.round(euScore)};
}

// ── Single decision-tree question node ────────────────────────────────
function dtQuestion(icon,question,answers){
  return '<div class="dt-node">'
    +'<div class="dt-node-q">'+icon+' '+question+'</div>'
    +'<div class="dt-node-ans">'+answers.map(function(a){
      return '<div class="dt-ans-row">'
        +'<div class="dt-ans-dot" style="background:'+(a.col||'#ccc')+'"></div>'
        +'<span>'+a.text+'</span></div>';
    }).join('')+'</div></div>';
}

// ── Plain-language narrative for the winner card ───────────────────────
function buildWinnerNarrative(winner,runner,scored){
  var w=winner, r2=runner, ws=w.scores, rs=r2.scores;
  var margin=ws.total-rs.total;
  var parts=[];
  var dimNames={fin:'financial viability',be:'fast payback',rider:'ridership efficiency',
                env:'environmental impact',eu:'EU funding alignment'};
  var bestDims=Object.keys(ws).filter(function(k){return k!=='total';})
    .sort(function(a,b){return ws[b]-ws[a];}).slice(0,2)
    .map(function(k){return dimNames[k]||k;});
  parts.push('<strong style="color:#1a7a3e">'+w.name+'</strong> scores highest overall ('+ws.total+'/100), with particular strengths in <strong>'+bestDims[0]+'</strong> and <strong>'+bestDims[1]+'</strong>.');
  if(margin>15){
    parts.push('It leads '+r2.name+' by '+margin+' points — a <strong>clear margin</strong> across multiple criteria.');
  } else if(margin>7){
    parts.push('It leads '+r2.name+' by '+margin+' points. A meaningful gap, but '+r2.name+' may suit you better if your council prioritises a different criterion.');
  } else {
    parts.push('<strong>This is a very close call</strong> — '+r2.name+' is only '+margin+" points behind. The final choice may come down to your city council's priorities.");
  }
  if(w.r.be<20) parts.push('It breaks even in just '+w.r.be+' years — '+(w.r.be<15?'exceptional':'very good')+' for a transit project.');
  if(w.r.euAmt>0) parts.push('Capturing '+fE(w.r.euAmt)+" in EU co-funding significantly reduces the city's own financing burden.");
  return parts.join(' ');
}

// ── Main decision-tree renderer ───────────────────────────────────────
function runDecisionTree(){
  if(scenarios.length<2)return;
  var scored=scenarios.map(function(s){return Object.assign({},s,{scores:scoreScenario(s)});});
  scored.sort(function(a,b){return b.scores.total-a.scores.total;});
  var winner=scored[0], runner=scored[1];
  var ws=winner.scores;
  var margin=ws.total-runner.scores.total;
  var confidence=margin>15?'Clear winner':margin>7?'Likely best choice':'Very close — read detail below';

  // ── Score-bar (proportional coloured segments) ────────────────
  var segDefs=[
    {k:'fin', col:'#1a7a3e', w:0.30, lbl:'💰'},
    {k:'be',  col:'#155090', w:0.20, lbl:'⏱️'},
    {k:'rider',col:'#9a6000',w:0.22, lbl:'👥'},
    {k:'env', col:'#4a2e90', w:0.14, lbl:'🌿'},
    {k:'eu',  col:'#003399', w:0.14, lbl:'🇪🇺'},
  ];
  var scoreBarHTML=segDefs.map(function(seg){
    var pct=Math.round(ws[seg.k]*seg.w);
    return '<div class="dt-score-seg" style="background:'+seg.col+';width:'+pct+'%">'+(pct>6?seg.lbl:'')+'</div>';
  }).join('');

  // ── Per-criterion mini tiles ──────────────────────────────────
  var critMeta={
    fin:{ico:'💰',lbl:'Viability',    tip:'Does the money add up over 30 years?'},
    be: {ico:'⏱️',lbl:'Quick payback',tip:'How many years before the investment pays off?'},
    rider:{ico:'👥',lbl:'Ridership',  tip:'How many people use it, per euro spent?'},
    env:{ico:'🌿',lbl:'Environment',  tip:'CO₂ saved per euro invested'},
    eu: {ico:'🇪🇺',lbl:'EU alignment',tip:'How much EU grant money does it capture?'},
  };
  var criteriaHTML=Object.keys(critMeta).map(function(k){
    var v=ws[k], col=v>66?'#1a7a3e':v>40?'#a85e00':'#b0261a';
    var m=critMeta[k];
    return '<div class="dt-crit" title="'+m.tip+'">'
      +'<div class="dt-crit-val" style="color:'+col+'">'+v+'</div>'
      +'<div class="dt-crit-lbl">'+m.ico+' '+m.lbl+'</div></div>';
  }).join('');

  G('dt-winner-box').innerHTML=
    '<div class="dt-winner">'
      +'<div class="dt-winner-crown">🏆</div>'
      +'<div class="dt-winner-body">'
        +'<div style="display:flex;align-items:center;gap:8px;margin-bottom:4px;flex-wrap:wrap">'
          +'<div class="dt-winner-title">'+winner.name+'</div>'
          +'<span style="background:#1a7a3e;color:#fff;padding:2px 10px;border-radius:8px;font-size:11px;font-weight:700">'+ws.total+'/100</span>'
          +'<span style="background:#edf2fb;color:#155090;padding:2px 9px;border-radius:8px;font-size:10px;font-weight:600">'+confidence+'</span>'
        +'</div>'
        +'<div class="dt-score-bar" title="Weighted score breakdown by criterion">'+scoreBarHTML+'</div>'
        +'<div class="dt-winner-sub" style="margin:8px 0">'+buildWinnerNarrative(winner,runner,scored)+'</div>'
        +'<div class="dt-criteria">'+criteriaHTML+'</div>'
      +'</div>'
    +'</div>';

  // ── Decision-tree question nodes ──────────────────────────────
  var nodes=[];

  // Q1 — viability gate
  var viable=scored.filter(function(s){return s.r.viab>50;});
  var notViable=scored.filter(function(s){return s.r.viab<=50;});
  nodes.push(dtQuestion('💰','Step 1 — Is the project financially viable at all?',
    viable.map(function(s){return{text:'✅ '+s.name+' — viability '+Math.round(s.r.viab)+'% (passes the gate, moves to next test)',col:s.col};})
    .concat(notViable.map(function(s){return{text:'❌ '+s.name+' — viability only '+Math.round(s.r.viab)+'%. Needs higher subsidy, lower cost mode, or EU funding before it can proceed.',col:s.col};}))
  ));

  // Q2 — break-even speed (among viable)
  if(viable.length>1){
    var beRanked=viable.slice().sort(function(a,b){return a.r.be-b.r.be;});
    nodes.push(dtQuestion('⏱️','Step 2 — Which recoups its investment the fastest?',
      beRanked.map(function(s,i){
        var label=s.r.be>=99?'never breaks even within 30 years':s.r.be+' years to break even';
        return{text:(i===0?'✅ ':'· ')+s.name+' — '+label+(i===0?' ← fastest payback':''),col:s.col};
      })
    ));
  }

  // Q3 — ridership efficiency
  var riderRanked=scored.slice().sort(function(a,b){return b.scores.rider-a.scores.rider;});
  nodes.push(dtQuestion('👥','Step 3 — Which moves the most people per euro spent?',
    riderRanked.map(function(s,i){
      return{text:(i===0?'✅ ':'· ')+s.name+' — '+fPF(s.r.riders)+' daily riders at maturity (efficiency score '+s.scores.rider+'/100)',col:s.col};
    })
  ));

  // Q4 — EU co-funding (only if any scenario uses it)
  var euRanked=scored.slice().sort(function(a,b){return b.r.euAmt-a.r.euAmt;});
  if(euRanked[0].r.euAmt>0){
    nodes.push(dtQuestion('🇪🇺','Step 4 — Which captures the most EU grant money?',
      euRanked.map(function(s,i){
        var eu=s.r.euAmt>0?fE(s.r.euAmt)+' ('+Math.round(s.r.euShare*100)+'% of build cost covered)':'No EU grant selected';
        return{text:(i===0?'✅ ':'· ')+s.name+' — '+eu,col:s.col};
      })
    ));
  }

  // Q5 — environmental outcome
  var envRanked=scored.slice().sort(function(a,b){return b.r.co2-a.r.co2;});
  nodes.push(dtQuestion('🌿','Step 5 — Which is best for the environment?',
    envRanked.map(function(s,i){
      return{text:(i===0?'✅ ':'· ')+s.name+' — '+Math.round(s.r.co2*1000).toLocaleString()+' tonnes of CO₂ avoided per year',col:s.col};
    })
  ));

  // Final verdict node
  nodes.push(dtQuestion('🏆','Final verdict — weighted score across all five tests:',
    scored.map(function(s,i){
      var medal=i===0?'🥇':i===1?'🥈':i===2?'🥉':'#'+(i+1);
      return{text:medal+' '+s.name+' — '+s.scores.total+'/100'+(i===0?' ← RECOMMENDED':''),col:s.col};
    })
  ));

  G('dt-tree-nodes').innerHTML=nodes.join('');

  // ── Full scoring table ────────────────────────────────────────
  var rows=scored.map(function(s,i){
    var sc=s.scores;
    function cell(k){
      var v=sc[k], col=v>66?'#1a7a3e':v>40?'#a85e00':'#b0261a';
      return '<td style="text-align:center"><span class="dt-score-pill" style="background:'+col+'">'+v+'</span></td>';
    }
    var medal=i===0?'🥇':i===1?'🥈':i===2?'🥉':'#'+(i+1);
    return '<tr class="'+(i===0?'winner-row':'')+'">'
      +'<td style="text-align:center;font-size:14px">'+medal+'</td>'
      +'<td><span style="display:inline-block;width:9px;height:9px;border-radius:50%;background:'+s.col+';margin-right:5px;vertical-align:middle"></span>'+s.name+'</td>'
      +cell('fin')+cell('be')+cell('rider')+cell('env')+cell('eu')
      +'<td style="text-align:center;font-weight:700;font-size:14px;color:'+(i===0?'#1a7a3e':'#504d44')+'">'+sc.total+'</td>'
      +'</tr>';
  }).join('');

  G('dt-ranking').innerHTML=
    '<div style="font-size:11px;font-weight:700;color:var(--ink3);text-transform:uppercase;letter-spacing:.5px;margin:12px 0 5px">Full scoring breakdown — 5 criteria, scored 0 to 100</div>'
    +'<div style="display:grid;grid-template-columns:repeat(auto-fill,minmax(200px,1fr));gap:6px;margin-bottom:10px">'
      +'<div style="background:#f4fbf6;border:1px solid #b8e4c8;border-radius:8px;padding:7px 10px"><div style="font-weight:700;font-size:11px;color:#1a7a3e">💰 Worth the money?</div><div style="font-size:10px;color:var(--ink3);margin-top:2px">Does the project earn back its total cost over 30 years, including economic benefits like time saved and cleaner air? 100 = excellent value, 0 = very poor value.</div></div>'
      +'<div style="background:#edf2fb;border:1px solid #b0c8f0;border-radius:8px;padding:7px 10px"><div style="font-weight:700;font-size:11px;color:#155090">⏱️ How fast it pays back</div><div style="font-size:10px;color:var(--ink3);margin-top:2px">How many years from opening until the investment has been fully recovered. Faster is better — politicians and citizens expect to see results within a generation.</div></div>'
      +'<div style="background:#fdf4e3;border:1px solid #f0c060;border-radius:8px;padding:7px 10px"><div style="font-weight:700;font-size:11px;color:#8a5800">👥 People served</div><div style="font-size:10px;color:var(--ink3);margin-top:2px">Daily passengers carried per million euros invested. A system that moves many people cheaply scores high; one that is expensive and lightly used scores low.</div></div>'
      +'<div style="background:#f4fbf6;border:1px solid #b8e4c8;border-radius:8px;padding:7px 10px"><div style="font-weight:700;font-size:11px;color:#2a6040">🌿 Greener air</div><div style="font-size:10px;color:var(--ink3);margin-top:2px">Tonnes of CO₂ avoided each year per million euros spent. Replacing car trips with clean transit reduces air pollution and helps meet EU climate targets.</div></div>'
      +'<div style="background:#edf2fb;border:1px solid #b0c8f0;border-radius:8px;padding:7px 10px"><div style="font-weight:700;font-size:11px;color:#003399">🇪🇺 EU money captured</div><div style="font-size:10px;color:var(--ink3);margin-top:2px">How much of the build cost is covered by EU grants. EU co-funding can pay up to 85% of costs — leaving it unclaimed means the city pays far more from its own budget.</div></div>'
    +'</div>'
    +'<table class="dt-rank-table">'
      +'<thead><tr>'
        +'<th>Rank</th><th>Scenario</th>'
        +'<th title="Does the project earn back its investment over 30 years?">💰 Worth the money?<br><small style=\'font-weight:400;font-size:8px\'>Long-term value</small></th>'
        +'<th title="How many years before the project recoups its build cost?">⏱️ How fast it pays back<br><small style=\'font-weight:400;font-size:8px\'>Years to break even</small></th>'
        +'<th title="How many daily passengers per million euros invested?">👥 People served<br><small style=\'font-weight:400;font-size:8px\'>Riders per € spent</small></th>'
        +'<th title="Tonnes of CO₂ avoided per million euros invested">🌿 Greener air<br><small style=\'font-weight:400;font-size:8px\'>CO₂ saved</small></th>'
        +'<th title="How much EU grant money does this scenario capture?">🇪🇺 EU money captured<br><small style=\'font-weight:400;font-size:8px\'>Grant share</small></th>'
        +'<th>Overall score<br><small style=\'font-weight:400;font-size:8px\'>/100</small></th>'
      +'</tr></thead>'
      +'<tbody>'+rows+'</tbody>'
    +'</table>'
    +'<div style="background:#f8f6f0;border-radius:8px;padding:9px 12px;margin-top:8px;font-size:10px;color:var(--ink3);line-height:1.6">'
      +'<strong style="color:var(--ink2)">🔢 Weights used:</strong> '
      +'💰 Worth the money: 30 pts · ⏱️ Payback speed: 20 pts · 👥 People served: 22 pts · 🌿 Environment: 14 pts · 🇪🇺 EU funding: 14 pts. '
      +'Scores are shown as 🟢 green (66+), 🟡 amber (40–65) or 🔴 red (under 40). A scenario does not need to be perfect on every criterion — the best choice is the one with the highest <em>total</em> across all five.'
    +'</div>';
}
/* ═══ SCENARIOS ═══ */
function saveScenario(){
  const inp=G('sc-name-in');const name=inp.value.trim()||'Scenario '+(scenarios.length+1);
  if(!lastCalc){toast('Run the simulator first.');return;}
  const {r,m,params}=lastCalc;const col=SC_COLORS[scenarios.length%SC_COLORS.length];const id='sc_'+Date.now();
  scenarios.push({id,name,r,m,params,col});activeScId=id;inp.value='';renderScChips();toast('Saved: '+name+' — decision tree updated');
  if(scenarios.length>=2){G('cmp-wrap').style.display='block';renderCmpPanel();}
  if(scenarios.length>=2)runDecisionTree();
}
function renderScChips(){
  const cont=G('sc-chips');
  if(!scenarios.length){cont.innerHTML='<span style="font-size:11px;color:var(--ink3);font-style:italic">None saved yet.</span>';return;}
  cont.innerHTML=scenarios.map(s=>`<div class="sc-chip ${s.id===activeScId?'cur':''}" onclick="loadSc('${s.id}')"><span class="sc-chip-dot" style="background:${s.col}"></span>${s.name}<span class="sc-del" onclick="event.stopPropagation();delSc('${s.id}')">×</span></div>`).join('');
}
function loadSc(id){
  const s=scenarios.find(x=>x.id===id);if(!s)return;activeScId=id;selMode=s.m;const pp=s.params;
  G('s-ticket').value=pp.ticket;G('s-sub').value=Math.round(pp.subsidy*100);G('s-length').value=pp.length;
  G('s-stations').value=pp.stations;G('s-speed').value=pp.speed;G('s-freq').value=pp.freq;
  G('s-growth').value=(pp.growth*100).toFixed(1);G('s-fund').value=pp.funding;G('s-fare').value=pp.fare;
  metroType=pp.metroType||'underground';setMetroType(metroType);setLinesSlider(pp.numLines||1);renderSimModeTabs();renderScChips();upd();toast('Loaded: '+s.name);
}
function delSc(id){scenarios=scenarios.filter(s=>s.id!==id);if(activeScId===id)activeScId=null;if(scenarios.length<2)G('cmp-wrap').style.display='none';renderScChips();if(scenarios.length>=2)renderCmpPanel();}
function renderCmpPanel(){
  const metrics=[
    {l:'Transit mode',        note:'Which type of public transport this scenario uses',
     fn:s=>`<div class="mode-cell"><span class="mdot" style="background:${s.m.color}"></span>${s.m.icon} ${s.m.name}</div>`,raw:null},
    {l:'Total build cost',    note:'How much it costs to design, build and equip the whole network before a single passenger boards',
     fn:s=>fE(s.r.capex),raw:s=>s.r.capex,b:'min'},
    {l:'Daily passengers',    note:'How many people will use the system every day once it has been running for several years and demand has matured',
     fn:s=>fPF(s.r.riders),raw:s=>s.r.riders,b:'max'},
    {l:'Time to open',        note:'How many years from today until the first passengers travel — includes design, approvals and construction',
     fn:s=>s.r.dur.toFixed(1)+' yr',raw:s=>s.r.dur,b:'min'},
    {l:'Fare income / year',  note:'How much money the system collects from ticket sales each year at maturity',
     fn:s=>fE(s.r.annRev),raw:s=>s.r.annRev,b:'max'},
    {l:'Running costs / year',note:'What it costs each year to operate the system: drivers, energy, maintenance and administration',
     fn:s=>fE(s.r.annOpex),raw:s=>s.r.annOpex,b:'min'},
    {l:'Break-even year',     note:'How many years after opening until the cumulative economic and financial benefits outweigh the total investment. Under 20 years is good for transit.',
     fn:s=>s.r.be>=99?'>30 yrs':s.r.be+' yrs',raw:s=>s.r.be>=99?99:s.r.be,b:'min'},
    {l:'30-year net value',   note:'The total financial result after 30 years — build cost minus all benefits earned. Positive means the investment paid off; negative means it did not fully recover its cost in financial terms alone (which is normal for public transport).',
     fn:s=>(s.r.npv>=0?'+':'')+fE(s.r.npv),raw:s=>s.r.npv,b:'max'},
    {l:'EU grant received',   note:'How much of the build cost is covered by EU funds (Cohesion Fund, ERDF or CEF). This is money the city does not need to borrow or raise from local taxes.',
     fn:s=>s.r.euAmt>0?fE(s.r.euAmt):'None',raw:s=>s.r.euAmt,b:'max'},
  ];
  G('cmp-thead').innerHTML='<th style="min-width:200px">What we are measuring<br><span style="font-weight:400;font-size:9px;color:var(--ink3)">and what it means in plain English</span></th>'+scenarios.map(s=>`<th class="r" style="color:${s.col};min-width:110px">
    <div>${s.name}</div>
    <div style="font-size:9px;font-weight:500;background:${s.col}18;border-radius:5px;padding:2px 5px;margin-top:3px;display:inline-block">${s.m.icon} ${s.m.name}</div>
  </th>`).join('');
  G('cmp-tbody').innerHTML=metrics.map(met=>{
    const raws=met.raw?scenarios.map(s=>met.raw(s)):null;
    const best=raws?(met.b==='min'?Math.min(...raws):Math.max(...raws)):null;
    return`<tr><td style="font-size:11px;font-weight:600;color:var(--ink2);padding-right:8px"><div>${met.l}</div>${met.note?`<div style="font-size:9px;color:var(--ink3);font-weight:400;line-height:1.4;margin-top:1px">${met.note}</div>`:''}</td>${scenarios.map((s,i)=>{const v=met.fn(s);const isBest=raws&&raws[i]===best&&scenarios.length>1;return`<td class="r">${v}${isBest?` <span style="background:var(--green-bg);color:var(--green);border:1px solid #8ed4aa;border-radius:5px;padding:1px 5px;font-size:8px;font-weight:700">BEST</span>`:''}</td>`;}).join('')}</tr>`;
  }).join('');
  setTimeout(()=>{drawCmpR();drawCmpF();if(scenarios.length>=2)runDecisionTree();},60);
}

/* ═══ PRESETS ═══ */
function preset(key){
  const P={
    affordable:{ticket:.6,sub:70,len:18,st:14,spd:2,fr:6,fnd:'public',fare:'zone',gr:1.5,mt:'underground',nl:1},
    eu_max:    {ticket:1.2,sub:40,len:18,st:14,spd:2,fr:6,fnd:'cohesion',fare:'zone',gr:1.5,mt:'underground',nl:1},
    fast:      {ticket:1.5,sub:40,len:18,st:14,spd:3,fr:6,fnd:'cef',fare:'zone',gr:1.5,mt:'elevated',nl:1},
    ambitious: {ticket:1.5,sub:40,len:45,st:35,spd:2,fr:6,fnd:'cohesion',fare:'zone',gr:1.5,mt:'underground',nl:1},
    free:      {ticket:.1,sub:85,len:18,st:14,spd:2,fr:6,fnd:'public',fare:'free',gr:1.5,mt:'underground',nl:1},
    twolines:  {ticket:1.2,sub:50,len:18,st:14,spd:2,fr:6,fnd:'cohesion',fare:'zone',gr:2.0,mt:'underground',nl:2},
    sequential:{ticket:1.2,sub:40,len:18,st:14,spd:2,fr:6,fnd:'cohesion',fare:'zone',gr:2.0,mt:'underground',nl:3},
  };
  const pp=P[key];if(!pp)return;
  G('s-ticket').value=pp.ticket;G('s-sub').value=pp.sub;G('s-length').value=pp.len;
  G('s-stations').value=pp.st;G('s-speed').value=pp.spd;G('s-freq').value=pp.fr;
  G('s-growth').value=pp.gr;G('s-fund').value=pp.fnd;G('s-fare').value=pp.fare;
  metroType=pp.mt;setMetroType(pp.mt);setLinesSlider(pp.nl||1);
  const names={affordable:'Low-fare social policy',eu_max:'Maximum EU co-funding',fast:'Accelerated construction',ambitious:'Ambitious long network',free:'Free public transport',twolines:'2 simultaneous lines',sequential:'Sequential build (L1 then L2)'};
  toast('Loaded: '+names[key]);
}

/* ═══ EXPORT ═══ */
function exportCSV(){
  if(!lastCalc)return;
  const {r,m}=lastCalc;
  const rows=[['Year','Passengers/day','Capacity/day','Revenue €M/yr','Costs €M/yr','Net €M/yr','Cumulative NPV €M']];
  r.years.forEach(d=>rows.push([d.y,d.riders,d.cap,d.fareRev.toFixed(2),d.opex.toFixed(2),d.net.toFixed(2),d.cumNPV.toFixed(2)]));
  const a=document.createElement('a');a.href='data:text/csv;charset=utf-8,'+encodeURIComponent(rows.map(r=>r.join(',')).join('\n'));a.download='transit-simulation-eu.csv';a.click();toast('Data exported!');
}

/* ═══ TOAST ═══ */
let _tt;
function toast(msg){const t=G('toast');t.textContent=msg;clearTimeout(_tt);requestAnimationFrame(()=>{t.style.opacity='1';t.style.transform='translateX(-50%) translateY(0)';});_tt=setTimeout(()=>{t.style.opacity='0';t.style.transform='translateX(-50%) translateY(10px)';},2600);}

/* ═══ INIT ═══ */
renderCityGrid();
renderTerrainGrid();
window.addEventListener('resize',()=>{clearTimeout(window._rt);window._rt=setTimeout(()=>{if(currentStep===3&&selCity)renderRecommend();if(currentStep===4&&selMode)upd();},140);});
</script>
</body>
</html>
