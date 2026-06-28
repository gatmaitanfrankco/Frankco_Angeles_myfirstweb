<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no"/>
<title>SaKay Bulacan</title>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800;900&family=Inter:wght@400;500;600&display=swap" rel="stylesheet"/>
<style>
:root{--navy:#0d2b4e;--blue:#1a4a7a;--sky:#2e7fc1;--gold:#f5a623;--amber:#e8871a;--white:#fff;--light:#f0f6ff;--muted:#6b7a90;--border:#dce6f0;--red:#dc3545;--green:#198754;--radius:14px;--shadow:0 4px 20px rgba(13,43,78,.13);}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;}
html,body{height:100%;overflow:hidden;}
body{font-family:'Inter',sans-serif;background:#0d2b4e;color:#1a2535;}
h1,h2,h3,h4{font-family:'Outfit',sans-serif;}
#phone{width:100vw;height:100vh;display:flex;flex-direction:column;background:var(--light);overflow:hidden;position:relative;}
.status-bar{background:var(--navy);padding:10px 20px 6px;display:flex;justify-content:space-between;align-items:center;flex-shrink:0;}
.status-time{color:#fff;font-size:13px;font-weight:700;font-family:'Outfit',sans-serif;}
.status-icons{display:flex;gap:6px;}
.status-icons span{color:#fff;font-size:12px;}
.screen{flex:1;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch;display:none;flex-direction:column;}
.screen.active{display:flex;}
#screen-splash{background:linear-gradient(160deg,#071825 0%,#0d2b4e 50%,#1a4a7a 100%);align-items:center;justify-content:center;text-align:center;padding:40px 30px;}
.splash-glow{width:110px;height:110px;border-radius:28px;background:linear-gradient(135deg,var(--gold),var(--amber));display:flex;align-items:center;justify-content:center;font-size:52px;margin:0 auto 24px;box-shadow:0 0 60px rgba(245,166,35,.45);animation:pulse 2.5s ease-in-out infinite;}
@keyframes pulse{0%,100%{box-shadow:0 0 60px rgba(245,166,35,.45);}50%{box-shadow:0 0 90px rgba(245,166,35,.7);}}
.splash-title{color:#fff;font-size:32px;font-weight:900;letter-spacing:-1px;margin-bottom:6px;}
.splash-sub{color:#93b8d8;font-size:14px;margin-bottom:6px;}
.splash-region{color:var(--gold);font-size:11px;font-weight:700;letter-spacing:1px;text-transform:uppercase;margin-bottom:40px;}
.splash-features{display:flex;gap:16px;margin-bottom:48px;justify-content:center;}
.sf{display:flex;flex-direction:column;align-items:center;gap:6px;}
.sf-icon{width:48px;height:48px;border-radius:14px;background:rgba(255,255,255,.08);display:flex;align-items:center;justify-content:center;font-size:22px;}
.sf-label{color:#93b8d8;font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:.5px;}
.btn-get-started{width:100%;padding:16px;border:none;border-radius:14px;background:linear-gradient(135deg,var(--gold),var(--amber));color:var(--navy);font-size:16px;font-weight:800;font-family:'Outfit',sans-serif;cursor:pointer;box-shadow:0 8px 30px rgba(245,166,35,.4);margin-bottom:14px;}
.btn-get-started:active{transform:scale(.97);}
.btn-sign-in-splash{width:100%;padding:14px;border:1.5px solid rgba(255,255,255,.2);border-radius:14px;background:transparent;color:#fff;font-size:15px;font-weight:700;font-family:'Outfit',sans-serif;cursor:pointer;}
.btn-sign-in-splash:active{background:rgba(255,255,255,.1);}
#screen-auth{background:linear-gradient(160deg,#071825 0%,#0d2b4e 100%);padding:0;}
.auth-scroll{flex:1;overflow-y:auto;padding:24px 20px 40px;}
.auth-back{background:rgba(255,255,255,.1);border:none;border-radius:10px;padding:8px 14px;color:#fff;font-size:13px;cursor:pointer;display:flex;align-items:center;gap:6px;margin-bottom:24px;font-family:'Outfit',sans-serif;font-weight:600;}
.auth-logo-row{display:flex;align-items:center;gap:14px;margin-bottom:28px;}
.auth-logo-box{width:52px;height:52px;border-radius:14px;background:linear-gradient(135deg,var(--gold),var(--amber));display:flex;align-items:center;justify-content:center;font-size:26px;box-shadow:0 6px 20px rgba(245,166,35,.4);}
.auth-logo-text h2{color:#fff;font-size:22px;font-weight:900;letter-spacing:-.5px;}
.auth-logo-text p{color:#93b8d8;font-size:12px;margin-top:2px;}
.auth-card{background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.1);border-radius:20px;padding:24px;backdrop-filter:blur(10px);}
.auth-tab-row{display:flex;background:rgba(0,0,0,.2);border-radius:12px;padding:4px;margin-bottom:22px;}
.auth-tab-btn{flex:1;padding:10px;border:none;border-radius:9px;font-size:13px;font-weight:700;font-family:'Outfit',sans-serif;cursor:pointer;background:transparent;color:#93b8d8;}
.auth-tab-btn.active{background:rgba(255,255,255,.12);color:#fff;}
.auth-panel{display:none;}
.auth-panel.active{display:block;}
.afield{margin-bottom:16px;}
.afield label{display:block;font-size:11px;font-weight:700;color:#93b8d8;text-transform:uppercase;letter-spacing:.5px;margin-bottom:7px;}
.ainput-wrap{position:relative;}
.ainput-icon{position:absolute;left:13px;top:50%;transform:translateY(-50%);font-size:16px;pointer-events:none;}
.ainput{width:100%;padding:13px 13px 13px 40px;border:1.5px solid rgba(255,255,255,.15);border-radius:11px;background:rgba(255,255,255,.08);color:#fff;font-size:14px;font-family:'Inter',sans-serif;outline:none;}
.ainput::placeholder{color:rgba(255,255,255,.35);}
.ainput:focus{border-color:var(--gold);background:rgba(255,255,255,.12);}
.arow2{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.btn-auth-submit{width:100%;padding:15px;border:none;border-radius:12px;background:linear-gradient(135deg,var(--gold),var(--amber));color:var(--navy);font-size:15px;font-weight:800;font-family:'Outfit',sans-serif;cursor:pointer;margin-top:4px;box-shadow:0 6px 20px rgba(245,166,35,.35);}
.btn-auth-submit:active{transform:scale(.97);}
.auth-global-err{color:#f87171;font-size:13px;margin-bottom:12px;text-align:center;}
.aerr{font-size:11px;color:#f87171;margin-top:5px;}
.demo-hint{background:rgba(245,166,35,.1);border:1px solid rgba(245,166,35,.25);border-radius:10px;padding:10px 14px;margin-top:16px;}
.demo-hint p{color:#f5a623;font-size:11px;font-weight:700;text-transform:uppercase;letter-spacing:.5px;margin-bottom:4px;}
.demo-hint span{color:#93b8d8;font-size:12px;line-height:1.6;}
#screen-app{background:var(--light);flex-direction:column;}
.app-header{background:linear-gradient(135deg,var(--navy),var(--blue));padding:14px 16px 0;flex-shrink:0;}
.app-header-top{display:flex;align-items:center;gap:10px;padding-bottom:10px;}
.app-logo-badge{width:38px;height:38px;border-radius:10px;background:var(--gold);display:flex;align-items:center;justify-content:center;font-size:19px;flex-shrink:0;}
.app-logo-text h1{font-size:17px;font-weight:900;color:#fff;letter-spacing:-.3px;}
.app-logo-text p{font-size:10px;color:#93b8d8;}
.app-header-right{margin-left:auto;display:flex;align-items:center;gap:8px;}
.hstat-mini{text-align:center;}
.hstat-mini span{display:block;font-size:15px;font-weight:800;color:var(--gold);font-family:'Outfit',sans-serif;line-height:1;}
.hstat-mini small{font-size:9px;color:#93b8d8;}
.user-chip{display:flex;align-items:center;gap:6px;background:rgba(255,255,255,.12);border-radius:999px;padding:4px 10px 4px 4px;border:1px solid rgba(255,255,255,.15);cursor:pointer;}
.user-av{width:26px;height:26px;border-radius:50%;background:var(--gold);display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:800;color:var(--navy);}
.user-chip span{font-size:11px;font-weight:600;color:#fff;max-width:70px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap;}
.nav-tabs{display:flex;border-top:1px solid rgba(255,255,255,.1);overflow-x:auto;scrollbar-width:none;}
.nav-tabs::-webkit-scrollbar{display:none;}
.nav-tab{flex:1;min-width:60px;padding:9px 4px;border:none;background:transparent;color:#93b8d8;cursor:pointer;font-size:9px;font-weight:700;font-family:'Outfit',sans-serif;text-transform:uppercase;letter-spacing:.3px;border-bottom:3px solid transparent;display:flex;flex-direction:column;align-items:center;gap:2px;}
.nav-tab .ti{font-size:18px;}
.nav-tab.active{color:#fff;border-bottom-color:var(--gold);}
.tab-views{flex:1;overflow:hidden;position:relative;}
.tab-view{position:absolute;inset:0;overflow-y:auto;overflow-x:hidden;-webkit-overflow-scrolling:touch;display:none;padding:14px;}
.tab-view.active{display:block;}
.card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);box-shadow:var(--shadow);overflow:hidden;margin-bottom:12px;}
.card-hd{padding:13px 15px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;}
.card-hd h3{font-size:13px;font-weight:700;color:var(--navy);}
.card-bd{padding:14px;}
.stat-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:14px;}
.stat-card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:13px;border-left:4px solid var(--sky);box-shadow:var(--shadow);}
.stat-card .si{font-size:20px;margin-bottom:5px;}
.stat-card .sv{font-size:22px;font-weight:900;font-family:'Outfit',sans-serif;color:var(--navy);}
.stat-card .sl{font-size:10px;font-weight:700;color:var(--muted);text-transform:uppercase;letter-spacing:.4px;margin-top:2px;}
.stat-card .ss{font-size:10px;color:var(--muted);margin-top:1px;}
.welcome-banner{background:linear-gradient(135deg,var(--navy),var(--blue));border-radius:var(--radius);padding:14px 16px;margin-bottom:12px;display:flex;align-items:center;gap:10px;}
.wb-icon{font-size:26px;flex-shrink:0;}
.wb-text h3{color:#fff;font-size:14px;font-weight:700;}
.wb-text p{color:#93b8d8;font-size:11px;margin-top:2px;}
.toolbar{display:flex;gap:8px;margin-bottom:12px;flex-wrap:wrap;}
.sw{flex:1;min-width:140px;position:relative;}
.sw input{width:100%;padding:9px 12px 9px 32px;border:1.5px solid var(--border);border-radius:9px;font-size:13px;background:var(--white);outline:none;font-family:'Inter',sans-serif;}
.sw input:focus{border-color:var(--sky);}
.si-ic{position:absolute;left:9px;top:50%;transform:translateY(-50%);font-size:13px;}
.btn{padding:9px 14px;border:none;border-radius:9px;cursor:pointer;font-size:12px;font-weight:700;font-family:'Outfit',sans-serif;white-space:nowrap;}
.btn-primary{background:linear-gradient(135deg,var(--navy),var(--blue));color:#fff;}
.btn-success{background:linear-gradient(135deg,#0d6a3f,var(--green));color:#fff;}
.btn-danger{background:var(--red);color:#fff;}
.btn-ghost{background:none;border:1.5px solid var(--border);color:var(--muted);}
.btn-icon{padding:7px 9px;font-size:14px;}
.item-card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:13px;margin-bottom:10px;display:flex;align-items:flex-start;gap:10px;box-shadow:0 2px 8px rgba(13,43,78,.06);}
.iico{width:40px;height:40px;border-radius:10px;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:18px;}
.ibody{flex:1;min-width:0;}
.ititle{font-size:13px;font-weight:700;color:var(--navy);margin-bottom:2px;display:flex;align-items:center;gap:6px;flex-wrap:wrap;}
.isub{font-size:11px;color:var(--muted);margin-bottom:5px;}
.imeta{display:flex;flex-wrap:wrap;gap:8px;font-size:11px;color:#445;}
.iact{display:flex;gap:5px;flex-shrink:0;}
.badge{display:inline-block;padding:2px 9px;border-radius:999px;font-size:10px;font-weight:700;font-family:'Outfit',sans-serif;}
.bg-green{background:#d1fae5;color:#065f46;}
.bg-red{background:#fee2e2;color:#991b1b;}
.bg-yellow{background:#fef3c7;color:#92400e;}
.bg-blue{background:#dbeafe;color:#1e40af;}
.bg-gray{background:#f3f4f6;color:#374151;}
.pill-row{display:flex;gap:6px;flex-wrap:wrap;margin-bottom:12px;}
.pill{padding:5px 12px;border-radius:999px;border:1.5px solid var(--border);background:var(--white);color:var(--muted);font-size:11px;font-weight:700;cursor:pointer;font-family:'Outfit',sans-serif;}
.pill.active{background:var(--navy);color:#fff;border-color:var(--navy);}
.stops-row{display:flex;flex-wrap:wrap;gap:4px;margin-top:6px;}
.stop-chip{background:var(--light);border:1px solid var(--border);border-radius:999px;padding:2px 9px;font-size:10px;color:var(--blue);}
.prog-row{display:flex;align-items:center;gap:8px;margin-bottom:8px;}
.prog-label{width:72px;font-size:11px;color:var(--muted);flex-shrink:0;}
.prog-bar{flex:1;background:var(--light);border-radius:999px;height:7px;overflow:hidden;}
.prog-fill{height:100%;border-radius:999px;background:linear-gradient(90deg,var(--navy),var(--sky));}
.prog-count{font-size:11px;font-weight:700;color:var(--navy);min-width:14px;text-align:right;}
.empty{text-align:center;padding:36px 20px;color:var(--muted);}
.empty-icon{font-size:36px;margin-bottom:8px;}
.empty p{font-size:12px;}
.ea-layer{display:flex;gap:10px;margin-bottom:10px;align-items:flex-start;}
.ea-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;margin-top:4px;}
.ea-lt{font-size:12px;font-weight:700;color:var(--navy);}
.ea-ld{font-size:11px;color:var(--muted);margin-top:1px;}
.modal-overlay{display:none;position:fixed;inset:0;background:rgba(13,43,78,.7);z-index:1000;align-items:flex-end;justify-content:center;}
.modal-overlay.open{display:flex;}
.modal{background:var(--white);border-radius:20px 20px 0 0;width:100%;max-height:92vh;overflow-y:auto;box-shadow:0 -8px 40px rgba(0,0,0,.3);animation:slideUp .25s ease;}
@keyframes slideUp{from{transform:translateY(100%);}to{transform:translateY(0);}}
.modal-handle{width:40px;height:4px;background:var(--border);border-radius:999px;margin:12px auto 0;}
.modal-hd{padding:16px 18px 14px;border-bottom:1px solid var(--border);display:flex;justify-content:space-between;align-items:center;position:sticky;top:0;background:var(--white);z-index:1;}
.modal-hd h3{font-size:16px;color:var(--navy);}
.modal-close{background:none;border:none;font-size:22px;cursor:pointer;color:var(--muted);padding:2px 6px;border-radius:6px;}
.modal-bd{padding:18px;}
.fg{margin-bottom:13px;}
.fl{display:block;font-size:10px;font-weight:700;color:#445;margin-bottom:5px;text-transform:uppercase;letter-spacing:.5px;}
.fc{width:100%;padding:10px 12px;border:1.5px solid var(--border);border-radius:9px;font-size:13px;background:#fafcff;outline:none;font-family:'Inter',sans-serif;}
.fc:focus{border-color:var(--sky);background:#fff;}
.fe{font-size:11px;color:var(--red);margin-top:3px;}
.frow{display:grid;grid-template-columns:1fr 1fr;gap:10px;}
.factions{display:flex;gap:10px;margin-top:4px;}
.factions .btn{flex:1;}
.fare-preview{background:linear-gradient(135deg,#eff6ff,#dbeafe);border:1px solid #bfdbfe;border-radius:9px;padding:10px 13px;margin-bottom:13px;font-size:12px;color:#1e40af;}
.confirm-msg{color:var(--muted);font-size:13px;margin-bottom:16px;line-height:1.5;}
.toast-container{position:fixed;bottom:80px;left:50%;transform:translateX(-50%);z-index:9999;display:flex;flex-direction:column;gap:8px;pointer-events:none;width:90%;max-width:340px;}
.toast{background:rgba(13,43,78,.95);color:#fff;padding:11px 16px;border-radius:12px;font-size:13px;font-weight:600;font-family:'Outfit',sans-serif;box-shadow:0 6px 24px rgba(0,0,0,.3);animation:fadeInToast .3s ease;text-align:center;}
@keyframes fadeInToast{from{opacity:0;transform:translateY(8px);}to{opacity:1;transform:translateY(0);}}
.planner-hero{background:linear-gradient(135deg,var(--navy) 0%,var(--blue) 60%,var(--sky) 100%);border-radius:var(--radius);padding:18px;margin-bottom:14px;position:relative;overflow:hidden;}
.planner-hero::before{content:"🚌";position:absolute;right:-12px;bottom:-12px;font-size:70px;opacity:.07;line-height:1;}
.planner-hero h2{color:#fff;font-size:16px;margin-bottom:3px;}
.planner-hero p{color:#93b8d8;font-size:11px;margin-bottom:14px;}
.loc-wrap{position:relative;margin-bottom:9px;}
.loc-wrap .loc-ic{position:absolute;left:12px;top:50%;transform:translateY(-50%);font-size:15px;z-index:1;}
.loc-wrap input{width:100%;padding:12px 12px 12px 36px;border:1.5px solid rgba(255,255,255,.2);border-radius:10px;font-size:13px;background:rgba(255,255,255,.12);color:#fff;outline:none;font-family:'Inter',sans-serif;}
.loc-wrap input::placeholder{color:rgba(255,255,255,.45);}
.loc-wrap input:focus{background:rgba(255,255,255,.2);border-color:var(--gold);}
.swap-btn{display:flex;align-items:center;justify-content:center;width:30px;height:30px;border-radius:50%;background:rgba(255,255,255,.13);border:1.5px solid rgba(255,255,255,.22);color:#fff;cursor:pointer;font-size:15px;margin:0 auto 9px;}
.btn-search-trip{width:100%;padding:13px;border:none;border-radius:10px;background:var(--gold);color:var(--navy);font-size:14px;font-weight:800;font-family:'Outfit',sans-serif;cursor:pointer;}
.ac-list{position:absolute;top:100%;left:0;right:0;z-index:300;background:#fff;border:1.5px solid var(--border);border-top:none;border-radius:0 0 10px 10px;max-height:160px;overflow-y:auto;box-shadow:0 8px 24px rgba(0,0,0,.12);}
.ac-item{padding:9px 13px;font-size:12px;cursor:pointer;color:var(--navy);}
.ac-item:hover{background:var(--light);}
.trip-result-card{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);overflow:hidden;margin-bottom:12px;box-shadow:var(--shadow);}
.trh{padding:11px 14px;display:flex;align-items:center;gap:9px;border-bottom:1px solid var(--border);}
.tr-icon{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;font-size:17px;flex-shrink:0;}
.tr-name{font-size:13px;font-weight:700;color:var(--navy);}
.tr-code{font-size:10px;color:var(--muted);}
.trip-journey{padding:12px 14px;}
.journey-step{display:flex;gap:9px;position:relative;}
.journey-step:not(:last-child)::after{content:"";position:absolute;left:10px;top:22px;width:2px;height:calc(100% - 4px);background:var(--border);}
.step-dot{width:22px;height:22px;border-radius:50%;flex-shrink:0;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:800;z-index:1;margin-top:2px;}
.step-dot.origin{background:var(--gold);color:var(--navy);}
.step-dot.stop{background:var(--border);color:var(--muted);}
.step-dot.dest{background:var(--sky);color:#fff;}
.step-label{font-size:12px;padding-bottom:12px;line-height:1.4;}
.step-label strong{color:var(--navy);}
.step-tag{font-size:10px;color:var(--muted);display:block;}
.trip-footer{padding:9px 14px;background:var(--light);border-top:1px solid var(--border);display:flex;gap:10px;align-items:center;flex-wrap:wrap;}
.trip-footer span{font-size:11px;color:#445;}
.book-this-btn{margin-left:auto;padding:7px 14px;background:linear-gradient(135deg,#0d6a3f,var(--green));color:#fff;border:none;border-radius:8px;font-size:11px;font-weight:700;font-family:'Outfit',sans-serif;cursor:pointer;}
.no-results{background:var(--white);border-radius:var(--radius);border:1px solid var(--border);padding:28px 16px;text-align:center;color:var(--muted);}
.no-results .nr-icon{font-size:32px;margin-bottom:8px;}
.no-results p{font-size:12px;line-height:1.6;}
.muni-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;}
.muni-card{background:var(--light);border:1px solid var(--border);border-radius:10px;padding:10px 11px;}
.muni-name{font-size:12px;font-weight:700;color:var(--navy);}
.muni-type-row{display:flex;align-items:center;gap:5px;margin-top:3px;}
.muni-pop{font-size:10px;color:var(--muted);margin-top:2px;}
.bottom-nav{background:var(--white);border-top:1px solid var(--border);display:flex;flex-shrink:0;box-shadow:0 -4px 20px rgba(13,43,78,.08);}
.profile-sheet{background:rgba(13,43,78,.7);position:fixed;inset:0;z-index:900;display:none;align-items:flex-end;}
.profile-sheet.open{display:flex;}
.profile-panel{background:var(--white);border-radius:20px 20px 0 0;width:100%;padding:0 0 20px;animation:slideUp .25s ease;}
.profile-hero{background:linear-gradient(135deg,var(--navy),var(--blue));padding:20px 20px 24px;border-radius:20px 20px 0 0;text-align:center;}
.profile-av-big{width:72px;height:72px;border-radius:50%;background:var(--gold);display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:900;color:var(--navy);margin:0 auto 12px;box-shadow:0 6px 20px rgba(245,166,35,.4);}
.profile-name{color:#fff;font-size:20px;font-weight:800;}
.profile-email{color:#93b8d8;font-size:12px;margin-top:3px;}
.profile-muni{display:inline-block;background:rgba(245,166,35,.2);border:1px solid rgba(245,166,35,.4);color:var(--gold);font-size:11px;font-weight:700;padding:4px 12px;border-radius:999px;margin-top:8px;}
.profile-stats{display:flex;border-bottom:1px solid var(--border);}
.ps-item{flex:1;text-align:center;padding:16px 8px;border-right:1px solid var(--border);}
.ps-item:last-child{border-right:none;}
.ps-val{font-size:20px;font-weight:900;font-family:'Outfit',sans-serif;color:var(--navy);}
.ps-lbl{font-size:10px;color:var(--muted);text-transform:uppercase;letter-spacing:.5px;margin-top:2px;}
.profile-actions{padding:16px 20px 0;}
.btn-logout-big{width:100%;padding:14px;border-radius:12px;border:none;background:#fee2e2;color:#991b1b;font-size:14px;font-weight:800;font-family:'Outfit',sans-serif;cursor:pointer;margin-bottom:10px;}
.btn-close-profile{width:100%;padding:13px;border-radius:12px;border:1.5px solid var(--border);background:transparent;color:var(--muted);font-size:13px;font-weight:700;font-family:'Outfit',sans-serif;cursor:pointer;}
</style>
</head>
<body>
<div id="phone">
<div class="status-bar"><div class="status-time" id="status-time">9:41</div><div class="status-icons"><span>📶</span><span>🔋</span></div></div>

<div class="screen active" id="screen-splash" style="overflow-y:auto;">
<div style="display:flex;flex-direction:column;align-items:center;justify-content:center;padding:40px 28px;min-height:100%;text-align:center;background:linear-gradient(160deg,#071825 0%,#0d2b4e 50%,#1a4a7a 100%);">
<div class="splash-glow">🚌</div>
<div class="splash-title">SaKay Bulacan</div>
<div class="splash-sub">Online SaKay System</div>
<div class="splash-region">🏛 Province of Bulacan · Region III</div>
<div class="splash-features">
<div class="sf"><div class="sf-icon">🗺</div><div class="sf-label">Routes</div></div>
<div class="sf"><div class="sf-icon">🎫</div><div class="sf-label">Bookings</div></div>
<div class="sf"><div class="sf-icon">📍</div><div class="sf-label">Trip Plan</div></div>
<div class="sf"><div class="sf-icon">🏛</div><div class="sf-label">Towns</div></div>
</div>
<button class="btn-get-started" onclick="goToAuth('signup')">Get Started →</button>
<button class="btn-sign-in-splash" onclick="goToAuth('login')">I already have an account</button>
</div></div>

<div class="screen" id="screen-auth"><div class="auth-scroll">
<button class="auth-back" onclick="showScreen('screen-splash')">← Back</button>
<div class="auth-logo-row"><div class="auth-logo-box">🚌</div><div class="auth-logo-text"><h2>SaKay Bulacan</h2><p>Province of Bulacan · Region III</p></div></div>
<div class="auth-card">
<div class="auth-tab-row">
<button class="auth-tab-btn active" id="at-login" onclick="switchAuthTab('login')">Sign In</button>
<button class="auth-tab-btn" id="at-signup" onclick="switchAuthTab('signup')">Create Account</button>
</div>
<div class="auth-panel active" id="panel-login">
<div class="afield"><label>Email Address</label><div class="ainput-wrap"><span class="ainput-icon">📧</span><input class="ainput" id="l-email" type="email" placeholder="you@email.com" autocomplete="email"/></div><div class="aerr" id="le-email"></div></div>
<div class="afield"><label>Password</label><div class="ainput-wrap"><span class="ainput-icon">🔒</span><input class="ainput" id="l-password" type="password" placeholder="Your password" autocomplete="current-password"/></div><div class="aerr" id="le-password"></div></div>
<div class="auth-global-err" id="le-global"></div>
<button class="btn-auth-submit" onclick="doLogin()">Sign In →</button>
<div class="demo-hint"><p>Demo Account</p><span>Email: <strong>admin@sakay.ph</strong><br>Password: <strong>bulacan2025</strong></span></div>
</div>
<div class="auth-panel" id="panel-signup">
<div class="arow2">
<div class="afield"><label>First Name</label><div class="ainput-wrap"><span class="ainput-icon">👤</span><input class="ainput" id="s-fname" type="text" placeholder="Juan"/></div><div class="aerr" id="se-fname"></div></div>
<div class="afield"><label>Last Name</label><div class="ainput-wrap"><span class="ainput-icon">👤</span><input class="ainput" id="s-lname" type="text" placeholder="dela Cruz"/></div><div class="aerr" id="se-lname"></div></div>
</div>
<div class="afield"><label>Email Address</label><div class="ainput-wrap"><span class="ainput-icon">📧</span><input class="ainput" id="s-email" type="email" placeholder="you@email.com"/></div><div class="aerr" id="se-email"></div></div>
<div class="afield"><label>Municipality / City</label><div class="ainput-wrap"><span class="ainput-icon">📍</span><select class="ainput" id="s-muni" style="padding-left:36px"><option value="">— Select your municipality —</option></select></div><div class="aerr" id="se-muni"></div></div>
<div class="afield"><label>Password</label><div class="ainput-wrap"><span class="ainput-icon">🔒</span><input class="ainput" id="s-password" type="password" placeholder="Min. 6 characters"/></div><div class="aerr" id="se-password"></div></div>
<div class="afield"><label>Confirm Password</label><div class="ainput-wrap"><span class="ainput-icon">🔒</span><input class="ainput" id="s-confirm" type="password" placeholder="Repeat password"/></div><div class="aerr" id="se-confirm"></div></div>
<div class="auth-global-err" id="se-global"></div>
<button class="btn-auth-submit" onclick="doSignup()">Create Account →</button>
</div>
</div></div></div>

<div class="screen" id="screen-app">
<div class="app-header">
<div class="app-header-top">
<div class="app-logo-badge">🚌</div>
<div class="app-logo-text"><h1>SaKay Bulacan</h1><p>Online Transit System</p></div>
<div class="app-header-right">
<div class="hstat-mini"><span id="hs-routes">0</span><small>Routes</small></div>
<div class="hstat-mini"><span id="hs-bookings">0</span><small>Bookings</small></div>
<div class="user-chip" onclick="openProfile()"><div class="user-av" id="user-av">?</div><span id="user-name-display">User</span></div>
</div>
</div>
<div class="nav-tabs">
<button class="nav-tab active" onclick="switchTab('dashboard')" id="tab-dashboard"><span class="ti">📊</span>Dashboard</button>
<button class="nav-tab" onclick="switchTab('routes')" id="tab-routes"><span class="ti">🗺</span>Routes</button>
<button class="nav-tab" onclick="switchTab('bookings')" id="tab-bookings"><span class="ti">🎫</span>Bookings</button>
<button class="nav-tab" onclick="switchTab('planner')" id="tab-planner"><span class="ti">📍</span>Planner</button>
<button class="nav-tab" onclick="switchTab('municipalities')" id="tab-municipalities"><span class="ti">🏛</span>Towns</button>
</div>
</div>

<div class="tab-views">
<div class="tab-view active" id="view-dashboard">
<div id="welcome-banner-wrap"></div>
<div class="stat-grid">
<div class="stat-card" style="border-left-color:#0d2b4e"><div class="si">🗺</div><div class="sv" id="d-routes">0</div><div class="sl">Total Routes</div><div class="ss" id="d-routes-sub"></div></div>
<div class="stat-card" style="border-left-color:#198754"><div class="si">🎫</div><div class="sv" id="d-bookings">0</div><div class="sl">Bookings</div><div class="ss" id="d-bookings-sub"></div></div>
<div class="stat-card" style="border-left-color:#f5a623"><div class="si">💰</div><div class="sv" id="d-revenue">₱0</div><div class="sl">Revenue</div><div class="ss">confirmed</div></div>
<div class="stat-card" style="border-left-color:#dc3545"><div class="si">⏳</div><div class="sv" id="d-pending">0</div><div class="sl">Pending</div><div class="ss">awaiting</div></div>
</div>
<div class="card"><div class="card-hd"><h3>Fleet by Transport Type</h3></div><div class="card-bd" id="fleet-chart"></div></div>
<div class="card"><div class="card-hd"><h3>🏛 EA Architecture</h3></div><div class="card-bd">
<div class="ea-layer"><div class="ea-dot" style="background:#2e7fc1"></div><div><div class="ea-lt">Application Architecture</div><div class="ea-ld">Modular tab-based SPA; vanilla JS CRUD; auth session layer</div></div></div>
<div class="ea-layer"><div class="ea-dot" style="background:#198754"></div><div><div class="ea-lt">Data Architecture</div><div class="ea-ld">Normalized Routes & Bookings; Users registry; referential integrity</div></div></div>
<div class="ea-layer"><div class="ea-dot" style="background:#8b5cf6"></div><div><div class="ea-lt">Technology Architecture</div><div class="ea-ld">HTML5 + CSS3 mobile SPA; Google Fonts; zero external dependencies</div></div></div>
<div class="ea-layer"><div class="ea-dot" style="background:#f5a623"></div><div><div class="ea-lt">IT Governance & Security</div><div class="ea-ld">Auth gate; session validation; input validation; delete confirmation</div></div></div>
</div></div>
<div class="card"><div class="card-hd"><h3>📍 Coverage Areas</h3></div><div class="card-bd"><div class="stops-row" id="coverage-areas"></div></div></div>
</div>

<div class="tab-view" id="view-routes">
<div class="toolbar"><div class="sw"><span class="si-ic">🔍</span><input type="text" placeholder="Search routes, codes…" oninput="renderRoutes()" id="route-search"/></div><button class="btn btn-primary" onclick="openRouteModal()">＋ Add</button></div>
<div id="routes-list"></div>
</div>

<div class="tab-view" id="view-bookings">
<div class="pill-row" id="booking-filters">
<button class="pill active" onclick="setBookingFilter('All',this)">All</button>
<button class="pill" onclick="setBookingFilter('Confirmed',this)">Confirmed</button>
<button class="pill" onclick="setBookingFilter('Pending',this)">Pending</button>
<button class="pill" onclick="setBookingFilter('Cancelled',this)">Cancelled</button>
</div>
<div class="toolbar"><div class="sw"><span class="si-ic">🔍</span><input type="text" placeholder="Search passenger, ref…" oninput="renderBookings()" id="booking-search"/></div><button class="btn btn-success" onclick="openBookingModal()">＋ Book</button></div>
<div id="bookings-list"></div>
</div>

<div class="tab-view" id="view-planner">
<div class="planner-hero">
<h2>🗺 Plan Your Trip</h2><p>Find the best route from your location to your destination</p>
<div class="loc-wrap" style="position:relative"><span class="loc-ic">📍</span><input type="text" id="trip-from" placeholder="Current location (e.g. Malolos)" oninput="acSuggest('trip-from','ac-from')" autocomplete="off"/><div class="ac-list" id="ac-from" style="display:none"></div></div>
<button class="swap-btn" onclick="swapLocations()">⇅</button>
<div class="loc-wrap" style="position:relative"><span class="loc-ic">🏁</span><input type="text" id="trip-to" placeholder="Destination (e.g. Trinoma)" oninput="acSuggest('trip-to','ac-to')" autocomplete="off"/><div class="ac-list" id="ac-to" style="display:none"></div></div>
<div style="height:10px"></div>
<button class="btn-search-trip" onclick="searchTrip()">Search Routes →</button>
</div>
<div id="trip-results"></div>
</div>

<div class="tab-view" id="view-municipalities">
<div class="card" style="margin-bottom:12px">
<div class="card-hd"><h3>🏛 All Municipalities & Cities</h3><span class="badge bg-blue" id="muni-count-badge">24</span></div>
<div class="card-bd">
<p style="font-size:11px;color:var(--muted);margin-bottom:12px">Bulacan — 1st class province, Region III. 3 cities · 21 municipalities.</p>
<div class="toolbar" style="margin-bottom:10px"><div class="sw"><span class="si-ic">🔍</span><input type="text" id="muni-search" placeholder="Search municipality…" oninput="renderMunicipalities()"/></div></div>
<div class="pill-row" style="margin-bottom:12px">
<button class="pill active" onclick="setMuniFilter('all',this)">All</button>
<button class="pill" onclick="setMuniFilter('City',this)">Cities</button>
<button class="pill" onclick="setMuniFilter('Municipality',this)">Municipalities</button>
</div>
<div class="muni-grid" id="muni-grid"></div>
</div></div>
</div>
</div></div></div>

<div class="modal-overlay" id="route-modal"><div class="modal">
<div class="modal-handle"></div>
<div class="modal-hd"><h3 id="route-modal-title">Add Route</h3><button class="modal-close" onclick="closeModal('route-modal')">×</button></div>
<div class="modal-bd">
<div class="frow">
<div class="fg"><label class="fl">Route Code</label><input class="fc" id="f-code" placeholder="BUL-001"/><div class="fe" id="e-code"></div></div>
<div class="fg"><label class="fl">Transport Type</label><select class="fc" id="f-type"><option>Jeepney</option><option>Bus</option><option>UV Express</option><option>Tricycle</option><option>FX / AUV</option><option>E-Jeep</option></select></div>
</div>
<div class="fg"><label class="fl">Route Name (Origin → Destination)</label><input class="fc" id="f-name" placeholder="Malolos → Trinoma"/><div class="fe" id="e-name"></div></div>
<div class="frow">
<div class="fg"><label class="fl">Fare (₱)</label><input class="fc" id="f-fare" type="number" min="1" placeholder="30"/><div class="fe" id="e-fare"></div></div>
<div class="fg"><label class="fl">Duration (mins)</label><input class="fc" id="f-duration" type="number" min="1" placeholder="60"/><div class="fe" id="e-duration"></div></div>
</div>
<div class="fg"><label class="fl">Stops (comma-separated)</label><input class="fc" id="f-stops" placeholder="Malolos, Calumpit, Plaridel…"/></div>
<div class="fg"><label class="fl">Status</label><select class="fc" id="f-status"><option>Active</option><option>Inactive</option></select></div>
<div class="factions"><button class="btn btn-ghost" onclick="closeModal('route-modal')">Cancel</button><button class="btn btn-primary" onclick="saveRoute()">Save Route</button></div>
</div></div></div>

<div class="modal-overlay" id="booking-modal"><div class="modal">
<div class="modal-handle"></div>
<div class="modal-hd"><h3 id="booking-modal-title">New Booking</h3><button class="modal-close" onclick="closeModal('booking-modal')">×</button></div>
<div class="modal-bd">
<div class="fg"><label class="fl">Passenger Name</label><input class="fc" id="b-passenger" placeholder="Juan dela Cruz"/><div class="fe" id="be-passenger"></div></div>
<div class="frow">
<div class="fg"><label class="fl">📍 From</label><input class="fc" id="b-from" placeholder="e.g. Malolos" oninput="bookingAcSuggest('b-from','bac-from')" autocomplete="off"/><div class="ac-list" id="bac-from" style="display:none;position:absolute;z-index:400"></div></div>
<div class="fg"><label class="fl">🏁 To</label><input class="fc" id="b-to" placeholder="e.g. Trinoma" oninput="bookingAcSuggest('b-to','bac-to')" autocomplete="off"/><div class="ac-list" id="bac-to" style="display:none;position:absolute;z-index:400"></div></div>
</div>
<div class="fg"><label class="fl">Select Route</label><select class="fc" id="b-route" onchange="updateFarePreview()"><option value="">— Choose a route —</option></select><div class="fe" id="be-route"></div></div>
<div id="fare-preview-box" class="fare-preview" style="display:none"></div>
<div class="frow">
<div class="fg"><label class="fl">Travel Date</label><input class="fc" id="b-date" type="date"/><div class="fe" id="be-date"></div></div>
<div class="fg"><label class="fl">Departure Time</label><input class="fc" id="b-time" type="time"/><div class="fe" id="be-time"></div></div>
</div>
<div class="frow">
<div class="fg"><label class="fl">Seats</label><input class="fc" id="b-seats" type="number" min="1" max="20" value="1" oninput="updateFarePreview()"/><div class="fe" id="be-seats"></div></div>
<div class="fg"><label class="fl">Status</label><select class="fc" id="b-status"><option>Pending</option><option>Confirmed</option><option>Cancelled</option></select></div>
</div>
<div class="factions"><button class="btn btn-ghost" onclick="closeModal('booking-modal')">Cancel</button><button class="btn btn-success" onclick="saveBooking()">Book Now</button></div>
</div></div></div>

<div class="modal-overlay" id="confirm-modal"><div class="modal">
<div class="modal-handle"></div>
<div class="modal-hd"><h3 id="confirm-title">Confirm</h3><button class="modal-close" onclick="closeModal('confirm-modal')">×</button></div>
<div class="modal-bd"><p class="confirm-msg" id="confirm-msg"></p>
<div class="factions"><button class="btn btn-ghost" onclick="closeModal('confirm-modal')">Cancel</button><button class="btn btn-danger" id="confirm-ok-btn">Delete</button></div>
</div></div></div>

<div class="profile-sheet" id="profile-sheet" onclick="closeProfile(event)"><div class="profile-panel">
<div class="profile-hero">
<div class="profile-av-big" id="profile-av">?</div>
<div class="profile-name" id="profile-name">User</div>
<div class="profile-email" id="profile-email">user@email.com</div>
<div class="profile-muni" id="profile-muni">Bulacan</div>
</div>
<div class="profile-stats">
<div class="ps-item"><div class="ps-val" id="ps-bookings">0</div><div class="ps-lbl">Bookings</div></div>
<div class="ps-item"><div class="ps-val" id="ps-routes">0</div><div class="ps-lbl">Routes</div></div>
<div class="ps-item"><div class="ps-val" id="ps-revenue">₱0</div><div class="ps-lbl">Revenue</div></div>
</div>
<div class="profile-actions">
<button class="btn-logout-big" onclick="doLogout()">🚪 Sign Out</button>
<button class="btn-close-profile" onclick="closeProfile()">Close</button>
</div>
</div></div>

<div class="toast-container" id="toasts"></div>

<script>
// ── DATA: Municipalities ──
const MUNICIPALITIES=[
{name:"Malolos",type:"City",district:"1st",population:282428,icon:"🏙"},
{name:"Meycauayan",type:"City",district:"2nd",population:366493,icon:"🏙"},
{name:"San Jose del Monte",type:"City",district:"5th",population:651813,icon:"🏙"},
{name:"Angat",type:"Municipality",district:"4th",population:53699,icon:"🏘"},
{name:"Balagtas",type:"Municipality",district:"2nd",population:128064,icon:"🏘"},
{name:"Baliuag",type:"Municipality",district:"3rd",population:203510,icon:"🏘"},
{name:"Bocaue",type:"Municipality",district:"2nd",population:131666,icon:"🏘"},
{name:"Bulacan",type:"Municipality",district:"2nd",population:80478,icon:"🏘"},
{name:"Calumpit",type:"Municipality",district:"1st",population:134052,icon:"🏘"},
{name:"Doña Remedios Trinidad",type:"Municipality",district:"4th",population:11907,icon:"🏘"},
{name:"Guiguinto",type:"Municipality",district:"2nd",population:115829,icon:"🏘"},
{name:"Hagonoy",type:"Municipality",district:"1st",population:130709,icon:"🏘"},
{name:"Marilao",type:"Municipality",district:"2nd",population:218898,icon:"🏘"},
{name:"Norzagaray",type:"Municipality",district:"4th",population:126342,icon:"🏘"},
{name:"Obando",type:"Municipality",district:"2nd",population:75455,icon:"🏘"},
{name:"Pandi",type:"Municipality",district:"5th",population:100042,icon:"🏘"},
{name:"Paombong",type:"Municipality",district:"1st",population:60534,icon:"🏘"},
{name:"Plaridel",type:"Municipality",district:"3rd",population:133217,icon:"🏘"},
{name:"Pulilan",type:"Municipality",district:"3rd",population:130501,icon:"🏘"},
{name:"San Ildefonso",type:"Municipality",district:"3rd",population:128421,icon:"🏘"},
{name:"San Miguel",type:"Municipality",district:"4th",population:151624,icon:"🏘"},
{name:"San Rafael",type:"Municipality",district:"4th",population:112890,icon:"🏘"},
{name:"Sta. Maria",type:"Municipality",district:"5th",population:251478,icon:"🏘"},
];
const MUNIS_UNIQUE=MUNICIPALITIES.filter((m,i,a)=>a.findIndex(x=>x.name===m.name)===i);

// ── AUTH ──
let users=[{id:1,fname:"Admin",lname:"SaKay",email:"admin@sakay.ph",password:"bulacan2025",municipality:"Malolos",role:"admin"}];
let currentUser=null;
function hashPw(pw){return btoa(pw+"sakay_bulacan_2025");}
function switchAuthTab(tab){
  ["login","signup"].forEach(t=>{document.getElementById("at-"+t).classList.toggle("active",t===tab);document.getElementById("panel-"+t).classList.toggle("active",t===tab);});
  ["le-email","le-password","le-global","se-fname","se-lname","se-email","se-muni","se-password","se-confirm","se-global"].forEach(id=>{const el=document.getElementById(id);if(el)el.textContent="";});
}
function goToAuth(tab){showScreen("screen-auth");switchAuthTab(tab||"login");}
function doLogin(){
  const email=document.getElementById("l-email").value.trim().toLowerCase();
  const pw=document.getElementById("l-password").value;
  let v=true;const e=(id,m)=>{document.getElementById(id).textContent=m;v=false;};const c=id=>document.getElementById(id).textContent="";
  email?c("le-email"):e("le-email","Email is required");
  pw?c("le-password"):e("le-password","Password is required");
  if(!v)return;
  const user=users.find(u=>u.email.toLowerCase()===email&&(u.password===pw||u.password===hashPw(pw)));
  if(!user){document.getElementById("le-global").textContent="❌ Incorrect email or password.";return;}
  currentUser=user;launchApp();
}
function doSignup(){
  const fname=document.getElementById("s-fname").value.trim(),lname=document.getElementById("s-lname").value.trim();
  const email=document.getElementById("s-email").value.trim().toLowerCase(),muni=document.getElementById("s-muni").value;
  const pw=document.getElementById("s-password").value,conf=document.getElementById("s-confirm").value;
  let v=true;const e=(id,m)=>{document.getElementById(id).textContent=m;v=false;};const c=id=>document.getElementById(id).textContent="";
  fname?c("se-fname"):e("se-fname","Required");
  lname?c("se-lname"):e("se-lname","Required");
  /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email)?c("se-email"):e("se-email","Valid email required");
  muni?c("se-muni"):e("se-muni","Please select your municipality");
  pw.length>=6?c("se-password"):e("se-password","Min. 6 characters");
  pw===conf?c("se-confirm"):e("se-confirm","Passwords do not match");
  if(!v)return;
  if(users.find(u=>u.email.toLowerCase()===email)){document.getElementById("se-global").textContent="❌ Email already registered.";return;}
  const nu={id:users.length+1,fname,lname,email,password:hashPw(pw),municipality:muni,role:"user"};
  users.push(nu);currentUser=nu;launchApp();
}
function doLogout(){
  currentUser=null;closeProfile();showScreen("screen-splash");
  document.getElementById("l-email").value="";document.getElementById("l-password").value="";
  showToast("👋 Signed out");
}
function launchApp(){
  populateMunicipalityDropdowns();showScreen("screen-app");
  const initials=(currentUser.fname[0]+(currentUser.lname||"")[0]||"").toUpperCase();
  document.getElementById("user-av").textContent=initials;
  document.getElementById("user-name-display").textContent=currentUser.fname;
  renderDashboard();renderMunicipalities();updateHeaderStats();
}

// ── SCREEN ROUTING ──
function showScreen(id){document.querySelectorAll(".screen").forEach(s=>s.classList.remove("active"));document.getElementById(id).classList.add("active");}

// ── DATA: Routes & Bookings ──
let routes=[
{id:1,code:"BUL-001",name:"Malolos → EDSA Monumento",type:"Bus",fare:55,duration:75,stops:["Malolos City Hall","Calumpit","Meycauayan","Valenzuela","EDSA Monumento"],status:"Active",createdAt:"2025-01-05"},
{id:2,code:"BUL-002",name:"San Jose del Monte → Trinoma (via NLEX)",type:"Bus",fare:130,duration:90,stops:["San Jose del Monte","Bocaue","Marilao","Meycauayan","NLEX","Trinoma"],status:"Active",createdAt:"2025-01-08"},
{id:3,code:"BUL-003",name:"Malolos → Bocaue",type:"Jeepney",fare:18,duration:35,stops:["Malolos Supermarket","Calumpit Junction","Hagonoy Road","Bocaue Palengke"],status:"Active",createdAt:"2025-01-10"},
{id:4,code:"BUL-004",name:"San Jose del Monte → Fairview",type:"UV Express",fare:65,duration:50,stops:["SJDM City Hall","Muzon","Sta. Maria","Fairview"],status:"Active",createdAt:"2025-01-12"},
{id:5,code:"BUL-005",name:"Balagtas → Cubao",type:"FX / AUV",fare:80,duration:65,stops:["Balagtas","Guiguinto","Marilao","Meycauayan","Cubao"],status:"Active",createdAt:"2025-01-15"},
{id:6,code:"BUL-006",name:"Plaridel → Malolos",type:"Tricycle",fare:12,duration:20,stops:["Plaridel Town Center","Pulilan","Calumpit","Malolos"],status:"Active",createdAt:"2025-01-18"},
{id:7,code:"BUL-007",name:"Bulacan E-Jeep (Malolos Loop)",type:"E-Jeep",fare:10,duration:25,stops:["Malolos Station","Barasoain","Paseo de Malolos","City Hall","Malolos Station"],status:"Inactive",createdAt:"2025-02-01"},
{id:8,code:"BUL-008",name:"Baliuag → Cubao",type:"Bus",fare:95,duration:80,stops:["Baliuag","San Ildefonso","Plaridel","Bocaue","NLEX","Cubao"],status:"Active",createdAt:"2025-02-10"},
{id:9,code:"BUL-009",name:"Norzagaray → Fairview",type:"UV Express",fare:70,duration:55,stops:["Norzagaray","Angat","San Rafael","Fairview"],status:"Active",createdAt:"2025-03-01"},
{id:10,code:"BUL-010",name:"Obando → Navotas",type:"Jeepney",fare:22,duration:30,stops:["Obando","Paombong","Hagonoy","Navotas Fish Port"],status:"Active",createdAt:"2025-03-15"},
];
let bookings=[
{id:1,ref:"SK-2025-001",passenger:"Nike Manalansan",routeId:1,route:"Malolos → EDSA Monumento",date:"2025-06-28",time:"06:00",seats:1,fare:55,status:"Confirmed"},
{id:2,ref:"SK-2025-002",passenger:"Angeles Frankco",routeId:2,route:"San Jose del Monte → Trinoma (via NLEX)",date:"2025-06-28",time:"07:30",seats:2,fare:260,status:"Pending"},
{id:3,ref:"SK-2025-003",passenger:"Ana Reyes Bulacan",routeId:4,route:"San Jose del Monte → Fairview",date:"2025-06-29",time:"08:00",seats:1,fare:65,status:"Confirmed"},
{id:4,ref:"SK-2025-004",passenger:"Pedro Mabini Garcia",routeId:3,route:"Malolos → Bocaue",date:"2025-06-29",time:"09:15",seats:3,fare:54,status:"Pending"},
];
let bookingFilter="All",editingRouteId=null,editingBookingId=null,muniFilter="all";
let nextRouteId=11,nextBookingId=5,nextRefNum=5;

// ── DROPDOWNS ──
function populateMunicipalityDropdowns(){
  const sel=document.getElementById("s-muni");if(!sel)return;
  sel.innerHTML='<option value="">— Select your municipality —</option>';
  const cities=MUNIS_UNIQUE.filter(m=>m.type==="City"),munis=MUNIS_UNIQUE.filter(m=>m.type==="Municipality");
  const og1=document.createElement("optgroup");og1.label="🏙 Cities";
  cities.forEach(m=>{const o=document.createElement("option");o.value=m.name;o.textContent=m.name+" (City)";og1.appendChild(o);});
  const og2=document.createElement("optgroup");og2.label="🏘 Municipalities";
  munis.forEach(m=>{const o=document.createElement("option");o.value=m.name;o.textContent=m.name;og2.appendChild(o);});
  sel.appendChild(og1);sel.appendChild(og2);
}
populateMunicipalityDropdowns();

// ── TAB SWITCHING ──
function switchTab(tab){
  ["dashboard","routes","bookings","planner","municipalities"].forEach(t=>{
    document.getElementById("view-"+t).classList.toggle("active",t===tab);
    document.getElementById("tab-"+t).classList.toggle("active",t===tab);
  });
  if(tab==="dashboard")renderDashboard();
  if(tab==="routes")renderRoutes();
  if(tab==="bookings")renderBookings();
  if(tab==="planner")document.getElementById("trip-results").innerHTML="";
  if(tab==="municipalities")renderMunicipalities();
}

// ── DASHBOARD ──
function renderDashboard(){
  if(!currentUser)return;
  const activeR=routes.filter(r=>r.status==="Active").length;
  const confirmedB=bookings.filter(b=>b.status==="Confirmed").length;
  const revenue=bookings.filter(b=>b.status==="Confirmed").reduce((s,b)=>s+b.fare,0);
  const pending=bookings.filter(b=>b.status==="Pending").length;
  document.getElementById("d-routes").textContent=routes.length;
  document.getElementById("d-routes-sub").textContent=activeR+" active";
  document.getElementById("d-bookings").textContent=bookings.length;
  document.getElementById("d-bookings-sub").textContent=confirmedB+" confirmed";
  document.getElementById("d-revenue").textContent="₱"+revenue.toLocaleString();
  document.getElementById("d-pending").textContent=pending;
  updateHeaderStats();
  document.getElementById("welcome-banner-wrap").innerHTML=`<div class="welcome-banner"><div class="wb-icon">👋</div><div class="wb-text"><h3>Welcome, ${escH(currentUser.fname)}!</h3><p>📍 ${escH(currentUser.municipality)} · ${currentUser.role==="admin"?"Admin":"Passenger"}</p></div></div>`;
  const types={};routes.forEach(r=>types[r.type]=(types[r.type]||0)+1);
  document.getElementById("fleet-chart").innerHTML=Object.entries(types).map(([t,c])=>`<div class="prog-row"><div class="prog-label">${t}</div><div class="prog-bar"><div class="prog-fill" style="width:${Math.round(c/routes.length*100)}%"></div></div><div class="prog-count">${c}</div></div>`).join("")||"<p style='color:var(--muted);font-size:12px'>No routes yet.</p>";
  const allStops=[...new Set(routes.flatMap(r=>r.stops))];
  const towns=[...new Set(allStops.map(s=>s.split(" ")[0]))].slice(0,20);
  document.getElementById("coverage-areas").innerHTML=towns.map(t=>`<span class="stop-chip">${escH(t)}</span>`).join("");
}

// ── MUNICIPALITIES ──
function setMuniFilter(f,el){muniFilter=f;document.querySelectorAll("#view-municipalities .pill").forEach(p=>p.classList.remove("active"));el.classList.add("active");renderMunicipalities();}
function renderMunicipalities(){
  const q=(document.getElementById("muni-search")?.value||"").toLowerCase();
  const filtered=MUNIS_UNIQUE.filter(m=>{
    const mq=m.name.toLowerCase().includes(q)||m.district.toLowerCase().includes(q);
    const mt=muniFilter==="all"||m.type===muniFilter;
    return mq&&mt;
  });
  const el=document.getElementById("muni-count-badge");if(el)el.textContent=filtered.length;
  const g=document.getElementById("muni-grid");if(!g)return;
  g.innerHTML=filtered.map(m=>`<div class="muni-card" style="border-left:3px solid ${m.type==="City"?"#0d2b4e":"#1a4a7a"}">
    <div class="muni-name">${m.icon} ${escH(m.name)}</div>
    <div class="muni-type-row"><span class="badge ${m.type==="City"?"bg-blue":"bg-gray"}" style="font-size:9px;padding:1px 7px">${m.type}</span><span style="font-size:10px;color:var(--muted)">${m.district} Dist.</span></div>
    <div class="muni-pop">Pop. ~${m.population.toLocaleString()}</div></div>`).join("");
}

// ── TRIP PLANNER ──
function allStopNames(){return[...new Set(routes.flatMap(r=>r.stops))].sort();}
function acSuggest(inputId,listId){
  const q=document.getElementById(inputId).value.trim().toLowerCase();
  const list=document.getElementById(listId);
  if(!q||q.length<2){list.style.display="none";return;}
  const all=[...new Set([...MUNIS_UNIQUE.map(m=>m.name),...allStopNames()])];
  const matches=all.filter(s=>s.toLowerCase().includes(q)).slice(0,7);
  if(!matches.length){list.style.display="none";return;}
  list.innerHTML=matches.map(s=>`<div class="ac-item" onmousedown="pickAc('${inputId}','${listId}','${s.replace(/'/g,"\\'")}')">📍 ${escH(s)}</div>`).join("");
  list.style.display="";
}
function pickAc(inputId,listId,val){document.getElementById(inputId).value=val;document.getElementById(listId).style.display="none";}
function bookingAcSuggest(inputId,listId){
  const q=document.getElementById(inputId).value.trim().toLowerCase();
  const list=document.getElementById(listId);
  if(!q||q.length<2){list.style.display="none";return;}
  const all=[...new Set([...MUNIS_UNIQUE.map(m=>m.name),...allStopNames()])];
  const matches=all.filter(s=>s.toLowerCase().includes(q)).slice(0,6);
  if(!matches.length){list.style.display="none";return;}
  list.innerHTML=matches.map(s=>`<div class="ac-item" onmousedown="pickAc('${inputId}','${listId}','${s.replace(/'/g,"\\'")}')">📍 ${escH(s)}</div>`).join("");
  list.style.display="";
}
function swapLocations(){const f=document.getElementById("trip-from"),t=document.getElementById("trip-to");[f.value,t.value]=[t.value,f.value];}
function searchTrip(){
  ["ac-from","ac-to"].forEach(id=>document.getElementById(id).style.display="none");
  const fromRaw=document.getElementById("trip-from").value.trim().toLowerCase();
  const toRaw=document.getElementById("trip-to").value.trim().toLowerCase();
  const resultsEl=document.getElementById("trip-results");
  if(!fromRaw&&!toRaw){resultsEl.innerHTML=`<div class="no-results"><div class="nr-icon">📍</div><p>Enter your location and destination to find routes.</p></div>`;return;}
  const typeIcons={Bus:"🚌",Jeepney:"🚐","UV Express":"🚖",Tricycle:"🛺","FX / AUV":"🚗","E-Jeep":"⚡"};
  const typeBg={Bus:"#0d2b4e",Jeepney:"#065f46","UV Express":"#7c3aed",Tricycle:"#b45309","FX / AUV":"#0e7490","E-Jeep":"#065f46"};
  const matched=[];
  routes.filter(r=>r.status==="Active").forEach(r=>{
    const stops=r.stops;let fromIdx=-1,toIdx=-1;
    if(fromRaw)fromIdx=stops.findIndex(s=>s.toLowerCase().includes(fromRaw));
    if(toRaw){const sf=fromIdx>=0?fromIdx+1:0;for(let i=sf;i<stops.length;i++){if(stops[i].toLowerCase().includes(toRaw)){toIdx=i;break;}}if(toIdx<0&&fromIdx<0)toIdx=stops.findIndex(s=>s.toLowerCase().includes(toRaw));}
    if(fromRaw&&toRaw&&fromIdx>=0&&toIdx>fromIdx)matched.push({route:r,fromIdx,toIdx,fromStop:stops[fromIdx],toStop:stops[toIdx]});
    else if(fromRaw&&!toRaw&&fromIdx>=0)matched.push({route:r,fromIdx,toIdx:stops.length-1,fromStop:stops[fromIdx],toStop:stops[stops.length-1]});
    else if(!fromRaw&&toRaw&&toIdx>=0)matched.push({route:r,fromIdx:0,toIdx,fromStop:stops[0],toStop:stops[toIdx]});
  });
  if(!matched.length){resultsEl.innerHTML=`<div class="no-results"><div class="nr-icon">🔍</div><p>No routes found from <strong>"${escH(fromRaw||"—")}"</strong> to <strong>"${escH(toRaw||"—")}"</strong>.<br><br>Try broader terms or check the Routes tab.</p></div>`;return;}
  resultsEl.innerHTML=`<p style="font-size:11px;color:var(--muted);margin-bottom:10px;font-weight:700">${matched.length} route${matched.length>1?"s":""} found</p>`+
    matched.map(({route:r,fromIdx,toIdx})=>{
      const sIT=r.stops.slice(fromIdx,toIdx+1);
      const stH=sIT.map((s,i)=>{
        const dc=i===0?"origin":i===sIT.length-1?"dest":"stop";
        const num=i===0?"A":i===sIT.length-1?"B":i;
        return `<div class="journey-step"><div class="step-dot ${dc}">${num}</div><div class="step-label"><strong>${escH(s)}</strong><span class="step-tag">${i===0?"Your location":i===sIT.length-1?"Your destination":"Stop"}</span></div></div>`;
      }).join("");
      const td=Math.round(r.duration*(sIT.length-1)/Math.max(r.stops.length-1,1));
      return `<div class="trip-result-card"><div class="trh"><div class="tr-icon" style="background:${typeBg[r.type]||"#0d2b4e"}">${typeIcons[r.type]||"🚌"}</div><div><div class="tr-name">${escH(r.name)}</div><div class="tr-code">${escH(r.code)} · ${escH(r.type)}</div></div><span class="badge bg-green" style="margin-left:auto">Active</span></div><div class="trip-journey">${stH}</div><div class="trip-footer"><span>⏱ ~${td}min</span><span>📍 ${sIT.length} stops</span><span>₱${r.fare}</span><button class="book-this-btn" onclick="bookFromPlanner(${r.id},'${escH(sIT[0]).replace(/'/g,"\\'")}','${escH(sIT[sIT.length-1]).replace(/'/g,"\\'")}')">Book →</button></div></div>`;
    }).join("");
}
function bookFromPlanner(routeId,from,to){switchTab("bookings");setTimeout(()=>openBookingModal(null,routeId,from,to),80);}
document.addEventListener("click",()=>{["ac-from","ac-to","bac-from","bac-to"].forEach(id=>{const el=document.getElementById(id);if(el)el.style.display="none";});});

// ── ROUTES CRUD ──
function renderRoutes(){
  const q=(document.getElementById("route-search")?.value||"").toLowerCase();
  const filtered=routes.filter(r=>r.name.toLowerCase().includes(q)||r.code.toLowerCase().includes(q));
  const tI={Bus:"🚌",Jeepney:"🚐","UV Express":"🚖",Tricycle:"🛺","FX / AUV":"🚗","E-Jeep":"⚡"};
  const tB={Bus:"#0d2b4e",Jeepney:"#065f46","UV Express":"#7c3aed",Tricycle:"#b45309","FX / AUV":"#0e7490","E-Jeep":"#065f46"};
  if(!filtered.length){document.getElementById("routes-list").innerHTML=`<div class="empty"><div class="empty-icon">🗺</div><p>No routes found.</p></div>`;return;}
  document.getElementById("routes-list").innerHTML=filtered.map(r=>`<div class="item-card">
    <div class="iico" style="background:${tB[r.type]||"#0d2b4e"}">${tI[r.type]||"🚌"}</div>
    <div class="ibody">
      <div class="ititle">${escH(r.name)}<span class="badge ${r.status==="Active"?"bg-green":"bg-red"}">${r.status}</span></div>
      <div class="isub">${escH(r.code)} · ${escH(r.type)}</div>
      <div class="imeta"><span>₱${r.fare}</span><span>⏱ ${r.duration}min</span><span>📍 ${r.stops.length} stops</span></div>
      <div class="stops-row">${r.stops.map(s=>`<span class="stop-chip">${escH(s)}</span>`).join("")}</div>
    </div>
    <div class="iact"><button class="btn btn-ghost btn-icon" onclick="openRouteModal(${r.id})">✏️</button><button class="btn btn-ghost btn-icon" onclick="confirmDeleteRoute(${r.id})" style="border-color:#fecaca">🗑</button></div>
  </div>`).join("");
}
function openRouteModal(id=null){
  editingRouteId=id;const r=id?routes.find(x=>x.id===id):null;
  document.getElementById("route-modal-title").textContent=id?"Edit Route":"Add Route";
  document.getElementById("f-code").value=r?.code||"";
  document.getElementById("f-type").value=r?.type||"Jeepney";
  document.getElementById("f-name").value=r?.name||"";
  document.getElementById("f-fare").value=r?.fare||"";
  document.getElementById("f-duration").value=r?.duration||"";
  document.getElementById("f-stops").value=r?.stops?.join(", ")||"";
  document.getElementById("f-status").value=r?.status||"Active";
  ["code","name","fare","duration"].forEach(k=>document.getElementById("e-"+k).textContent="");
  document.getElementById("route-modal").classList.add("open");
}
function saveRoute(){
  const code=document.getElementById("f-code").value.trim(),type=document.getElementById("f-type").value;
  const name=document.getElementById("f-name").value.trim(),fare=Number(document.getElementById("f-fare").value);
  const duration=Number(document.getElementById("f-duration").value);
  const stops=document.getElementById("f-stops").value.split(",").map(s=>s.trim()).filter(Boolean);
  const status=document.getElementById("f-status").value;
  let v=true;const e=(id,m)=>{document.getElementById(id).textContent=m;v=false;};const c=id=>document.getElementById(id).textContent="";
  code?c("e-code"):e("e-code","Required");
  name?c("e-name"):e("e-name","Required");
  fare>0?c("e-fare"):e("e-fare","Enter fare");
  duration>0?c("e-duration"):e("e-duration","Enter duration");
  if(!v)return;
  if(editingRouteId){const idx=routes.findIndex(r=>r.id===editingRouteId);routes[idx]={...routes[idx],code,type,name,fare,duration,stops,status};showToast("✅ Route updated");}
  else{routes.push({id:nextRouteId++,code,type,name,fare,duration,stops,status,createdAt:new Date().toISOString().split("T")[0]});showToast("✅ Route added");}
  closeModal("route-modal");renderRoutes();updateHeaderStats();
}
function confirmDeleteRoute(id){
  const r=routes.find(x=>x.id===id);
  document.getElementById("confirm-title").textContent="Delete Route?";
  document.getElementById("confirm-msg").textContent=`Remove "${r.name}"? Bookings referencing this route will lose their link.`;
  document.getElementById("confirm-ok-btn").onclick=()=>{routes=routes.filter(x=>x.id!==id);showToast("🗑 Route deleted");renderRoutes();updateHeaderStats();closeModal("confirm-modal");};
  document.getElementById("confirm-modal").classList.add("open");
}

// ── BOOKINGS CRUD ──
function setBookingFilter(f,el){bookingFilter=f;document.querySelectorAll("#booking-filters .pill").forEach(p=>p.classList.remove("active"));el.classList.add("active");renderBookings();}
function renderBookings(){
  const q=(document.getElementById("booking-search")?.value||"").toLowerCase();
  const filtered=bookings.filter(b=>(bookingFilter==="All"||b.status===bookingFilter)&&(b.passenger.toLowerCase().includes(q)||b.ref.toLowerCase().includes(q)||b.route.toLowerCase().includes(q)));
  const sB={Confirmed:"bg-green",Pending:"bg-yellow",Cancelled:"bg-red"};
  if(!filtered.length){document.getElementById("bookings-list").innerHTML=`<div class="empty"><div class="empty-icon">🎫</div><p>No bookings found.</p></div>`;return;}
  document.getElementById("bookings-list").innerHTML=filtered.map(b=>`<div class="item-card">
    <div class="iico" style="background:#065f46">🎫</div>
    <div class="ibody">
      <div class="ititle">${escH(b.passenger)}<span class="badge ${sB[b.status]||"bg-gray"}">${b.status}</span></div>
      <div class="isub">${escH(b.ref)}</div>
      <div class="imeta"><span>🗺 ${escH(b.route)}</span></div>
      ${b.from||b.to?`<div class="imeta" style="margin-top:3px">${b.from?`<span>📍 ${escH(b.from)}</span>`:""}${b.to?`<span>🏁 ${escH(b.to)}</span>`:""}</div>`:""}
      <div class="imeta" style="margin-top:3px"><span>📅 ${b.date} ${b.time}</span><span>💺 ${b.seats}</span><span>₱${b.fare.toLocaleString()}</span></div>
    </div>
    <div class="iact"><button class="btn btn-ghost btn-icon" onclick="openBookingModal(${b.id})">✏️</button><button class="btn btn-ghost btn-icon" onclick="confirmDeleteBooking(${b.id})" style="border-color:#fecaca">🗑</button></div>
  </div>`).join("");
}
function openBookingModal(id=null,preRouteId=null,preFrom="",preTo=""){
  editingBookingId=id;const b=id?bookings.find(x=>x.id===id):null;
  document.getElementById("booking-modal-title").textContent=id?"Edit Booking":"New Booking";
  const sel=document.getElementById("b-route");sel.innerHTML=`<option value="">— Choose a route —</option>`;
  routes.filter(r=>r.status==="Active"||(b&&r.id===b.routeId)).forEach(r=>{
    const opt=document.createElement("option");opt.value=r.id;opt.textContent=r.name+" (₱"+r.fare+")";
    if((b&&b.routeId===r.id)||(!b&&preRouteId===r.id))opt.selected=true;
    sel.appendChild(opt);
  });
  document.getElementById("b-passenger").value=b?.passenger||"";
  document.getElementById("b-from").value=b?.from||preFrom;
  document.getElementById("b-to").value=b?.to||preTo;
  document.getElementById("b-date").value=b?.date||"";
  document.getElementById("b-time").value=b?.time||"";
  document.getElementById("b-seats").value=b?.seats||1;
  document.getElementById("b-status").value=b?.status||"Pending";
  ["passenger","route","date","time","seats"].forEach(k=>document.getElementById("be-"+k).textContent="");
  updateFarePreview();
  document.getElementById("booking-modal").classList.add("open");
}
function updateFarePreview(){
  const routeId=Number(document.getElementById("b-route")?.value);
  const seats=Number(document.getElementById("b-seats")?.value)||1;
  const r=routes.find(x=>x.id===routeId);
  const box=document.getElementById("fare-preview-box");
  if(r){box.style.display="";box.innerHTML=`<strong>Total Fare: ₱${(r.fare*seats).toLocaleString()}</strong> · ${r.duration} mins · ${r.stops.length} stops`;}
  else box.style.display="none";
}
function saveBooking(){
  const passenger=document.getElementById("b-passenger").value.trim();
  const routeId=Number(document.getElementById("b-route").value);
  const from=document.getElementById("b-from").value.trim(),to=document.getElementById("b-to").value.trim();
  const date=document.getElementById("b-date").value,time=document.getElementById("b-time").value;
  const seats=Number(document.getElementById("b-seats").value),status=document.getElementById("b-status").value;
  let v=true;const e=(id,m)=>{document.getElementById(id).textContent=m;v=false;};const c=id=>document.getElementById(id).textContent="";
  passenger?c("be-passenger"):e("be-passenger","Name required");
  routeId?c("be-route"):e("be-route","Select a route");
  date?c("be-date"):e("be-date","Date required");
  time?c("be-time"):e("be-time","Time required");
  seats>=1?c("be-seats"):e("be-seats","Min. 1 seat");
  if(!v)return;
  const r=routes.find(x=>x.id===routeId),fare=r?r.fare*seats:0;
  if(editingBookingId){const idx=bookings.findIndex(b=>b.id===editingBookingId);bookings[idx]={...bookings[idx],passenger,routeId,route:r?.name||"",from,to,date,time,seats,fare,status};showToast("✅ Booking updated");}
  else{const ref=`SK-2025-00${nextRefNum++}`;bookings.push({id:nextBookingId++,ref,passenger,routeId,route:r?.name||"",from,to,date,time,seats,fare,status});showToast("✅ Booked · "+ref);}
  closeModal("booking-modal");renderBookings();updateHeaderStats();
}
function confirmDeleteBooking(id){
  const b=bookings.find(x=>x.id===id);
  document.getElementById("confirm-title").textContent="Remove Booking?";
  document.getElementById("confirm-msg").textContent=`Remove ${b.ref} for "${b.passenger}"? This cannot be undone.`;
  document.getElementById("confirm-ok-btn").onclick=()=>{bookings=bookings.filter(x=>x.id!==id);showToast("🗑 Removed");renderBookings();updateHeaderStats();closeModal("confirm-modal");};
  document.getElementById("confirm-modal").classList.add("open");
}

// ── PROFILE ──
function openProfile(){
  if(!currentUser)return;
  const initials=(currentUser.fname[0]+(currentUser.lname||"")[0]||"").toUpperCase();
  document.getElementById("profile-av").textContent=initials;
  document.getElementById("profile-name").textContent=currentUser.fname+" "+(currentUser.lname||"");
  document.getElementById("profile-email").textContent=currentUser.email;
  document.getElementById("profile-muni").textContent="📍 "+currentUser.municipality;
  document.getElementById("ps-bookings").textContent=bookings.length;
  document.getElementById("ps-routes").textContent=routes.length;
  document.getElementById("ps-revenue").textContent="₱"+bookings.filter(b=>b.status==="Confirmed").reduce((s,b)=>s+b.fare,0).toLocaleString();
  document.getElementById("profile-sheet").classList.add("open");
}
function closeProfile(e){if(!e||e.target===document.getElementById("profile-sheet"))document.getElementById("profile-sheet").classList.remove("open");}

// ── UTILITIES ──
function closeModal(id){document.getElementById(id).classList.remove("open");}
function updateHeaderStats(){document.getElementById("hs-routes").textContent=routes.length;document.getElementById("hs-bookings").textContent=bookings.length;}
function showToast(msg){const t=document.createElement("div");t.className="toast";t.textContent=msg;document.getElementById("toasts").appendChild(t);setTimeout(()=>t.remove(),3000);}
function escH(str){return String(str).replace(/&/g,"&").replace(/</g,"<").replace(/>/g,">").replace(/"/g,""");}
document.querySelectorAll(".modal-overlay").forEach(el=>el.addEventListener("click",e=>{if(e.target===el)el.classList.remove("open");}));
document.addEventListener("keydown",e=>{
  if(e.key!=="Enter")return;
  const panel=document.querySelector(".auth-panel.active");if(!panel)return;
  if(panel.id==="panel-login")doLogin();else if(panel.id==="panel-signup")doSignup();
});
function updateClock(){
  const now=new Date();let h=now.getHours(),m=now.getMinutes();
  const ampm=h>=12?"PM":"AM";h=h%12||12;
  document.getElementById("status-time").textContent=h+":"+(m<10?"0"+m:m)+" "+ampm;
}
updateClock();setInterval(updateClock,10000);
</script>
</body>
</html>
