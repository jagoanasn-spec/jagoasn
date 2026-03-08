<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>JagoASN – Mobile Preview</title>
  <link rel="preconnect" href="https://fonts.googleapis.com"/>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=DM+Sans:wght@400;500;600;700&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html, body {
      height: 100%;
      background: #d8e6f5;
      display: flex; align-items: center; justify-content: center;
      font-family: 'DM Sans', sans-serif;
      overflow: hidden;
    }

    body::before {
      content: ''; position: fixed; inset: 0;
      background:
        radial-gradient(ellipse 55% 45% at 20% 40%, rgba(80,160,255,.2) 0%, transparent 60%),
        radial-gradient(ellipse 50% 40% at 80% 65%, rgba(60,190,255,.14) 0%, transparent 55%);
      pointer-events: none;
    }
    body::after {
      content: ''; position: fixed; inset: 0;
      background-image:
        linear-gradient(rgba(140,180,230,.3) 1px, transparent 1px),
        linear-gradient(90deg, rgba(140,180,230,.3) 1px, transparent 1px);
      background-size: 40px 40px;
      pointer-events: none;
    }

    /* PHONE */
    .phone-shell {
      position: relative;
      width: 375px; height: 812px;
      border-radius: 54px;
      background: #f8fbff;
      box-shadow:
        0 0 0 2px rgba(150,195,255,.6),
        0 0 0 6px rgba(200,225,255,.22),
        0 40px 90px rgba(70,120,200,.22),
        inset 0 0 0 1px rgba(255,255,255,.95);
      overflow: hidden;
      flex-shrink: 0; z-index: 1;
    }
    .phone-shell::before {
      content: ''; position: absolute;
      right: -4px; top: 160px;
      width: 4px; height: 68px;
      background: #b8cee8; border-radius: 0 4px 4px 0;
      box-shadow: 0 90px 0 #b8cee8;
    }
    .phone-shell::after {
      content: ''; position: absolute;
      left: -4px; top: 130px;
      width: 4px; height: 44px;
      background: #b8cee8; border-radius: 4px 0 0 4px;
      box-shadow: 0 60px 0 #b8cee8;
    }

    /* STATUS BAR */
    .status-bar {
      position: relative; z-index: 10;
      height: 50px;
      background: rgba(248,252,255,.98);
      border-bottom: 1px solid rgba(150,195,240,.2);
      display: flex; align-items: flex-end; justify-content: space-between;
      padding: 0 28px 10px;
    }
    .status-time {
      font-family: 'Orbitron', sans-serif;
      font-size: .7rem; font-weight: 700;
      color: #0a1830; letter-spacing: .5px;
    }
    .status-icons { display: flex; align-items: center; gap: 5px; }

    /* DYNAMIC ISLAND */
    .dynamic-island {
      position: absolute; top: 12px; left: 50%; transform: translateX(-50%);
      width: 120px; height: 34px;
      background: #07111f; border-radius: 999px; z-index: 20;
      box-shadow: 0 2px 8px rgba(0,0,0,.18);
    }

    /* SCREEN */
    .screen {
      position: absolute;
      top: 50px; left: 0; right: 0; bottom: 0;
      overflow-y: auto; overflow-x: hidden;
      border-radius: 0 0 54px 54px;
      scrollbar-width: none;
    }
    .screen::-webkit-scrollbar { display: none; }

    /* ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
       LINKTREE CONTENT
    ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ */
    .linktree {
      min-height: 100%;
      background: linear-gradient(168deg, #ffffff 0%, #edf4ff 40%, #f6faff 100%);
      position: relative; overflow: hidden;
    }

    /* dot grid */
    .lt-grid {
      position: absolute; inset: 0; pointer-events: none; z-index: 0;
      background-image: radial-gradient(rgba(60,130,220,.16) 1.2px, transparent 1.2px);
      background-size: 22px 22px;
    }

    /* blobs */
    .blob {
      position: absolute; border-radius: 50%;
      pointer-events: none; z-index: 0;
    }
    .blob1 { width:300px; height:300px; top:-80px; left:-80px;
      background: radial-gradient(circle, rgba(80,160,255,.14) 0%, transparent 70%); }
    .blob2 { width:260px; height:260px; top:300px; right:-80px;
      background: radial-gradient(circle, rgba(0,190,255,.1) 0%, transparent 70%); }
    .blob3 { width:220px; height:220px; bottom:80px; left:-40px;
      background: radial-gradient(circle, rgba(100,180,255,.11) 0%, transparent 70%); }

    /* scan lines */
    .scan {
      position: absolute; inset: 0; pointer-events: none; z-index: 0;
      background: repeating-linear-gradient(
        0deg, transparent, transparent 4px,
        rgba(120,180,255,.035) 4px, rgba(120,180,255,.035) 5px
      );
    }

    /* corner brackets */
    .corner {
      position: absolute; width: 20px; height: 20px;
      border-color: rgba(26,106,255,.2); border-style: solid;
      pointer-events: none; z-index: 3;
    }
    .corner.tl { top:14px; left:14px; border-width:2px 0 0 2px; border-radius:3px 0 0 0; }
    .corner.tr { top:14px; right:14px; border-width:2px 2px 0 0; border-radius:0 3px 0 0; }
    .corner.bl { bottom:14px; left:14px; border-width:0 0 2px 2px; border-radius:0 0 0 3px; }
    .corner.br { bottom:14px; right:14px; border-width:0 2px 2px 0; border-radius:0 0 3px 0; }

    /* CONTENT */
    .lt-content {
      position: relative; z-index: 2;
      padding: 36px 18px 52px;
      display: flex; flex-direction: column; align-items: center;
    }

    /* BRAND */
    .lt-brand {
      text-align: center; margin-bottom: 26px;
      opacity: 0; transform: translateY(-14px);
      animation: ltUp .5s .1s ease forwards;
    }

    .lt-pill {
      display: inline-flex; align-items: center; gap: 6px;
      padding: 5px 14px 5px 9px; border-radius: 999px;
      background: linear-gradient(135deg, #1a6aff, #00c6f7);
      box-shadow: 0 4px 14px rgba(26,106,255,.28), inset 0 1px 0 rgba(255,255,255,.3);
      margin-bottom: 13px;
    }
    .lt-pill-dot {
      width: 7px; height: 7px; border-radius: 50%;
      background: #fff; box-shadow: 0 0 6px rgba(255,255,255,.9);
      animation: blink 1.8s ease-in-out infinite;
    }
    .lt-pill span {
      font-family: 'Orbitron', sans-serif;
      font-size: .55rem; font-weight: 700;
      letter-spacing: 2px; text-transform: uppercase; color: #fff;
    }

    .lt-name {
      font-family: 'Orbitron', sans-serif;
      font-size: 2rem; font-weight: 900;
      letter-spacing: -1px; line-height: 1; color: #071428;
    }
    .lt-name-bar {
      display: block; width: 56px; height: 3px;
      margin: 8px auto 0; border-radius: 999px;
      background: linear-gradient(90deg, #1a6aff, #00c6f7);
      box-shadow: 0 0 8px rgba(0,198,247,.5);
    }

    .lt-tagline {
      margin-top: 11px; font-size: .79rem;
      line-height: 1.65; font-weight: 500;
      color: #526890; max-width: 265px;
      margin-left: auto; margin-right: auto;
    }
    .lt-tagline strong { color: #1a6aff; font-weight: 700; }

    /* SECTION LABEL */
    .lt-section {
      width: 100%;
      display: flex; align-items: center; gap: 8px;
      margin-bottom: 11px; opacity: 0;
    }
    .lt-section span {
      font-family: 'Orbitron', sans-serif;
      font-size: .54rem; font-weight: 700;
      letter-spacing: 2.5px; text-transform: uppercase;
      color: #1a6aff; white-space: nowrap;
    }
    .lt-section::before, .lt-section::after {
      content: ''; flex: 1; height: 1px;
      background: linear-gradient(90deg, transparent, rgba(26,106,255,.22), transparent);
    }
    .lt-section:nth-of-type(1) { animation: ltUp .4s .27s ease forwards; }
    .lt-section:nth-of-type(2) { animation: ltUp .4s .50s ease forwards; }

    /* BUTTON GROUP */
    .lt-group {
      width: 100%;
      display: flex; flex-direction: column; gap: 11px;
      margin-bottom: 16px;
    }

    /* BASE BUTTON */
    .lt-btn {
      display: flex; align-items: center; gap: 13px;
      width: 100%; padding: 14px 16px;
      border-radius: 16px;
      text-decoration: none;
      font-family: 'DM Sans', sans-serif;
      font-weight: 700; font-size: .86rem;
      position: relative; overflow: hidden;
      transition: transform .18s ease, box-shadow .18s ease;
      opacity: 0; animation: ltUp .4s ease forwards;
      -webkit-tap-highlight-color: transparent; cursor: pointer;
    }
    .lt-group:first-of-type .lt-btn:nth-child(1) { animation-delay: .34s; }
    .lt-group:first-of-type .lt-btn:nth-child(2) { animation-delay: .44s; }
    .lt-group:last-of-type  .lt-btn:nth-child(1) { animation-delay: .56s; }
    .lt-group:last-of-type  .lt-btn:nth-child(2) { animation-delay: .64s; }
    .lt-group:last-of-type  .lt-btn:nth-child(3) { animation-delay: .72s; }

    .lt-btn:active { transform: scale(.97); }

    /* glass sheen */
    .lt-btn::before {
      content: ''; position: absolute; inset: 0;
      background: linear-gradient(140deg, rgba(255,255,255,.2) 0%, transparent 55%);
      pointer-events: none; z-index: 1; border-radius: inherit;
    }

    /* PRIMARY — blue */
    .lt-primary {
      background: linear-gradient(135deg, #1251c5 0%, #1a6aff 60%, #33aaff 100%);
      border: 1px solid rgba(26,106,255,.5);
      box-shadow: 0 6px 24px rgba(26,106,255,.3), inset 0 1px 0 rgba(255,255,255,.22);
      color: #fff; padding: 17px 18px; font-size: .9rem;
    }
    .lt-primary .lt-sub  { color: rgba(255,255,255,.68); }
    .lt-primary .lt-icon { background: rgba(255,255,255,.18); }

    .lt-primary::after {
      content: ''; position: absolute; top: 0; left: -110%;
      width: 55%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255,255,255,.2), transparent);
      transform: skewX(-18deg);
      animation: shimmer 3.5s ease-in-out infinite;
      pointer-events: none;
    }

    /* CYAN — YouTube */
    .lt-cyan {
      background: linear-gradient(135deg, #0088bb 0%, #00c6f7 65%, #55ddff 100%);
      border: 1px solid rgba(0,198,247,.45);
      box-shadow: 0 6px 24px rgba(0,198,247,.25), inset 0 1px 0 rgba(255,255,255,.22);
      color: #fff; padding: 17px 18px; font-size: .9rem;
    }
    .lt-cyan .lt-sub  { color: rgba(255,255,255,.68); }
    .lt-cyan .lt-icon { background: rgba(255,255,255,.18); }
    .lt-cyan::after {
      content: ''; position: absolute; top: 0; left: -110%;
      width: 55%; height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255,255,255,.2), transparent);
      transform: skewX(-18deg);
      animation: shimmer 3.5s 1.75s ease-in-out infinite;
      pointer-events: none;
    }

    /* GLASS — secondary */
    .lt-glass {
      background: rgba(255,255,255,.9);
      border: 1.5px solid rgba(26,106,255,.2);
      box-shadow: 0 4px 18px rgba(26,106,255,.1), inset 0 1px 0 rgba(255,255,255,.98);
      color: #071428;
      backdrop-filter: blur(16px); -webkit-backdrop-filter: blur(16px);
    }
    .lt-glass .lt-sub   { color: #526890; }
    .lt-glass .lt-icon  { background: rgba(26,106,255,.09); }
    .lt-glass .lt-arrow { color: #1a6aff; }

    /* pulse ring */
    .lt-pulse {
      position: absolute; inset: -1px; border-radius: 16px;
      border: 2px solid rgba(26,106,255,.4);
      animation: pulseRing 2.6s ease-out infinite;
      pointer-events: none; z-index: 0;
    }
    .lt-cyan .lt-pulse { border-color: rgba(0,198,247,.45); }

    /* ICON */
    .lt-icon {
      width: 38px; height: 38px; border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0; position: relative; z-index: 2;
    }
    .lt-icon svg { width: 19px; height: 19px; }

    /* TEXT */
    .lt-text { flex: 1; position: relative; z-index: 2; }
    .lt-label { display: block; line-height: 1.2; }
    .lt-sub { display: block; font-size: .67rem; font-weight: 500; margin-top: 2px; }
    .lt-arrow { flex-shrink: 0; color: rgba(255,255,255,.75); position: relative; z-index: 2; }

    /* DIVIDER */
    .lt-divider {
      width: 100%; height: 1px;
      background: linear-gradient(90deg, transparent, rgba(26,106,255,.16), transparent);
      margin: 6px 0 16px; opacity: 0;
      animation: ltUp .4s .8s ease forwards;
    }

    /* SOCIAL */
    .lt-social {
      display: flex; gap: 10px; justify-content: center;
      width: 100%; opacity: 0;
      animation: ltUp .45s .9s ease forwards;
    }
    .lt-social-btn {
      display: flex; align-items: center; gap: 7px;
      padding: 10px 16px; border-radius: 999px;
      border: 1.5px solid rgba(26,106,255,.18);
      background: rgba(255,255,255,.92);
      backdrop-filter: blur(12px);
      text-decoration: none;
      font-family: 'DM Sans', sans-serif;
      font-size: .72rem; font-weight: 700; color: #1a3060;
      box-shadow: 0 3px 12px rgba(26,106,255,.1);
      transition: all .2s;
      -webkit-tap-highlight-color: transparent;
    }
    .lt-social-btn:active { transform: scale(.96); }

    /* FOOTER */
    .lt-footer {
      margin-top: 26px; text-align: center;
      opacity: 0; animation: ltUp .5s 1s ease forwards;
    }
    .lt-footer-logo {
      font-family: 'Orbitron', sans-serif;
      font-size: .72rem; font-weight: 700;
      letter-spacing: 1px; color: #1a6aff;
    }
    .lt-footer-copy { font-size: .62rem; color: rgba(80,110,160,.45); margin-top: 3px; }

    /* HOME BAR */
    .home-bar {
      position: absolute; bottom: 10px; left: 50%; transform: translateX(-50%);
      width: 120px; height: 4px;
      background: rgba(30,80,180,.16); border-radius: 999px;
      z-index: 30; pointer-events: none;
    }

    /* KEYFRAMES */
    @keyframes ltUp {
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes shimmer {
      0%, 100% { left: -110%; }
      50%       { left: 160%; }
    }
    @keyframes pulseRing {
      0%   { opacity: .55; transform: scale(1); }
      70%  { opacity: 0;   transform: scale(1.03); }
      100% { opacity: 0;   transform: scale(1.03); }
    }
    @keyframes blink {
      0%, 100% { opacity: 1; transform: scale(1); }
      50%       { opacity: .35; transform: scale(.6); }
    }

    /* outer label */
    .preview-label {
      position: absolute;
      bottom: calc(50% - 440px); left: 50%; transform: translateX(-50%);
      font-family: 'Orbitron', sans-serif;
      font-size: .52rem; font-weight: 700;
      letter-spacing: 3px; text-transform: uppercase;
      color: rgba(70,110,170,.25); white-space: nowrap;
    }

    .phone-glow {
      position: absolute;
      width: 416px; height: 860px; border-radius: 60px;
      border: 1px solid rgba(80,160,255,.15);
      box-shadow: 0 0 60px rgba(80,160,255,.08);
      pointer-events: none; z-index: 0;
    }
  </style>
</head>
<body>

<div class="phone-glow"></div>

<div class="phone-shell">
  <div class="dynamic-island"></div>

  <!-- Status Bar -->
  <div class="status-bar">
    <span class="status-time">9:41</span>
    <div class="status-icons">
      <svg width="14" height="14" viewBox="0 0 24 24" fill="#0a1830">
        <rect x="1" y="15" width="3" height="6" rx="1"/>
        <rect x="6" y="11" width="3" height="10" rx="1"/>
        <rect x="11" y="7" width="3" height="14" rx="1"/>
        <rect x="16" y="3" width="3" height="18" rx="1" opacity=".25"/>
      </svg>
      <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#0a1830" stroke-width="2">
        <path d="M5 12.55a11 11 0 0 1 14.08 0" opacity=".25"/>
        <path d="M1.42 9a16 16 0 0 1 21.16 0" opacity=".15"/>
        <path d="M8.53 16.11a6 6 0 0 1 6.95 0"/>
        <circle cx="12" cy="20" r="1" fill="#0a1830" stroke="none"/>
      </svg>
      <svg width="20" height="12" viewBox="0 0 22 12">
        <rect x=".5" y=".5" width="18" height="11" rx="2" fill="none" stroke="#0a1830" stroke-width="1.2"/>
        <rect x="2" y="2" width="14" height="8" rx="1" fill="#0a1830"/>
        <path d="M19.5 4v4" stroke="#0a1830" stroke-width="1.4" stroke-linecap="round"/>
      </svg>
    </div>
  </div>

  <div class="screen">
    <div class="linktree">
      <div class="lt-grid"></div>
      <div class="blob blob1"></div>
      <div class="blob blob2"></div>
      <div class="blob blob3"></div>
      <div class="scan"></div>
      <div class="corner tl"></div>
      <div class="corner tr"></div>
      <div class="corner bl"></div>
      <div class="corner br"></div>

      <div class="lt-content">

        <!-- BRAND -->
        <div class="lt-brand">
          <div class="lt-pill">
            <div class="lt-pill-dot"></div>
            <span>Platform CPNS</span>
          </div>
          <div class="lt-name">JagoASN</div>
          <div class="lt-name-bar"></div>
          <div class="lt-tagline">
            Jagonya belajar CPNS: <strong>TWK, TIU, TKP</strong>,<br>tryout, dan kelas intensif.
          </div>
        </div>

        <!-- SECTION 1 -->
        <div class="lt-section"><span>Platform Utama</span></div>

        <div class="lt-group">

          <a href="#" class="lt-btn lt-primary">
            <div class="lt-pulse"></div>
            <div class="lt-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <circle cx="12" cy="12" r="10"/>
                <line x1="2" y1="12" x2="22" y2="12"/>
                <path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/>
              </svg>
            </div>
            <div class="lt-text">
              <span class="lt-label">Portal Belajar JagoASN</span>
              <span class="lt-sub">Akses materi, latihan soal & fitur lengkap</span>
            </div>
            <svg class="lt-arrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="rgba(255,255,255,.75)" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>

          <a href="#" class="lt-btn lt-cyan">
            <div class="lt-pulse"></div>
            <div class="lt-icon">
              <svg viewBox="0 0 24 24" fill="white">
                <path d="M23.5 6.2a3 3 0 0 0-2.1-2.1C19.5 3.5 12 3.5 12 3.5s-7.5 0-9.4.6A3 3 0 0 0 .5 6.2C0 8.1 0 12 0 12s0 3.9.5 5.8a3 3 0 0 0 2.1 2.1c1.9.6 9.4.6 9.4.6s7.5 0 9.4-.6a3 3 0 0 0 2.1-2.1C24 15.9 24 12 24 12s0-3.9-.5-5.8z" opacity=".85"/>
                <polygon points="9.75,15.5 15.5,12 9.75,8.5"/>
              </svg>
            </div>
            <div class="lt-text">
              <span class="lt-label">Kelas Gratis di YouTube</span>
              <span class="lt-sub">Pembahasan soal & video belajar terlengkap</span>
            </div>
            <svg class="lt-arrow" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="rgba(255,255,255,.75)" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>

        </div>

        <!-- SECTION 2 -->
        <div class="lt-section" style="margin-top:2px"><span>Fitur & Layanan</span></div>

        <div class="lt-group">

          <a href="#" class="lt-btn lt-glass">
            <div class="lt-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M9 11l3 3L22 4"/>
                <path d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"/>
              </svg>
            </div>
            <div class="lt-text">
              <span class="lt-label">Tryout Gratis</span>
              <span class="lt-sub">Simulasi SKD CPNS tanpa biaya</span>
            </div>
            <svg class="lt-arrow" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>

          <a href="#" class="lt-btn lt-glass">
            <div class="lt-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M2 3h6a4 4 0 0 1 4 4v14a3 3 0 0 0-3-3H2z"/>
                <path d="M22 3h-6a4 4 0 0 0-4 4v14a3 3 0 0 1 3-3h7z"/>
              </svg>
            </div>
            <div class="lt-text">
              <span class="lt-label">Daftar Kelas Intensif</span>
              <span class="lt-sub">Bimbel online bersama mentor terbaik</span>
            </div>
            <svg class="lt-arrow" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>

          <a href="#" class="lt-btn lt-glass">
            <div class="lt-icon">
              <svg viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/>
                <circle cx="9" cy="7" r="4"/>
                <path d="M23 21v-2a4 4 0 0 0-3-3.87M16 3.13a4 4 0 0 1 0 7.75"/>
              </svg>
            </div>
            <div class="lt-text">
              <span class="lt-label">Gabung Grup Belajar</span>
              <span class="lt-sub">Komunitas pejuang CPNS yang aktif</span>
            </div>
            <svg class="lt-arrow" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="#1a6aff" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
          </a>

        </div>

        <!-- DIVIDER -->
        <div class="lt-divider"></div>

        <!-- SOCIAL -->
        <div class="lt-social">
          <a href="#" class="lt-social-btn">
            <svg viewBox="0 0 24 24" fill="#25d366" width="15" height="15">
              <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/>
              <path d="M11.98 0C5.37 0 0 5.373 0 11.988c0 2.109.553 4.09 1.524 5.808L.057 24l6.304-1.654a11.95 11.95 0 0 0 5.62 1.406h.005C18.59 23.752 24 18.379 24 11.764 24 5.176 18.59 0 11.98 0zm.004 21.747a9.924 9.924 0 0 1-5.058-1.384l-.362-.215-3.754.984 1.002-3.655-.237-.376A9.917 9.917 0 0 1 2.05 11.988C2.05 6.482 6.48 2.05 11.984 2.05c5.497 0 9.965 4.432 9.965 9.93 0 5.49-4.468 9.767-9.965 9.767z"/>
            </svg>
            WhatsApp Admin
          </a>
          <a href="#" class="lt-social-btn">
            <svg viewBox="0 0 24 24" fill="none" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" width="15" height="15">
              <defs>
                <linearGradient id="ig" x1="0%" y1="100%" x2="100%" y2="0%">
                  <stop offset="0%" stop-color="#f09433"/>
                  <stop offset="50%" stop-color="#dc2743"/>
                  <stop offset="100%" stop-color="#bc1888"/>
                </linearGradient>
              </defs>
              <rect x="2" y="2" width="20" height="20" rx="5" stroke="url(#ig)"/>
              <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z" stroke="url(#ig)"/>
              <line x1="17.5" y1="6.5" x2="17.51" y2="6.5" stroke="url(#ig)"/>
            </svg>
            Instagram
          </a>
        </div>

        <!-- FOOTER -->
        <div class="lt-footer">
          <div class="lt-footer-logo">◈ JagoASN</div>
          <div class="lt-footer-copy">Platform Belajar CPNS Terpercaya · #JagoASN</div>
        </div>

      </div>
    </div>
  </div>

  <div class="home-bar"></div>
</div>

<div class="preview-label">Mobile Preview · JagoASN Linktree</div>

</body>
</html>
