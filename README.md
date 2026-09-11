# 🌙 MoonlitMinds.com

MoonlitMinds.com adalah ruang digital estetik bertema fairyindie untuk pelacakan harian Anda. Layaknya fase bulan yang berganti, platform ini hadir sebagai wadah magis nan tenang untuk mencatat mood, kebiasaan, serta refleksi diri. Mari bertumbuh perlahan dan rayakan setiap progres kecil Anda di bawah pendar lembut cahaya bulan.

## ✨ Fitur Utama

### 📝 Pelacakan Aktivitas Harian
- Catat aktivitas dengan nama, kategori, waktu, dan durasi
- Sistem kategori yang intuitif:
  - 🎯 **Produktivitas** — kerja, belajar, proyek
  - 💚 **Kesehatan** — olahraga, makan, tidur
  - 🎭 **Hiburan** — hobi, bersantai, hiburan
  - ✨ **Lainnya** — apa saja yang penting untuk Anda
## 🚀 Cara Penggunaan

### 1. Buka Website
Buka `MoonlitMinds.com` di browser Anda.

### 2. Catat Aktivitas
- Masukkan nama aktivitas
- Pilih kategori (klik tombol kategori)
- (Opsional) Tambahkan waktu dan durasi
- Klik tombol "Catat Aktivitas"

### 3. Tandai Selesai
Klik centang di samping aktivitas untuk menandai selesai. Ring progress akan otomatis update.

### 4. Lihat Progres
- Ring progress menampilkan persentase selesai hari ini
- Bagian "Tujuh Hari Terakhir" menampilkan aktivitas seminggu
- Streak counter menunjukkan hari beruntun Anda

### 5. Manajemen Data
- Klik "Hapus" untuk menghapus aktivitas (ada tombol urungkan 5 detik)
- Klik "Hapus Semua Data" di footer untuk reset total

## 💡 Tips & Trik

### Gunakan Streak Sebagai Motivator
Konsistensi lebih penting dari jumlah. Usahakan untuk menyelesaikan minimal 1 aktivitas setiap hari untuk membangun streak.

### Kategori sebagai Filter Mental
Pilih kategori yang sesuai untuk membantu Anda mengelompokkan pikiran dan prioritas.

### Kutipan Harian Sebagai Inspirasi
Baca kutipan motivasi — itu dirancang khusus untuk memotivasi perjalanan personal Anda.

### Data Lokal = Privasi Penuh
Tidak ada data yang dikirim ke server manapun. Semua milik Anda, aman di device Anda.
## 🤝 Kontribusi
Ide, saran, atau perbaikan sangat diterima! Silakan buat issue atau diskusi untuk:
- Fitur baru
- Improvement desain
- Bug reports
- Saran kutipan

---

**Dibuat dengan 💙 untuk mereka yang ingin tumbuh perlahan, dengan konsisten, di bawah cahaya bulan.**
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" id="metaTheme" content="#EFE8D8">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
<title>MoonlitMinds — Pelacak Harian di Bawah Cahaya Bulan</title>
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='42' fill='%23B9913F'/%3E%3Ccircle cx='68' cy='44' r='36' fill='%23EFE8D8'/%3E%3C/svg%3E">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Julius+Sans+One&family=Caveat:wght@500;600&family=Spectral:ital,wght@0,400;0,500;1,400&family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Lora:ital,wght@0,400;1,400;1,500&family=Cormorant+Garamond:wght@500;600&display=swap" rel="stylesheet">
<script>try{if(localStorage.getItem('moonlit.theme')==='eclipse')document.documentElement.classList.add('theme-eclipse')}catch(e){}</script>
<script src="https://cdn.tailwindcss.com"></script>
<script>
tailwind.config = {
  theme: { extend: {
    colors: {
      paper:'rgb(var(--paper) / <alpha-value>)', parchment:'rgb(var(--parchment) / <alpha-value>)',
      ink:'rgb(var(--ink) / <alpha-value>)', olive:'rgb(var(--olive) / <alpha-value>)',
      gold:'rgb(var(--gold) / <alpha-value>)', notos:'rgb(var(--notos) / <alpha-value>)',
      eurus:'rgb(var(--eurus) / <alpha-value>)', boreas:'rgb(var(--boreas) / <alpha-value>)',
    },
    fontFamily: { display:['"Julius Sans One"','sans-serif'], script:['Caveat','cursive'], body:['Spectral','Georgia','serif'] },
    boxShadow: { card:'0 1px 2px rgba(0,0,0,.08), 0 18px 36px -24px rgba(0,0,0,.55)' },
  }}
}
</script>
<style>
  :root{
    --paper:239,232,216; --parchment:245,239,223; --ink:43,38,32;
    --olive:95,107,74; --gold:185,145,63; --notos:58,74,102; --eurus:147,49,46; --boreas:38,36,31;
    --spirit:110,90,126;
    --dotdim: rgba(43,38,32,.25); --cellbg: rgba(255,252,243,.55);
    --holbg: rgba(147,49,46,.06); --goldnum:#8A6822;
    --f-body: 'Spectral', Georgia, serif;
    --f-script: 'Caveat', cursive;
    --f-display: 'Julius Sans One', sans-serif;
  }
  .theme-eclipse{
    /* tinta diputihkan: 242,237,224 */
    --paper:20,24,33; --parchment:27,32,44; --ink:242,237,224;
    --olive:169,188,139; --gold:216,181,99; --notos:159,180,220; --eurus:224,124,106; --boreas:207,200,180;
    --spirit:201,184,220;
    --dotdim: rgba(242,237,224,.4); --cellbg: rgba(242,237,224,.10);
    --holbg: rgba(224,124,106,.13); --goldnum:#D8B563;
    --f-body: 'EB Garamond', Georgia, serif;
    --f-script: 'Lora', Georgia, serif;
    --f-display: 'Cormorant Garamond', Georgia, serif;
  }
  body{ font-family:var(--f-body); transition:background-color .5s ease, color .5s ease; }
  .theme-fade *, .theme-fade *::before, .theme-fade *::after{
    transition: background-color .55s ease, color .55s ease, border-color .55s ease,
                fill .55s ease, stroke .55s ease, box-shadow .55s ease,
                font-family .3s ease, letter-spacing .3s ease, font-size .3s ease; }

  .font-body{ font-family:var(--f-body); }
  .font-script{ font-family:var(--f-script); }
  .font-display{ font-family:var(--f-display); }

  #eclipseTex{ display:none; background-repeat:repeat; background-size:560px 560px; }
  .theme-eclipse #eclipseTex{ display:block; }
  .theme-eclipse .paper-noise{ opacity:.05; }
  .theme-eclipse #heroMoon svg{ filter: drop-shadow(0 0 16px rgba(205,80,50,.35)) drop-shadow(0 0 3px rgba(205,80,50,.4)); }

  /* ============================================================
     LUNAR ECLIPSE — SEMUA TULISAN PUTIH-KREM PENUH
     Setiap tingkat opasitas teks dipaksa penuh; hierarki tetap
     dijaga oleh ukuran, kapital, dan aksen emas — bukan warna.
     ============================================================ */
  .theme-eclipse .text-ink\/25,
  .theme-eclipse .text-ink\/30,
  .theme-eclipse .text-ink\/35,
  .theme-eclipse .text-ink\/40,
  .theme-eclipse .text-ink\/45,
  .theme-eclipse .text-ink\/50,
  .theme-eclipse .text-ink\/55,
  .theme-eclipse .text-ink\/60,
  .theme-eclipse .text-ink\/65,
  .theme-eclipse .text-ink\/70,
  .theme-eclipse .text-ink\/75{ color:rgb(var(--ink)); }
  .theme-eclipse .text-eurus\/60{ color:rgb(var(--eurus)); }

  .theme-eclipse .border-ink\/10{ border-color:rgb(var(--ink) / .2); }
  .theme-eclipse .border-ink\/15{ border-color:rgb(var(--ink) / .26); }
  .theme-eclipse .border-ink\/20{ border-color:rgb(var(--ink) / .32); }
  .theme-eclipse .border-ink\/25{ border-color:rgb(var(--ink) / .38); }
  .theme-eclipse .border-ink\/30{ border-color:rgb(var(--ink) / .44); }
  .theme-eclipse .border-ink\/40{ border-color:rgb(var(--ink) / .54); }
  .theme-eclipse .border-ink\/50{ border-color:rgb(var(--ink) / .64); }
  .theme-eclipse .bg-ink\/10{ background-color:rgb(var(--ink) / .12); }
  .theme-eclipse .bg-ink\/15{ background-color:rgb(var(--ink) / .22); }

  .theme-eclipse .lbl{ color:rgb(var(--ink)); }
  .theme-eclipse .inp{ border-bottom-color:rgba(var(--ink),.5); }
  .theme-eclipse .inp::placeholder{ color:rgba(var(--ink),.72); }
  .theme-eclipse .cat-pill{ color:rgb(var(--ink)); border-color:rgba(var(--ink),.38); }
  .theme-eclipse .cal-nav{ color:rgb(var(--ink)); border-color:rgba(var(--ink),.38); }
  .theme-eclipse .add-btn{ color:rgb(var(--ink)); border-color:rgba(var(--ink),.45); }
  .theme-eclipse .cal-cell{ border-color:rgba(var(--ink),.24); }
  .theme-eclipse .cal-cell:hover{ border-color:rgba(var(--ink),.58); }
  .theme-eclipse .cal-cell .num{ color:rgb(var(--ink)); }
  .theme-eclipse .cal-cell.is-today{ background:rgba(216,181,99,.15); }
  .theme-eclipse .mood-btn{ border-color:rgba(var(--ink),.38); }
  .theme-eclipse .mood-btn .ml{ color:rgb(var(--ink)); }
  .theme-eclipse .mood-btn .ms{ color:rgb(var(--ink) / .85); }
  .theme-eclipse .tt-hint{ color:rgb(var(--ink) / .8); }
  .theme-eclipse #undoBtn{ color:#8A5A20; }
  .theme-eclipse #permBtn{ color:#E08A7A !important; }
  .theme-eclipse .font-display{ font-weight:600; letter-spacing:.32em; }

  .paper-noise{ opacity:.07; mix-blend-mode:multiply;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='240' height='240'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='2' stitchTiles='stitch'/%3E%3CfeColorMatrix type='saturate' values='0'/%3E%3C/filter%3E%3Crect width='240' height='240' filter='url(%23n)'/%3E%3C/svg%3E"); }
  ::selection{ background:rgba(185,145,63,.35); }
  :focus-visible{ outline:2px solid rgba(185,145,63,.85); outline-offset:2px; }

  .lbl{ display:block; font-family:var(--f-display); font-size:10px; letter-spacing:.3em;
    text-transform:uppercase; color:rgba(var(--ink),.55); margin-bottom:.45rem; }
  .inp{ width:100%; background:transparent; border:0; border-radius:0;
    border-bottom:1px solid rgba(var(--ink),.3); padding:.45rem .1rem;
    font-family:var(--f-body); font-size:1rem; color:rgb(var(--ink)); transition:border-color .2s; }
  .inp:focus{ outline:none; border-color:rgb(var(--olive)); }
  .inp::placeholder{ color:rgba(var(--ink),.45); font-style:italic; }
  .input-error{ border-color:rgb(var(--eurus)) !important; }

  .cat-pill{ display:inline-flex; align-items:center; gap:.55rem; --c:rgb(var(--boreas));
    border:1px solid rgba(var(--ink),.25); background:transparent; padding:.45rem .85rem;
    font-family:var(--f-display); font-size:.66rem; letter-spacing:.18em; text-transform:uppercase;
    color:rgba(var(--ink),.65); cursor:pointer; transition:all .18s; }
  .cat-pill .dot{ width:.55rem; height:.55rem; border-radius:9999px; background:var(--c); flex:none; }
  .cat-pill:hover{ border-color:var(--c); color:var(--c); }
  .cat-pill[aria-pressed="true"]{ border-color:var(--c); color:var(--c);
    box-shadow:inset 0 0 0 1px var(--c); background:color-mix(in srgb, var(--c) 12%, transparent); }

  .badge{ font-size:10px; letter-spacing:.18em; text-transform:uppercase;
    font-family:var(--f-display); border:1px solid; padding:1px 8px; white-space:nowrap; }

  .theme-toggle{ display:flex; flex-direction:column; align-items:center; gap:.45rem;
    background:transparent; border:0; cursor:pointer; padding:.4rem 1.2rem; font:inherit;
    transition:transform .15s ease; }
  .theme-toggle:hover{ transform:translateY(-2px); }
  .theme-toggle:active{ transform:translateY(0) scale(.96); }
  .theme-toggle svg{ transition:filter .3s ease; }
  .theme-toggle:hover svg{ filter:drop-shadow(0 0 8px rgba(216,181,99,.5)); }
  .tt-label{ font-family:var(--f-display); font-size:10px; letter-spacing:.28em;
    text-transform:uppercase; color:rgb(var(--gold)); }
  .tt-hint{ font-family:var(--f-display); font-size:7px; letter-spacing:.2em;
    text-transform:uppercase; color:rgba(var(--ink),.4); }

  @keyframes itemIn{ from{opacity:0; transform:translateY(-8px);} to{opacity:1; transform:translateY(0);} }
  .item-in,.note-in{ animation:itemIn .35s ease both; }
  @keyframes shake{ 0%,100%{transform:translateX(0);} 25%{transform:translateX(-5px);} 75%{transform:translateX(5px);} }
  .animate-shake{ animation:shake .3s ease 1; }
  @keyframes fadeUp{ from{opacity:0; transform:translateY(8px);} to{opacity:1; transform:translateY(0);} }
  .quote-in{ animation:fadeUp .6s ease both; }

  .act-row{ cursor:pointer; }
  .act-row:active{ background:rgba(var(--ink),.04); }
  .chk{ transition:transform .12s ease, background-color .2s, border-color .2s, color .2s; }
  .chk:active{ transform:scale(.85); }
  @keyframes chkPop{ 0%{transform:scale(.75);} 55%{transform:scale(1.15);} 100%{transform:scale(1);} }
  .chk.pop{ animation:chkPop .3s ease; }

  @media (prefers-reduced-motion: reduce){
    .tw,.spark,.firefly,#shoot{ display:none !important; }
    .item-in,.note-in,.quote-in,.animate-shake,.chk.pop{ animation:none !important; }
    .theme-fade *, body{ transition:none !important; }
    .theme-toggle:hover{ transform:none; }
  }

  .tw{ position:absolute; border-radius:9999px; background:#B9913F;
    animation:tw var(--d,3s) ease-in-out infinite alternate; }
  @keyframes tw{ from{opacity:.12; transform:scale(.75);} to{opacity:.6; transform:scale(1.25);} }
  .spark{ position:absolute; color:#B9913F; animation:sparkle 5s ease-in-out infinite alternate; }
  @keyframes sparkle{ from{opacity:.1; transform:scale(.7) rotate(-8deg);} to{opacity:.45; transform:scale(1.05) rotate(14deg);} }
  .firefly{ position:absolute; width:5px; height:5px; border-radius:9999px; background:#D8B563;
    opacity:0; filter:blur(.4px); animation:drift var(--d,9s) ease-in-out var(--dl,0s) infinite; }
  @keyframes drift{
    0%{ transform:translate(0,0); opacity:0; }
    18%{ opacity:.75; }
    55%{ transform:translate(12px,-30px); opacity:.3; }
    70%{ opacity:.6; }
    100%{ transform:translate(-8px,-62px); opacity:0; } }
  #shoot{ position:absolute; height:1px; width:72px;
    background:linear-gradient(90deg, transparent, rgba(185,145,63,.9)); opacity:0; pointer-events:none; }
  #shoot.shooting{ animation:shoot 1.5s ease-out forwards; }
  @keyframes shoot{
    0%{ opacity:0; transform:translate(0,0) rotate(-33deg); }
    10%{ opacity:.9; }
    100%{ opacity:0; transform:translate(150px,97px) rotate(-33deg); } }

  #heroMoon{ cursor:pointer; transition:transform .2s; }
  #heroMoon:active{ transform:scale(.97); }

  .cal-cell{ position:relative; display:flex; flex-direction:column; align-items:center; gap:3px;
    padding:6px 0 5px; border:1px solid rgba(var(--ink),.12); background:var(--cellbg);
    transition:border-color .15s; appearance:none; font:inherit; cursor:pointer; }
  .cal-cell:hover{ border-color:rgba(var(--ink),.35); }
  .cal-cell .num{ font-family:var(--f-display); font-size:10px; line-height:1; color:rgba(var(--ink),.7); }
  .cal-cell.is-today{ border-color:rgb(var(--gold)); background:rgba(185,145,63,.1);
    box-shadow:inset 0 0 0 1px rgba(185,145,63,.55); }
  .cal-cell.is-today .num{ color:var(--goldnum); }
  .cal-cell.is-sun .num{ color:rgba(var(--eurus),.85); }
  .cal-cell.is-holiday{ background:var(--holbg); }
  .cal-cell.is-holiday .num{ color:rgb(var(--eurus)); }
  .cal-cell .dots{ display:flex; align-items:center; gap:2px; height:5px; }
  .hd{ width:4px; height:4px; border-radius:9999px; flex:none; }
  .dot-gold{ background:rgb(var(--gold)); } .dot-hol{ background:rgb(var(--eurus)); }
  .dot-dim{ background:var(--dotdim); }
  .ag-pin{ position:absolute; top:1px; right:4px; font-size:8px; line-height:1; color:rgb(var(--gold)); }
  .cal-nav{ display:inline-flex; align-items:center; justify-content:center;
    width:2rem; height:2rem; border:1px solid rgba(var(--ink),.25); background:transparent;
    color:rgba(var(--ink),.6); transition:all .15s; font-size:1.05rem; line-height:1; }
  .cal-nav:hover{ border-color:rgb(var(--gold)); color:rgb(var(--gold)); }

  .add-btn{ flex:none; border:1px solid rgba(var(--ink),.3); padding:.5rem .85rem;
    font-family:var(--f-display); font-size:10px; letter-spacing:.15em;
    text-transform:uppercase; color:rgba(var(--ink),.7); background:transparent; transition:all .15s; }
  .add-btn:hover{ background:rgb(var(--olive)); border-color:rgb(var(--olive)); color:rgb(var(--paper)); }

  #agendaModal{ visibility:hidden; pointer-events:none; }
  #agendaModal.open{ visibility:visible; pointer-events:auto; }
  #agendaModal .modal-backdrop{ opacity:0; transition:opacity .2s ease; }
  #agendaModal.open .modal-backdrop{ opacity:1; }
  #agendaModal .modal-panel{ opacity:0; transform:translateY(12px); transition:opacity .2s ease, transform .2s ease; }
  #agendaModal.open .modal-panel{ opacity:1; transform:none; }
  #agendaModal .inp{ font-size:1.05rem; border-bottom-width:2px; }
  #agendaList{ max-height:11rem; overflow-y:auto; }
  #agendaList li{ display:flex; align-items:flex-start; gap:.65rem;
    border:1px solid rgba(var(--ink),.16); background:rgba(var(--ink),.04); padding:.6rem .8rem; }
  #agendaList li > p{ color:rgb(var(--ink)); font-size:1.02rem; line-height:1.45; }
  #agendaList li .del{ color:rgba(var(--ink),.45); transition:color .15s; }
  #agendaList li .del:hover{ color:rgb(var(--eurus)); }
  #agendaList li.empty-row{ display:block; border-style:dashed; background:transparent;
    font-family:var(--f-script); font-size:1.15rem; color:rgba(var(--ink),.6); }
  .theme-eclipse #agendaList li{ border-color:rgba(var(--ink),.34); background:rgba(var(--ink),.08); }
  .theme-eclipse #agendaList li.empty-row{ background:transparent; color:rgb(var(--ink)); }
  .theme-eclipse #agendaList li .del{ color:rgba(var(--ink),.7); }
  #agDiary .d-row{ display:flex; align-items:flex-start; gap:.55rem; font-size:.92rem; line-height:1.45; }
  #agDiary .d-note{ font-family:var(--f-script); font-size:1.05rem; line-height:1.4; }

  .mood-btn{ display:flex; flex-direction:column; align-items:center; gap:.3rem; --c:rgb(var(--boreas));
    width:5.6rem; border:1px solid rgba(var(--ink),.25); background:transparent;
    padding:.6rem .4rem .5rem; cursor:pointer; transition:all .18s; font:inherit; }
  .mood-btn:hover{ border-color:var(--c); }
  .mood-btn[aria-pressed="true"]{ border-color:var(--c); box-shadow:inset 0 0 0 1px var(--c);
    background:color-mix(in srgb, var(--c) 10%, transparent); }
  .mood-btn .ml{ font-family:var(--f-display); font-size:9px; letter-spacing:.14em;
    text-transform:uppercase; color:rgba(var(--ink),.7); }
  .mood-btn .ms{ font-family:var(--f-script); font-size:.9rem; line-height:1; color:rgba(var(--ink),.45); }
</style>
</head>
<body class="min-h-screen bg-paper font-body text-ink antialiased">

<svg style="position:absolute;width:0;height:0;overflow:hidden" aria-hidden="true">
  <defs>
    <pattern id="moonShade" width="4" height="4" patternUnits="userSpaceOnUse" patternTransform="rotate(45)">
      <rect width="4" height="4" fill="rgba(43,38,32,.06)"/>
      <line x1="0" y1="0" x2="0" y2="4" stroke="rgba(43,38,32,.22)" stroke-width="1"/>
    </pattern>
    <pattern id="moonShadeE" width="4" height="4" patternUnits="userSpaceOnUse" patternTransform="rotate(45)">
      <rect width="4" height="4" fill="rgba(50,16,12,.45)"/>
      <line x1="0" y1="0" x2="0" y2="4" stroke="rgba(24,8,6,.5)" stroke-width="1"/>
    </pattern>
    <radialGradient id="moonLit" cx="35%" cy="32%" r="85%">
      <stop offset="0%" stop-color="#FDFAF0"/><stop offset="55%" stop-color="#F3EAD1"/><stop offset="100%" stop-color="#E2D3A6"/>
    </radialGradient>
    <radialGradient id="moonLitE" cx="35%" cy="32%" r="85%">
      <stop offset="0%" stop-color="#F2AF83"/><stop offset="45%" stop-color="#C96A48"/><stop offset="100%" stop-color="#7E3526"/>
    </radialGradient>
  </defs>
</svg>

<div id="eclipseTex" class="pointer-events-none fixed inset-0 z-0" aria-hidden="true"></div>
<div id="zodiacLayer" class="pointer-events-none fixed inset-0 z-0 overflow-hidden" aria-hidden="true"></div>
<div id="starfield" class="pointer-events-none fixed inset-0 z-0" aria-hidden="true"></div>
<div class="paper-noise pointer-events-none fixed inset-0 z-30" aria-hidden="true"></div>

<div class="relative z-10 mx-auto w-full max-w-xl px-4 pb-4 sm:max-w-2xl sm:px-6">

  <!-- ================= HEADER ================= -->
  <header id="heroZone" class="relative select-none pt-10 text-center sm:pt-14">
    <div class="pointer-events-none absolute inset-0 overflow-hidden" aria-hidden="true">
      <span class="firefly" style="left:8%;top:34%;--d:9s;--dl:0s"></span>
      <span class="firefly" style="left:88%;top:28%;--d:11s;--dl:2s"></span>
      <span class="firefly" style="left:18%;top:60%;--d:10s;--dl:4s"></span>
      <span class="firefly" style="left:78%;top:58%;--d:8.5s;--dl:1s"></span>
      <span class="firefly" style="left:50%;top:16%;--d:12s;--dl:5s"></span>
      <span class="firefly" style="left:32%;top:12%;--d:9.5s;--dl:3s"></span>
      <span id="shoot"></span>
    </div>

    <p class="pl-[0.55em] font-display text-[10px] uppercase tracking-[0.55em] text-ink/55 sm:text-[11px]">✳ MoonlitMinds ✳</p>
    <p class="pl-[0.4em] mt-2 font-display text-[8px] uppercase tracking-[0.4em] text-ink/40 sm:text-[9px]">pelacak harian di bawah cahaya bulan</p>

    <div class="mt-4 flex justify-center">
      <button id="themeToggle" class="theme-toggle" type="button" title="Sentuh untuk berganti tema">
        <span id="themeMoonIcon" aria-hidden="true"></span>
        <span id="themeName" class="tt-label">Full Moon</span>
        <span class="tt-hint">sentuh untuk berganti</span>
      </button>
    </div>

    <div class="relative mx-auto mt-6 flex items-center justify-center gap-4 sm:gap-8">
      <div>
        <div class="relative h-36 w-36 sm:h-44 sm:w-44">
          <svg viewBox="0 0 160 160" class="h-full w-full -rotate-90" aria-hidden="true">
            <defs><linearGradient id="goldGrad" x1="0" y1="0" x2="1" y2="1">
              <stop offset="0%" stop-color="#D8B563"/><stop offset="100%" stop-color="#A8842F"/>
            </linearGradient></defs>
            <circle cx="80" cy="80" r="70" fill="none" style="stroke:rgba(var(--ink),.12)" stroke-width="2.5"/>
            <circle id="ringProgress" cx="80" cy="80" r="70" fill="none" stroke="url(#goldGrad)" stroke-width="5"
                    stroke-linecap="round" stroke-dasharray="0 439.82"
                    style="transition:stroke-dasharray .7s cubic-bezier(.4,0,.2,1)"/>
            <circle cx="80" cy="80" r="62" fill="none" stroke="#B9913F" stroke-opacity="0.35" stroke-width="1.2" stroke-dasharray="46 344"/>
            <circle cx="80" cy="80" r="76" fill="none" style="stroke:rgba(var(--ink),.16)" stroke-width="1" stroke-dasharray="1.5 6"/>
            <g fill="#B9913F" opacity="0.5">
              <circle cx="14" cy="34" r="2"/><circle cx="146" cy="26" r="1.4"/><circle cx="150" cy="112" r="2.2"/>
              <circle cx="10" cy="120" r="1.3"/><circle cx="132" cy="150" r="1.6"/>
            </g>
          </svg>
          <div class="absolute inset-0 flex flex-col items-center justify-center">
            <span id="ringPct" class="font-display text-2xl sm:text-3xl">0%</span>
            <span id="ringCount" class="pl-[0.35em] mt-1 font-display text-[8px] uppercase tracking-[0.3em] text-ink/55 sm:text-[9px]">0/0 selesai</span>
          </div>
        </div>
        <p class="pl-[0.3em] mt-2 font-display text-[8px] uppercase tracking-[0.3em] text-ink/45">progres hari ini</p>
        <button id="shareBtn" type="button"
                class="pl-[0.25em] mt-1 font-display text-[8px] uppercase tracking-[0.25em] text-ink/40 transition-colors hover:text-gold">
          ✳ simpan kartu malam ini
        </button>
      </div>

      <div class="hidden flex-col items-center sm:flex" aria-hidden="true">
        <span class="h-9 w-px border-l border-dashed border-ink/30"></span>
        <svg class="my-1 text-gold/70" width="9" height="9" viewBox="0 0 10 10"><path d="M5 0 L6 4 L10 5 L6 6 L5 10 L4 6 L0 5 L4 4 Z" fill="currentColor"/></svg>
        <span class="h-9 w-px border-l border-dashed border-ink/30"></span>
      </div>

      <div>
        <div id="heroMoon" class="h-36 w-36 sm:h-44 sm:w-44" title="sentuh untuk memutar satu siklus bulan" role="button" tabindex="0" aria-label="Putar siklus fase bulan"></div>
        <p id="phaseName" class="pl-[0.3em] mt-2 font-display text-[9px] uppercase tracking-[0.3em] text-gold">…</p>
        <p class="pl-[0.2em] mt-0.5 font-display text-[7px] uppercase tracking-[0.2em] text-ink/35">sentuh bulannya</p>
      </div>
    </div>

    <p id="phaseSay" class="mx-auto mt-4 max-w-sm font-script text-xl leading-snug text-ink/60 sm:text-2xl">…</p>
    <p id="phaseMeta" class="pl-[0.25em] mt-1 font-display text-[8px] uppercase tracking-[0.25em] text-ink/40 sm:text-[9px]">…</p>

    <h1 class="pl-[0.45em] font-display mt-9 text-[2.3rem] tracking-[0.45em] sm:text-5xl">HARIAN</h1>
    <p class="mt-2 font-script text-2xl text-ink/60 sm:text-[1.7rem]"><span id="dateLabel">…</span></p>

    <figure class="mx-auto mt-7 max-w-md">
      <div class="flex items-center justify-center gap-3">
        <span class="h-px w-8 bg-gold/60"></span>
        <figcaption class="pl-[0.35em] font-display text-[9px] uppercase tracking-[0.35em] text-gold">Kata Hari Ini</figcaption>
        <span class="h-px w-8 bg-gold/60"></span>
      </div>
      <blockquote id="quoteOfDay" class="mt-2 font-script text-[1.6rem] leading-snug text-ink/70 sm:text-[1.8rem]">…</blockquote>
      <button id="quoteShuffle" type="button"
              class="pl-[0.3em] mt-2 font-display text-[9px] uppercase tracking-[0.3em] text-ink/35 transition-colors hover:text-gold">
        ✳ kutipan lainnya
      </button>
    </figure>
  </header>

  <!-- ================= KALENDER ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Piringan Bulan</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>

    <div class="mt-5 border border-ink/15 bg-parchment p-4 shadow-card sm:p-6">
      <div class="flex items-center justify-between gap-2">
        <button id="calPrev" class="cal-nav" type="button" aria-label="Bulan sebelumnya">‹</button>
        <div class="text-center">
          <p id="calTitle" class="pl-[0.35em] font-display text-xs uppercase tracking-[0.35em]">…</p>
          <p id="calEpi" class="mt-1 font-script text-lg text-ink/55">…</p>
        </div>
        <button id="calNext" class="cal-nav" type="button" aria-label="Bulan berikutnya">›</button>
      </div>

      <div class="mt-4 grid grid-cols-7 text-center font-display text-[8px] uppercase tracking-[0.18em] text-ink/40">
        <span class="text-eurus/60">Sen</span><span>Sel</span><span>Rab</span><span>Kam</span><span>Jum</span><span>Sab</span><span class="text-eurus/60">Min</span>
      </div>
      <div id="calGrid" class="mt-1 grid grid-cols-7 gap-1"></div>

      <button id="calToday" type="button"
              class="pl-[0.3em] mt-3 hidden w-full border border-ink/20 py-2 font-display text-[9px] uppercase tracking-[0.3em] text-ink/55 transition-colors hover:border-gold hover:text-gold">
        ✳ kembali ke bulan ini
      </button>
      <p class="mt-3 text-center font-script text-base text-ink/40">geser ‹ › untuk menjelajah · sentuh tanggal untuk jadwal & membuka jejak hari itu…</p>

      <div class="mt-4 flex flex-wrap items-center justify-center gap-x-4 gap-y-1.5 border-t border-dashed border-ink/20 pt-3 font-display text-[8px] uppercase tracking-[0.18em] text-ink/45">
        <span class="inline-flex items-center gap-1.5"><span class="hd dot-gold"></span>selesai</span>
        <span class="inline-flex items-center gap-1.5"><span class="hd dot-dim"></span>belum</span>
        <span class="inline-flex items-center gap-1.5"><span class="hd dot-hol"></span>minggu / hari besar</span>
        <span class="inline-flex items-center gap-1.5"><span class="text-gold">✦</span>jadwal penting</span>
        <span class="inline-flex items-center gap-1.5"><span class="hd" style="background:rgb(var(--notos))"></span>mood</span>
      </div>
      <p class="mt-2 text-center font-script text-sm text-ink/35">tanggal hari raya berdasarkan penanggalan hijriah merupakan perkiraan.</p>

      <div class="mt-5 border-t border-dashed border-ink/20 pt-4">
        <p class="lbl text-center">Rekap Bulan Ini</p>
        <div id="monthRecap" class="mt-1"></div>
      </div>

      <div class="mt-5 border-t border-dashed border-ink/20 pt-4">
        <p class="lbl text-center">Fase Berikutnya</p>
        <div id="nextPhases" class="mt-2 grid grid-cols-2 gap-2 sm:grid-cols-4"></div>
      </div>
    </div>
  </section>

  <!-- ================= FORMULIR ================= -->
  <section id="formSection" class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Catat Aktivitas</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>
    <p class="mx-auto mt-3 max-w-md text-center font-script text-lg text-ink/50">
      yang pernah kau catat akan menunggumu setiap hari — tak perlu menulis ulang; cukup centang, ubah, atau lepaskan saat ia tak lagi dirindukan.
    </p>

    <form id="activityForm" novalidate class="mt-4 border border-ink/15 bg-parchment p-5 shadow-card sm:p-7">
      <label class="lbl" for="actName">Nama aktivitas</label>
      <input id="actName" type="text" class="inp" maxlength="80" autocomplete="off" placeholder="mis. Lari pagi keliling komplek">

      <p class="lbl mt-6">Kategori</p>
      <div id="categoryPills" class="mt-1 flex flex-wrap gap-2" role="group" aria-label="Pilih kategori">
        <button type="button" class="cat-pill" data-cat="produktivitas" style="--c:rgb(var(--notos))" aria-pressed="false"><span class="dot"></span>Produktivitas</button>
        <button type="button" class="cat-pill" data-cat="spiritual"     style="--c:rgb(var(--spirit))" aria-pressed="false"><span class="dot"></span>Spiritual</button>
        <button type="button" class="cat-pill" data-cat="kesehatan"     style="--c:rgb(var(--olive))" aria-pressed="false"><span class="dot"></span>Kesehatan</button>
        <button type="button" class="cat-pill" data-cat="hiburan"       style="--c:rgb(var(--eurus))" aria-pressed="false"><span class="dot"></span>Hiburan</button>
        <button type="button" class="cat-pill" data-cat="lainnya"       style="--c:rgb(var(--boreas))" aria-pressed="false"><span class="dot"></span>Lainnya</button>
      </div>

      <div class="mt-6 grid grid-cols-1 gap-6 sm:grid-cols-2">
        <div>
          <label class="lbl" for="actTime">Waktu · opsional</label>
          <input id="actTime" type="time" class="inp">
        </div>
        <div>
          <label class="lbl" for="actDuration">Durasi (menit) · opsional</label>
          <input id="actDuration" type="number" inputmode="numeric" class="inp" min="1" max="1440" placeholder="mis. 30">
        </div>
      </div>

      <button id="submitBtn" type="submit"
              class="pl-[0.3em] mt-8 inline-flex w-full items-center justify-center gap-3 bg-ink py-3.5 font-display text-xs uppercase tracking-[0.3em] text-paper transition-colors hover:bg-olive active:translate-y-px sm:text-sm">
        <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round">
          <line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/>
        </svg>
        Catat Aktivitas
      </button>
      <button id="cancelEdit" type="button" class="mt-2 hidden w-full py-1 font-display text-[9px] uppercase tracking-[0.3em] text-ink/45 transition-colors hover:text-eurus">
        ✳ batal mengubah
      </button>
    </form>
  </section>

  <!-- ================= DAFTAR HARI INI ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Kegiatan Hari Ini</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>
    <p id="countText" aria-live="polite"
       class="pl-[0.3em] mt-3 text-center font-display text-[10px] uppercase tracking-[0.3em] text-ink/45">0 aktivitas</p>

    <p class="mt-2 text-center font-script text-lg text-ink/55">
      sentuh lingkaran — atau di mana saja pada barisnya — untuk menandai selesai ✓
    </p>

    <p id="streakLabel" class="pl-[0.3em] mt-2 hidden text-center font-display text-[10px] uppercase tracking-[0.3em] text-gold">
      ✳ <span id="streakNum">0</span> hari beruntun — kau tetap datang
    </p>

    <ul id="activityList" class="mt-4 space-y-2"></ul>
    <p id="congrats" class="mt-6 hidden text-center font-script text-2xl text-olive"></p>
    <p class="mt-4 text-center font-script text-base text-ink/40">✕ menghapus untuk hari ini · ikon tempat sampah melepasnya selamanya</p>
  </section>

  <!-- ================= RIWAYAT 7 HARI ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Tujuh Hari Terakhir</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>
    <div id="weekStrip" class="mt-6 grid grid-cols-7 gap-1 sm:gap-2"></div>
  </section>

  <!-- ================= GALERI LANGIT ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Galeri Langit</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>
    <p class="mx-auto mt-4 max-w-md text-center font-script text-xl text-ink/55">
      dua penjaga malam — seekor menunggu di bumi, seekor terbang lebih dahulu ke bintang.
    </p>

    <div class="mt-6 grid gap-5 md:grid-cols-2">
      <!-- Laika -->
      <div class="relative overflow-hidden border border-ink/50 bg-[#232733] p-3 shadow-card">
        <div class="border border-dashed border-[rgba(233,228,210,.25)] p-1">
          <svg viewBox="0 0 260 320" class="block h-auto w-full" role="img" aria-label="Rasi Laika, anjing kecil yang menunggu di langit">
            <defs><radialGradient id="gGlow"><stop offset="0%" stop-color="rgba(243,234,209,.32)"/><stop offset="100%" stop-color="rgba(243,234,209,0)"/></radialGradient></defs>
            <g id="laikaSpeck"></g>
            <g opacity=".55">
              <ellipse cx="222" cy="38" rx="20" ry="7" transform="rotate(-25 222 38)" fill="none" stroke="rgba(233,228,210,.5)"/>
              <ellipse cx="222" cy="38" rx="11" ry="3.5" transform="rotate(-25 222 38)" fill="none" stroke="rgba(233,228,210,.4)"/>
              <circle cx="222" cy="38" r="2" fill="rgba(233,228,210,.6)"/>
              <circle cx="244" cy="52" r="1" fill="rgba(233,228,210,.5)"/><circle cx="204" cy="24" r="1.1" fill="rgba(233,228,210,.4)"/>
            </g>
            <text id="laikaDate" x="250" y="80" text-anchor="end" font-size="13" fill="rgba(233,228,210,.55)" style="font-family:'Caveat',cursive">…</text>
            <circle cx="100" cy="52" r="26" fill="url(#gGlow)"/>
            <circle cx="112" cy="120" r="36" fill="url(#gGlow)"/>
            <circle cx="196" cy="118" r="22" fill="url(#gGlow)"/>
            <g stroke="rgba(233,228,210,.55)" stroke-width="1" fill="none" stroke-linecap="round">
              <path d="M118 34 L98 60"/><path d="M98 60 L86 42"/>
              <path d="M118 34 L112 120"/><path d="M112 120 L128 118"/><path d="M128 118 L98 60"/>
              <path d="M128 118 L150 132"/><path d="M150 132 L170 128"/><path d="M170 128 L196 118"/>
              <path d="M150 132 L146 226"/><path d="M112 120 L104 208"/><path d="M104 208 L126 168"/><path d="M126 168 L150 132"/>
            </g>
            <g fill="rgba(233,228,210,.45)">
              <circle cx="110" cy="90" r="1"/><circle cx="116" cy="102" r="1.2"/><circle cx="122" cy="140" r="1"/>
              <circle cx="118" cy="152" r=".9"/><circle cx="134" cy="148" r="1.1"/><circle cx="140" cy="112" r="1"/>
              <circle cx="108" cy="132" r=".9"/><circle cx="112" cy="180" r="1"/><circle cx="130" cy="122" r=".9"/>
              <circle cx="124" cy="158" r="1.1"/><circle cx="106" cy="66" r=".9"/><circle cx="146" cy="180" r="1"/>
            </g>
            <g fill="#E9E4D2">
              <circle cx="118" cy="34" r="2.2"/><circle cx="86" cy="42" r="1.7"/><circle cx="98" cy="60" r="1.7"/>
              <circle cx="128" cy="118" r="1.7"/><circle cx="104" cy="208" r="1.7"/><circle cx="150" cy="132" r="1.7"/>
              <circle cx="170" cy="128" r="1.7"/><circle cx="196" cy="118" r="2"/><circle cx="146" cy="226" r="1.7"/>
              <circle cx="126" cy="168" r="1.7"/>
            </g>
            <path d="M112 110 L114.8 117.2 L122 120 L114.8 122.8 L112 130 L109.2 122.8 L102 120 L109.2 117.2 Z" fill="#F3EAD1"/>
            <circle cx="112" cy="120" r="1.6" fill="#232733"/>
            <g fill="rgba(233,228,210,.72)" font-size="6.8" letter-spacing=".4" style="font-family:'Julius Sans One',sans-serif">
              <text x="126" y="16" text-anchor="middle">1. Pelabuhan Yang Tenang</text>
              <text x="80" y="40" text-anchor="end">2. Moonlight</text>
              <text x="92" y="70" text-anchor="end">3. Rindu Yang Jauh</text>
              <text x="102" y="126" text-anchor="end">4. Untuk Dua</text>
              <text x="96" y="212" text-anchor="end">5. Tahun-Tahun Bersama</text>
              <text x="134" y="108">6. Arunika</text>
              <text x="156" y="142">7. Peluk Yang Merana</text>
              <text x="176" y="118">8. Sisi Yang Hangat</text>
              <text x="254" y="100" text-anchor="end">9. Di Ambang Rangkaian</text>
              <text x="152" y="232">10. Langit Merindu</text>
              <text x="118" y="174" text-anchor="end">11. Laika, Kau Menunggu</text>
            </g>
          </svg>
        </div>
        <p class="mt-2 text-center font-script text-2xl text-[#E9E4D2]/85">Laika, yang Menunggu Purnama</p>
        <p class="pb-1 text-center font-display text-[8px] uppercase tracking-[0.3em] text-[#E9E4D2]/45">rasi anjing kecil penunggu langit</p>
      </div>

      <!-- Félicette -->
      <div class="relative overflow-hidden border border-ink/50 bg-[#232733] p-3 shadow-card">
        <div class="border border-dashed border-[rgba(233,228,210,.25)] p-1">
          <svg viewBox="0 0 260 320" class="block h-auto w-full" role="img" aria-label="Félicette, kucing yang memeluk purnama">
            <defs>
              <radialGradient id="sunG" cx="42%" cy="38%" r="80%">
                <stop offset="0%" stop-color="#FFE9A8"/><stop offset="45%" stop-color="#F0C65E"/><stop offset="100%" stop-color="#C08A2E"/>
              </radialGradient>
              <radialGradient id="gGlow2"><stop offset="0%" stop-color="rgba(240,198,94,.4)"/><stop offset="100%" stop-color="rgba(240,198,94,0)"/></radialGradient>
            </defs>
            <g id="felSpeck"></g>
            <g>
              <circle cx="34" cy="42" r="6" fill="none" stroke="#D8B563" stroke-width="1.5"/>
              <ellipse cx="34" cy="42" rx="11" ry="3.5" transform="rotate(-18 34 42)" fill="none" stroke="#D8B563" stroke-width=".9"/>
              <circle cx="47" cy="33" r="1.5" fill="rgba(233,228,210,.7)"/>
              <ellipse cx="228" cy="36" rx="14" ry="5" transform="rotate(20 228 36)" fill="none" stroke="rgba(233,228,210,.4)"/>
              <ellipse cx="228" cy="36" rx="7" ry="2.4" transform="rotate(20 228 36)" fill="none" stroke="rgba(233,228,210,.3)"/>
            </g>
            <circle cx="34" cy="258" r="5" fill="none" stroke="rgba(233,228,210,.6)"/>
            <circle cx="36" cy="256" r="1" fill="rgba(233,228,210,.6)"/>
            <circle cx="130" cy="196" r="92" fill="url(#gGlow2)"/>
            <g stroke="url(#sunG)" stroke-width="7" stroke-linecap="round">
              <line x1="130" y1="128" x2="130" y2="100"/><line x1="130" y1="264" x2="130" y2="292"/>
              <line x1="62" y1="196" x2="34" y2="196"/><line x1="198" y1="196" x2="226" y2="196"/>
              <line x1="83" y1="149" x2="63" y2="129"/><line x1="177" y1="149" x2="197" y2="129"/>
              <line x1="83" y1="243" x2="63" y2="263"/><line x1="177" y1="243" x2="197" y2="263"/>
            </g>
            <circle cx="130" cy="196" r="56" fill="url(#sunG)" stroke="rgba(43,38,32,.25)"/>
            <g fill="rgba(43,38,32,.12)">
              <circle cx="112" cy="182" r="7"/><circle cx="150" cy="212" r="5"/><circle cx="126" cy="226" r="4"/><circle cx="148" cy="184" r="3"/>
            </g>
            <path d="M74 116 C 112 62, 190 60, 222 112" stroke="#E9E4D2" stroke-width="19" fill="none" stroke-linecap="round"/>
            <path d="M74 116 C 112 62, 190 60, 222 112" stroke="#1B1C27" stroke-width="15" fill="none" stroke-linecap="round"/>
            <path d="M220 108 C 234 134, 224 160, 202 170" stroke="#E9E4D2" stroke-width="13" fill="none" stroke-linecap="round"/>
            <path d="M220 108 C 234 134, 224 160, 202 170" stroke="#1B1C27" stroke-width="9" fill="none" stroke-linecap="round"/>
            <path d="M62 102 L56 82 L76 94 Z" fill="#1B1C27" stroke="#E9E4D2" stroke-width="2.5" stroke-linejoin="round"/>
            <path d="M80 92 L88 74 L95 96 Z" fill="#1B1C27" stroke="#E9E4D2" stroke-width="2.5" stroke-linejoin="round"/>
            <circle cx="74" cy="114" r="16" fill="#1B1C27" stroke="#E9E4D2" stroke-width="2.5"/>
            <path d="M66 112 q5 4 10 0" fill="none" stroke="#E9E4D2" stroke-width="1.5" stroke-linecap="round"/>
            <path d="M70 123 q4 3 8 0" fill="none" stroke="#E9E4D2" stroke-width="1.2" stroke-linecap="round"/>
            <path d="M60 118 L44 114 M60 122 L44 124" stroke="rgba(233,228,210,.8)" stroke-width=".9" stroke-linecap="round"/>
            <circle cx="62" cy="116" r="1.3" fill="#E9E4D2"/>
            <circle cx="206" cy="264" r="24" fill="rgba(233,228,210,.05)" stroke="rgba(233,228,210,.7)"/>
            <path d="M190 254 A 22 22 0 0 1 204 241" fill="none" stroke="rgba(233,228,210,.5)" stroke-linecap="round"/>
            <path d="M206 259 L208.4 265 L214 267.5 L208.4 270 L206 276 L203.6 270 L198 267.5 L203.6 265 Z" fill="#D8B563"/>
            <g fill="rgba(233,228,210,.8)">
              <path d="M150 40 L151.4 45 L156 47 L151.4 49 L150 54 L148.6 49 L144 47 L148.6 45 Z"/>
              <path d="M52 148 L53.2 152 L57 153.5 L53.2 155 L52 159 L50.8 155 L47 153.5 L50.8 152 Z"/>
              <path d="M230 152 L231.2 156 L235 157.5 L231.2 159 L230 163 L228.8 159 L225 157.5 L228.8 156 Z"/>
              <path d="M70 240 L71 243 L74 244 L71 245 L70 248 L69 245 L66 244 L69 243 Z"/>
            </g>
          </svg>
        </div>
        <p class="mt-2 text-center font-script text-2xl text-[#E9E4D2]/85">Félicette, Pemeluk Purnama</p>
        <p class="pb-1 text-center font-display text-[8px] uppercase tracking-[0.3em] text-[#E9E4D2]/45">kucing pertama yang pulang dari bintang</p>
      </div>
    </div>
  </section>

  <!-- ================= SURAT KECIL ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Surat Kecil untuk Hari Ini</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>
    <p class="mx-auto mt-4 max-w-md text-center font-script text-xl leading-snug text-ink/60 sm:text-[1.35rem]">
      evaluasi bukanlah pengadilan. di sini tak ada yang menilai — hanya dirimu yang mengajar dirimu dengan lembut.
    </p>

    <div class="mt-6 grid gap-4 md:grid-cols-2 sm:gap-5">
      <div class="flex flex-col border border-ink/15 bg-parchment p-5 shadow-card">
        <div class="flex items-center justify-between gap-3 border-b border-dashed border-ink/20 pb-3">
          <h3 class="font-display text-[10px] uppercase tracking-[0.3em] text-olive">✦ Yang Disyukuri</h3>
          <button id="sukaPromptBtn" type="button" title="kata pancingan lain" aria-label="Ganti kata pancingan"
                  class="flex-none text-ink/35 transition-colors hover:text-gold">
            <svg viewBox="0 0 24 24" class="h-3.5 w-3.5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M21 12a9 9 0 1 1-3-6.7"/><path d="M21 3v6h-6"/></svg>
          </button>
        </div>
        <p id="sukaPrompt" class="mt-3 min-h-[3.5rem] font-script text-lg leading-snug text-ink/55">…</p>
        <form id="sukaForm" class="mt-2 flex items-end gap-2" novalidate>
          <div class="min-w-0 flex-1">
            <label class="lbl" for="sukaInput">tulis sesuatu</label>
            <input id="sukaInput" type="text" class="inp" maxlength="140" autocomplete="off" placeholder="mis. teh hangat dari ibu…">
          </div>
          <button type="submit" class="add-btn">tambahkan</button>
        </form>
        <ul id="sukaList" class="mt-4 flex-1 space-y-2.5"></ul>
        <p id="sukaCount" class="mt-3 font-display text-[9px] uppercase tracking-[0.25em] text-ink/40"></p>
      </div>

      <div class="flex flex-col border border-ink/15 bg-parchment p-5 shadow-card">
        <div class="flex items-center justify-between gap-3 border-b border-dashed border-ink/20 pb-3">
          <h3 class="font-display text-[10px] uppercase tracking-[0.3em] text-eurus">✦ Yang Terasa Kurang</h3>
          <button id="kurangPromptBtn" type="button" title="kata pancingan lain" aria-label="Ganti kata pancingan"
                  class="flex-none text-ink/35 transition-colors hover:text-eurus">
            <svg viewBox="0 0 24 24" class="h-3.5 w-3.5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M21 12a9 9 0 1 1-3-6.7"/><path d="M21 3v6h-6"/></svg>
          </button>
        </div>
        <p id="kurangPrompt" class="mt-3 min-h-[3.5rem] font-script text-lg leading-snug text-ink/55">…</p>
        <form id="kurangForm" class="mt-2 flex items-end gap-2" novalidate>
          <div class="min-w-0 flex-1">
            <label class="lbl" for="kurangInput">tulis tanpa menghakimi</label>
            <input id="kurangInput" type="text" class="inp" maxlength="140" autocomplete="off" placeholder="mis. lupa minum air…">
          </div>
          <button type="submit" class="add-btn">tambahkan</button>
        </form>
        <ul id="kurangList" class="mt-4 flex-1 space-y-2.5"></ul>
        <p id="kurangCount" class="mt-3 font-display text-[9px] uppercase tracking-[0.25em] text-ink/40"></p>
      </div>
    </div>

    <p class="mx-auto mt-5 max-w-md text-center font-script text-lg text-ink/45">
      yang disyukuri menjaga cahayamu; yang kurang menuntun langkahmu — keduanya sama sayangnya.
    </p>
  </section>

  <!-- ================= MOOD ================= -->
  <section class="mt-12">
    <div class="flex items-center gap-4">
      <span class="h-px flex-1 bg-ink/15"></span>
      <h2 class="pl-[0.4em] font-display text-[11px] uppercase tracking-[0.4em] text-ink/70">Bagaimana Mood Kamu Hari Ini?</h2>
      <span class="h-px flex-1 bg-ink/15"></span>
    </div>

    <div class="mt-5 border border-ink/15 bg-parchment p-5 text-center shadow-card sm:p-7">
      <div class="mx-auto flex h-14 w-14 items-center justify-center" id="moodIcon" aria-hidden="true"></div>
      <p class="pl-[0.3em] mt-2 font-display text-[9px] uppercase tracking-[0.3em] text-ink/45">pilih satu bulan yang paling mirip perasaanmu</p>
      <div id="moodBtns" class="mt-5 flex flex-wrap justify-center gap-2.5 sm:gap-3"></div>
      <p id="moodSay" class="quote-in mx-auto mt-5 max-w-sm font-script text-xl leading-snug text-ink/60 sm:text-[1.35rem]">…</p>
      <p id="moodPicked" class="pl-[0.3em] mt-2 font-display text-[8px] uppercase tracking-[0.25em] text-ink/35">…</p>
      <p class="mt-4 font-script text-base text-ink/40">tak ada jawaban yang salah di sini — yang lesu pun tetap disayang langit.</p>
    </div>
  </section>

  <!-- ================= FOOTER ================= -->
  <footer class="mt-16 border-t border-ink/10 pt-10">
    <div id="footerPhases" class="flex items-center justify-center gap-3 opacity-80 sm:gap-5" aria-hidden="true"></div>

    <div class="mt-8 flex select-none items-center justify-center gap-5" aria-hidden="true">
      <div class="-rotate-6 border border-ink/25 bg-parchment p-1 shadow-sm">
        <div class="border border-dashed border-ink/40 px-4 py-2 text-center">
          <p class="pl-[0.35em] font-display text-[8px] uppercase tracking-[0.35em] text-ink/60">Satu Hari</p>
          <p class="font-script text-xl leading-tight text-ink/70">satu catatan kecil</p>
          <p class="pl-[0.35em] font-display text-[8px] uppercase tracking-[0.35em] text-ink/60">✳ Satu Langkah ✳</p>
        </div>
      </div>
      <svg width="140" height="60" viewBox="0 0 150 60" class="text-ink/40">
        <g fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round">
          <path d="M4 14 q 18 -8 36 0 t 36 0 t 36 0 t 36 0"/>
          <path d="M4 30 q 18 -8 36 0 t 36 0 t 36 0 t 36 0"/>
          <path d="M4 46 q 18 -8 36 0 t 36 0 t 36 0 t 36 0"/>
        </g>
      </svg>
      <svg width="92" height="92" viewBox="0 0 92 92" class="hidden rotate-12 text-ink/45 sm:block">
        <defs><path id="pmCircle" d="M46 46 m -32 0 a 32 32 0 1 1 64 0 a 32 32 0 1 1 -64 0"/></defs>
        <circle cx="46" cy="46" r="38" fill="none" stroke="currentColor" stroke-width="1.5"/>
        <circle cx="46" cy="46" r="24" fill="none" stroke="currentColor" stroke-width="1"/>
        <text font-size="8.5" letter-spacing="2.5" fill="currentColor" style="font-family:'Julius Sans One',sans-serif">
          <textPath href="#pmCircle">MOONLIT • MINDS • LOKAL •</textPath>
        </text>
        <text x="46" y="50" text-anchor="middle" font-size="12" fill="currentColor">✳</text>
      </svg>
    </div>

    <p class="pl-[0.25em] mt-8 text-center font-display text-[10px] uppercase tracking-[0.25em] text-ink/45">
      <button id="exportBtn" class="underline underline-offset-4 transition-colors hover:text-gold">ekspor data</button>
      <span class="text-ink/25"> · </span>
      <button id="importBtn" class="underline underline-offset-4 transition-colors hover:text-gold">pulihkan data</button>
      <span class="text-ink/25"> · </span>
      <button id="clearAll" class="underline underline-offset-4 transition-colors hover:text-eurus">hapus semua data</button>
    </p>
    <p class="mt-2 text-center font-script text-base text-ink/40">peluk datamu sesekali — unduh cadangan kecil ini, siapa tahu perangkatmu lupa mengingat.</p>
    <input id="importFile" type="file" accept=".json,application/json" class="hidden">
  </footer>
</div>

<!-- ================= MODAL JADWAL & BUKU HARIAN ================= -->
<div id="agendaModal" class="fixed inset-0 z-40 flex items-start justify-center overflow-y-auto p-4 sm:items-center" role="dialog" aria-modal="true">
  <div class="modal-backdrop absolute inset-0 bg-black/55" data-close="1"></div>
  <div class="modal-panel relative z-[1] my-auto w-full max-w-sm border-2 border-ink/30 bg-parchment shadow-card">
    <button data-close="1" class="absolute right-3 top-3 z-[2] text-ink/50 transition-colors hover:text-eurus" aria-label="Tutup">
      <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg>
    </button>
    <div class="border-b-2 border-dashed border-ink/25 px-5 pb-3 pt-5 pr-10">
      <p id="agTitle" class="pl-[0.25em] font-display text-xs uppercase tracking-[0.25em]">…</p>
      <p id="agSub" class="mt-1 font-script text-lg leading-snug text-ink/70">…</p>
    </div>

    <div class="px-5 pt-4">
      <form id="agendaForm" class="flex items-end gap-2" novalidate>
        <div class="min-w-0 flex-1">
          <label class="lbl" for="agendaInput">tandai jadwal penting</label>
          <input id="agendaInput" type="text" class="inp" maxlength="120" autocomplete="off" enterkeyhint="done"
                 placeholder="mis. janji dengan tamu, mentor, atau dirimu…">
        </div>
        <button class="add-btn" type="submit">simpan</button>
      </form>
    </div>

    <div class="px-5 pt-4">
      <div id="agDiary"></div>
    </div>

    <div class="px-5 pb-5 pt-4">
      <p class="lbl">daftar jadwal tanggal ini</p>
      <ul id="agendaList" class="space-y-2"></ul>
    </div>
  </div>
</div>

<!-- ================= TOAST ================= -->
<div id="toast" class="pointer-events-none invisible fixed inset-x-0 bottom-6 z-50 flex translate-y-3 justify-center px-4 opacity-0 transition-all duration-300">
  <div class="flex flex-wrap items-center gap-x-4 gap-y-1 border border-ink/25 bg-ink px-5 py-3 text-paper shadow-card">
    <span id="toastMsg" class="pl-[0.25em] font-display text-[10px] uppercase tracking-[0.25em]">dihapus</span>
    <button id="permBtn" class="hidden font-display text-[10px] uppercase tracking-[0.25em] text-[#E08A7A] underline underline-offset-4">hapus permanen</button>
    <button id="undoBtn" class="font-display text-[10px] uppercase tracking-[0.25em] text-gold underline underline-offset-4 transition-colors hover:text-paper">urungkan</button>
  </div>
</div>

<script>
(function () {
'use strict';

/* ---------- Konstanta & util ---------- */
const KEY='harian.v1', NOTE_KEY='moonlit.notes.v1', AGENDA_KEY='moonlit.agenda.v1',
      MOOD_KEY='moonlit.mood.v1', THEME_KEY='moonlit.theme',
      RM_KEY='moonlit.removed.v1', BLK_KEY='moonlit.blocked.v1';
const CATS = {
  produktivitas: { label:'Produktivitas', color:'#3A4A66', colorE:'#9FB4DC' },
  spiritual:     { label:'Spiritual',     color:'#6E5A7E', colorE:'#C9B8DC' },
  kesehatan:     { label:'Kesehatan',     color:'#5F6B4A', colorE:'#A9BC8B' },
  hiburan:       { label:'Hiburan',       color:'#93312E', colorE:'#E08A7A' },
  lainnya:       { label:'Lainnya',       color:'#26241F', colorE:'#CFC8B4' },
};
const CIRC = 2*Math.PI*70;
const DAYS=['Minggu','Senin','Selasa','Rabu','Kamis','Jumat','Sabtu'];
const MONTHS=['Januari','Februari','Maret','April','Mei','Juni','Juli','Agustus','September','Oktober','November','Desember'];
const MON_S=['Jan','Feb','Mar','Apr','Mei','Jun','Jul','Agu','Sep','Okt','Nov','Des'];
const DAY_S=['Min','Sen','Sel','Rab','Kam','Jum','Sab'];
const EPITHETS=['bulan pertama, niat yang baru disemai','pendek, tetapi cukup untuk mulai','musim berganti, begitu pula dirimu','hujan merangkul tanah, kau merangkul dirimu','semua yang tumbuh, tumbuh diam-diam','cahaya terpanjang untuk yang paling lelah','tengah tahun — tetap bertaut','angin berpindah, kau tetap di rumahmu','daun gugur bukan untuk menyerah','gelap yang menyiapkan terang','menjelang akhir, pelan saja','tutup tahun dengan lembut'];

/* ---------- Tema ---------- */
let theme='full';
try{ theme = localStorage.getItem(THEME_KEY)==='eclipse' ? 'eclipse':'full'; }catch{}
const isEcl=()=>theme==='eclipse';
const THEME_LABEL=()=>isEcl()?'Lunar Eclipse':'Full Moon';
const LIT =()=>isEcl()?'moonLitE':'moonLit';
const SHD =()=>isEcl()?'moonShadeE':'moonShade';
const MSTR=()=>isEcl()?'rgba(226,150,120,.85)':'rgba(43,38,32,.6)';
const CRAT=()=>isEcl()?'rgba(80,26,18,.35)':'rgba(43,38,32,.1)';
const EM  =()=>isEcl()?'rgba(224,124,106,.7)':'rgba(147,49,46,.55)';
const GHOST=()=>isEcl()?'rgba(233,228,210,.3)':'rgba(43,38,32,.3)';
const DARKF=()=>isEcl()?'rgba(0,0,0,.16)':'rgba(43,38,32,.045)';
const CCOL=c=>isEcl()?c.colorE:c.color;

/* ---------- Fase bulan ---------- */
const SYNODIC=29.53058867, NEW_MOON_REF=Date.UTC(2000,0,6,18,14);
function moonPhase(date){ const days=(date.getTime()-NEW_MOON_REF)/864e5;
  const age=((days%SYNODIC)+SYNODIC)%SYNODIC; return {age, frac:age/SYNODIC}; }
const illum=f=>(1-Math.cos(2*Math.PI*f))/2;
const seg=f=>Math.min(7,Math.floor(f*8));
const PHASES=[
  {name:'Bulan Mati',say:'langit menyimpan cahayanya — untukmu, nanti.'},
  {name:'Sabit Muda',say:'sedikit cahaya pun tetap cahaya.'},
  {name:'Paruh Pertama',say:'setengah jalan pun patut dirayakan.'},
  {name:'Cembung Membesar',say:'kau hampir penuh — jangan berhenti dulu.'},
  {name:'Bulan Purnama',say:'semua yang kau rawat sedang bersinar penuh.'},
  {name:'Cembung Menyusut',say:'melepas sedikit bukan berarti kehilangan.'},
  {name:'Paruh Akhir',say:'sisa cahaya juga indah.'},
  {name:'Sabit Tua',say:'istirahatlah — bulan pun perlu pulang.'},
];
function moonPathD(frac,r,cx,cy){
  const q=frac<=.5?frac:1-frac, c=Math.cos(2*Math.PI*q), rx=Math.max(.01,Math.abs(c)*r);
  if(Math.abs(c)>.9995) return {d:`M ${cx} ${cy-r} A ${r} ${r} 0 0 1 ${cx} ${cy+r} L ${cx} ${cy-r} Z`, flip:frac>.5};
  return {d:`M ${cx} ${cy-r} A ${r} ${r} 0 0 1 ${cx} ${cy+r} A ${rx} ${r} 0 0 ${c>0?0:1} ${cx} ${cy-r} Z`, flip:frac>.5};
}
const star4=(x,y,r)=>`M ${x} ${y-r} L ${x+r*.28} ${y-r*.28} L ${x+r} ${y} L ${x+r*.28} ${y+r*.28} L ${x} ${y+r} L ${x-r*.28} ${y+r*.28} L ${x-r} ${y} L ${x-r*.28} ${y-r*.28} Z`;

function heroMoonSVG(frac){
  const {d,flip}=moonPathD(frac,40,50,50);
  const craters=illum(frac)>.35
    ? `<g fill="${CRAT()}"><circle cx="42" cy="42" r="5.5"/><circle cx="58" cy="56" r="4"/><circle cx="46" cy="63" r="2.6"/><circle cx="60" cy="36" r="2.2"/></g>`:'';
  return `<svg viewBox="0 0 100 100" class="h-full w-full" aria-hidden="true">
    <circle cx="50" cy="50" r="47" fill="none" stroke="${GHOST()}" stroke-width="1" stroke-dasharray="1.5 5"/>
    <g fill="#B9913F" opacity=".6">
      <path d="${star4(9,16,3)}"/><path d="${star4(90,12,2.2)}"/><path d="${star4(92,84,2.8)}"/><path d="${star4(7,80,2)}"/>
    </g>
    <g ${flip?'transform="translate(100,0) scale(-1,1)"':''}>
      <circle cx="50" cy="50" r="40" fill="${DARKF()}"/>
      <circle cx="50" cy="50" r="40" fill="url(${SHD()})" opacity=".5"/>
      <circle cx="50" cy="50" r="40" fill="none" stroke="${GHOST()}" stroke-width="1" stroke-dasharray="2 4"/>
      <path d="${d}" fill="url(${LIT()})" stroke="${MSTR()}" stroke-width="1.4"/>
      <clipPath id="heroCr"><path d="${d}"/></clipPath>
      <g clip-path="url(#heroCr)">${craters}</g>
    </g>
  </svg>`;
}
function tinyMoon(frac,size){
  const {d,flip}=moonPathD(frac,40,50,50);
  return `<svg viewBox="0 0 100 100" width="${size}" height="${size}" aria-hidden="true" style="display:block">
    <g ${flip?'transform="translate(100,0) scale(-1,1)"':''}>
      <circle cx="50" cy="50" r="38" fill="${DARKF()}"/>
      <circle cx="50" cy="50" r="38" fill="none" stroke="${GHOST()}" stroke-width="2.5" stroke-dasharray="3 5"/>
      <path d="${d}" fill="url(${LIT()})" stroke="${MSTR()}" stroke-width="3"/>
    </g>
  </svg>`;
}
function nextPhaseMs(t){
  const s=new Date(); s.setHours(0,0,0,0);
  const step=SYNODIC*864e5;
  let ms=NEW_MOON_REF+t*step;
  if(ms<s.getTime()) ms+=Math.ceil((s.getTime()-ms)/step)*step;
  return ms;
}

/* ---------- Hari besar ---------- */
const FIXED_HOL={'01-01':'Tahun Baru Masehi','05-01':'Hari Buruh','08-17':'Hari Kemerdekaan','12-25':'Hari Natal'};
const HOL={
  2025:{'01-27':'Isra Mikraj','01-29':'Tahun Baru Imlek','03-29':'Nyepi','03-31':'Idulfitri 1446 H','04-01':'Cuti Bersama Idulfitri','04-02':'Cuti Bersama Idulfitri','05-12':'Waisak','05-29':'Kenaikan Isa Almasih','06-01':'Hari Lahir Pancasila','06-06':'Iduladha 1446 H','06-27':'Tahun Baru Hijriah 1447','09-05':'Maulid Nabi','12-26':'Cuti Bersama Natal'},
  2026:{'01-16':'Isra Mikraj','02-17':'Tahun Baru Imlek','03-19':'Nyepi','03-20':'Idulfitri 1447 H','03-21':'Cuti Bersama Idulfitri','05-14':'Kenaikan Isa Almasih','05-27':'Iduladha 1447 H','05-31':'Waisak','06-01':'Hari Lahir Pancasila','06-16':'Tahun Baru Hijriah 1448','08-25':'Maulid Nabi'},
  2027:{'01-05':'Isra Mikraj','02-06':'Tahun Baru Imlek','03-08':'Nyepi','03-10':'Idulfitri 1448 H','03-11':'Cuti Bersama Idulfitri','05-06':'Kenaikan Isa Almasih','05-17':'Iduladha 1448 H','05-20':'Waisak','06-01':'Hari Lahir Pancasila','06-05':'Tahun Baru Hijriah 1449','08-15':'Maulid Nabi'},
};
function holidayName(y,m,d){
  const k=`${String(m+1).padStart(2,'0')}-${String(d).padStart(2,'0')}`;
  return (HOL[y]&&HOL[y][k])||FIXED_HOL[k]||null;
}

/* ---------- Mood ---------- */
const MOODS={
  ceria:{label:'Ceria',sub:'purnama',color:'#B9913F',colorE:'#D8B563',say:'senang mendengarnya — biarkan cahaya ini menginap lebih lama.'},
  tenang:{label:'Tenang',sub:'sabit',color:'#5F6B4A',colorE:'#A9BC8B',say:'tenang adalah bahagia yang berjalan pelan. dipeluk baik-baik, ya.'},
  biasa:{label:'Biasa Saja',sub:'paruh',color:'#3A4A66',colorE:'#9FB4DC',say:'hari biasa pun sah untuk dirayakan. kau sudah cukup hari ini.'},
  lelah:{label:'Lelah',sub:'berawan',color:'#6B5F4B',colorE:'#C9B48E',say:'terima kasih sudah bertahan. letakkan bebanmu dulu — bulan pun beristirahat.'},
  lesu:{label:'Lesu',sub:'bulan mati',color:'#93312E',colorE:'#E07C6A',say:'boleh hari ini hanya pulang dan tidur. besok kita coba lagi, pelan-pelan.'},
};
function moodFace(k){
  const st=isEcl()?'rgba(242,237,224,.9)':'rgba(43,38,32,.9)';
  const ln=`fill="none" stroke="${st}" stroke-width="1.6" stroke-linecap="round"`;
  const lelahBg=isEcl()?'#7A6248':'#DCCCA2';
  const cloudF=isEcl()?'#4A443A':'#EFE8D8';
  const cloudS=isEcl()?'rgba(242,237,224,.6)':'rgba(43,38,32,.5)';
  if(k==='ceria') return `<svg viewBox="0 0 40 40" class="h-10 w-10"><circle cx="20" cy="20" r="15" fill="url(${LIT()})" stroke="${st}"/><path d="M12.5 16.5 q2.5 3 5 0" ${ln}/><path d="M22.5 16.5 q2.5 3 5 0" ${ln}/><path d="M14 24 q6 5.5 12 0" ${ln}/></svg>`;
  if(k==='tenang') return `<svg viewBox="0 0 40 40" class="h-10 w-10"><circle cx="20" cy="20" r="15" fill="${DARKF()}"/><path d="M20 5 A15 15 0 0 1 20 35 A4.6 15 0 0 0 20 5 Z" fill="url(${LIT()})" stroke="${st}"/><path d="M26.5 13.5 q2 2.2 4 0" ${ln}/><path d="M27 21.5 q2 2 4 0" ${ln}/></svg>`;
  if(k==='biasa') return `<svg viewBox="0 0 40 40" class="h-10 w-10"><circle cx="20" cy="20" r="15" fill="${DARKF()}"/><path d="M20 5 A15 15 0 0 1 20 35 Z" fill="url(${LIT()})" stroke="${st}"/><path d="M24 15.5 q2.5 2.6 5 0" ${ln}/><path d="M23 25 h7" ${ln}/></svg>`;
  if(k==='lelah') return `<svg viewBox="0 0 40 40" class="h-10 w-10"><circle cx="20" cy="20" r="15" fill="${lelahBg}" stroke="${st}"/><path d="M12 17 h6 M22 17 h6" ${ln}/><path d="M14 25 q3 -2.5 6 0 q3 2.5 6 0" ${ln}/><g fill="${cloudF}" stroke="${cloudS}"><ellipse cx="27" cy="29" rx="8.5" ry="5"/><ellipse cx="19" cy="31" rx="6" ry="4"/></g></svg>`;
  return `<svg viewBox="0 0 40 40" class="h-10 w-10"><circle cx="20" cy="20" r="15" fill="${DARKF()}" stroke="${st}"/><path d="M12 15.5 q3 -2.5 6 0" ${ln}/><path d="M22 15.5 q3 -2.5 6 0" ${ln}/><path d="M14 27 q6 -5 12 0" ${ln}/></svg>`;
}

/* ---------- Zodiak ---------- */
const ZODIAC=[
  {n:'Aries',p:[[20,62],[45,52],[68,42],[86,36]],e:[[0,1],[1,2],[2,3]],b:1},
  {n:'Taurus',p:[[28,30],[45,55],[62,48],[86,24],[56,72],[70,90]],e:[[0,1],[1,2],[2,3],[1,4],[4,5]],b:2},
  {n:'Gemini',p:[[30,14],[33,40],[28,64],[30,86],[62,18],[64,44],[58,68],[60,88]],e:[[0,1],[1,2],[2,3],[4,5],[5,6],[6,7],[1,5],[2,6]],b:0},
  {n:'Cancer',p:[[50,12],[48,44],[30,80],[68,76]],e:[[0,1],[1,2],[1,3]],b:1},
  {n:'Leo',p:[[38,16],[45,33],[40,47],[27,57],[62,60],[73,85],[47,90]],e:[[0,1],[1,2],[2,3],[3,4],[4,5],[5,6]],b:3},
  {n:'Virgo',p:[[20,26],[42,38],[58,28],[74,40],[52,66],[47,88]],e:[[0,1],[1,2],[2,3],[1,4],[4,5]],b:5},
  {n:'Libra',p:[[50,18],[30,54],[70,54],[20,86],[80,86]],e:[[0,1],[0,2],[1,2],[1,3],[2,4]],b:0},
  {n:'Scorpio',p:[[76,12],[70,32],[74,52],[60,70],[42,80],[24,88],[88,22],[92,8]],e:[[0,1],[1,2],[2,3],[3,4],[4,5],[0,6],[6,7]],b:1},
  {n:'Sagitarius',p:[[30,42],[55,36],[76,46],[60,62],[34,62],[48,20],[86,32],[18,52]],e:[[0,1],[1,2],[2,3],[3,4],[4,0],[1,5],[2,6],[4,7]],b:2},
  {n:'Capricorn',p:[[16,32],[44,54],[74,26],[88,46]],e:[[0,1],[1,2],[2,3]],b:1},
  {n:'Aquarius',p:[[18,44],[34,34],[50,44],[66,34],[82,44],[26,68],[42,72]],e:[[0,1],[1,2],[2,3],[3,4],[5,6]],b:2},
  {n:'Pisces',p:[[12,40],[24,33],[29,47],[16,53],[72,58],[85,53],[87,68],[74,71],[50,12]],e:[[0,1],[1,2],[2,3],[3,0],[4,5],[5,6],[6,7],[7,4],[1,8],[8,4]],b:8},
];
const ZPOS=[
  {x:4,y:7,s:120,r:-8,m:true},{x:85,y:10,s:130,r:10,m:true},
  {x:10,y:22,s:120,r:0,m:false},{x:87,y:28,s:110,r:-12,m:false},
  {x:3,y:40,s:150,r:6,m:false},{x:85,y:46,s:130,r:-6,m:false},
  {x:12,y:58,s:110,r:0,m:false},{x:86,y:60,s:150,r:4,m:false},
  {x:5,y:73,s:130,r:-6,m:true},{x:88,y:77,s:120,r:8,m:false},
  {x:13,y:85,s:110,r:0,m:false},{x:84,y:89,s:130,r:-10,m:true},
];
function seedZodiac(){
  const lineC=isEcl()?'rgba(216,181,99,.9)':'rgba(185,145,63,.9)';
  const labelC=isEcl()?'rgba(242,237,224,.75)':'rgba(43,38,32,.5)';
  el('zodiacLayer').innerHTML=ZODIAC.map((s,i)=>{
    const pos=ZPOS[i];
    const lines=s.e.map(([a,b])=>`<line x1="${s.p[a][0]}" y1="${s.p[a][1]}" x2="${s.p[b][0]}" y2="${s.p[b][1]}" stroke="${lineC}" stroke-width="1.1"/>`).join('');
    const stars=s.p.map((p,j)=>j===s.b
      ?`<path d="${star4(p[0],p[1],4.5)}" fill="${lineC}"/><circle cx="${p[0]}" cy="${p[1]}" r="1.1" fill="rgba(239,232,216,.9)"/>`
      :`<circle cx="${p[0]}" cy="${p[1]}" r="1.7" fill="${lineC}"/>`).join('');
    return `<div class="absolute ${pos.m?'':'hidden lg:block'}" style="left:${pos.x}%;top:${pos.y}%;width:${pos.s}px;opacity:.85;transform:rotate(${pos.r}deg)">
      <svg viewBox="0 0 100 100" width="${pos.s}" height="${pos.s}" aria-hidden="true">${lines}${stars}
        <text x="50" y="98" text-anchor="middle" font-size="7.5" letter-spacing="2.6" fill="${labelC}" style="font-family:'Julius Sans One',sans-serif">${s.n.toUpperCase()}</text>
      </svg></div>`;
  }).join('');
}

/* ---------- Kutipan dll ---------- */
const QUOTES=['Langit tak pernah terlambat berganti warna — begitu pula kamu.','Satu langkah kecil hari ini lebih berat daripada seribu niat untuk besok.','Akar tumbuh diam-diam di tempat gelap. Begitu pula usahamu.','Musim tidak berlomba; ia datang tepat waktu. Kamu pun boleh begini.','Hujan hari ini adalah air untuk bunga bulan depan.','Yang penting bukan seberapa cepat, melainkan tetap berjalan.','Pohon besar dulunya biji yang tak diperhatikan siapa pun.','Istirahat bukan menyerah — sungai pun berkolam sebelum melanjutkan arus.','Mencoba lagi bukan berarti gagal dua kali; itu tanda kamu belum menyerah.','Matahari tak minta izin untuk terbit. Kamu tak perlu menunggu sempurna.','Kerjakan yang terjangkau hari ini; sisanya, biar angin yang menyambung.','Setiap daun yang gugur adalah keberanian untuk tumbuh lagi.','Kamu tidak harus menyala tiap hari — bara kecil pun tetap hangat.','Jadilah lembut pada dirimu; kamu sedang tumbuh, bukan berpacu.','Awan berlalu, badai berlalu — kamu yang tetap berdiri di sini.','Disiplin adalah memilih yang paling penting, bukan mengurus semuanya.','Hari yang biasa saja pun berarti: kamu hadir, dan itu cukup.','Bintang butuh langit gelap agar terlihat. Masa sulit pun begitu.','Mulailah kecil, mulailah jujur, mulailah hari ini.','Tak semua hari dibuat untuk produktif; sebagian dibuat untuk bernapas.','Burung tak takut cabangnya retak, karena percaya pada sayapnya.','Menulis ulang ceritamu dimulai dari satu kalimat hari ini.','Apa yang kamu rawat hari ini adalah kekuatanmu esok hari.','Pelankan langkah bukan berarti kalah — itu cara menyiasati jalan.','Setiap centang kecil adalah janji yang kamu tepati pada dirimu sendiri.','Angin musim semi selalu datang setelah musim terdingin.','Gagal adalah data, bukan identitas.','Kebaikan kecil yang rutin mengalahkan usaha besar yang sesekali.','Hari ini mungkin berat, tapi kamu lebih kuat daripada kemarin.','Jangan menunggu motivasi; mulailah, dan ia akan menyusul.','Tumbuh tak selalu terlihat — percayalah pada akar.','Waktu terbaik menanam adalah kemarin; waktu berikutnya adalah sekarang.','Setiap pagi adalah halaman kosong — tulis dengan tinta emas.','Yang konsisten mengalahkan yang sempurna.','Ucapkan terima kasih pada dirimu yang kemarin memilih bertahan.','Angin tak bertanya arah; ia bertiup, lalu jalannya menjadi jalan.','Lambat bukan hambatan — itu jeda untuk berakar lebih dalam.','Bandingkan dirimu hari ini dengan dirimu kemarin, bukan dengan orang lain.','Segala yang berat sedang membentuk sayap yang belum kamu lihat.','Selesai lebih baik daripada sempurna.','Hari ini milikmu — isi dengan hal yang membuatmu bertumbuh.','Senja tak pernah menyesal telah bersinar sepanjang hari. Kamu juga tak perlu.','Bulan tak pernah terlambat; ia hanya menunggu giliran bersinar. Kamu juga begitu.','Purnama tak terjadi dalam semalam — begitu pula dirimu.','Bulan mati pun masih disebut bulan. Kamu yang lelah hari ini tetap utuh.','Setiap malam bulan menunjukkan: berubah bentuk bukan berarti hilang.','Langit tak pernah memaksa bulan bersinar setiap malam. Kamu juga tak harus.','Sabit muda di langit adalah janji bahwa cahaya sedang menuju penuh.','Bulan berjalan sendirian melintasi malam — dan tak pernah tersesat.','Yang gelap hanyalah sisi yang belum tiba gilirannya untuk bercahaya.','Bulan yang tergerhana pun tetap terbit lagi — begitu pula kamu.','Malam merah itu sementara; cahaya hanya berhenti sejenak untuk menatapmu.','Roh adalah api yang tak minta disaksikan — ia menyala karena memilih setia.','Doa yang paling jujur kadang hanya napas yang dihitung pelan-pelan.'];
const CONGRATS=['semua selesai — angin hari ini berpihak padamu ✳','tuntas! tarik napas panjang, kamu luar biasa ✳','seluruh centang terkumpul — selamat beristirahat ✳','hari ini ditutup sempurna. terima kasih sudah gigih ✳','tak ada sisa! akar kebiasaanmu tumbuh makin kuat ✳','purnama kecilmu malam ini telah penuh ✳'];
const P_SUKA=['hal-hal kecil yang menyelamatkanmu hari ini — teh yang hangat, pelukan yang tiba tepat waktu, langit yang berbaik.','siapa yang hari ini membuatmu merasa seperti pulang ke rumah?','hal apa yang ingin kau ucapkan terima kasih pada dirimu sendiri?','benda, suara, atau bau apa yang menyentuhmu pelan-pelan tadi siang?','momen kecil apa yang membuatmu bertahan sampai malam ini?'];
const P_KURANG=['tuliskan yang terasa kurang tanpa menghakimi dirimu — besok kita coba lagi, pelan-pelan.','beban apa yang boleh kau letakkan dulu malam ini? tak semua harus kau bawa pulang.','kalimat baik apa yang ingin kau dengar saat hari terasa berat? katakan untuk dirimu.','apa yang membuatmu lelah hari ini — dan bolehkah ia duduk dulu esok?','jika hari ini sebuah surat, apa yang ingin kau perbaiki di paragraf besok?'];

/* ---------- State ---------- */
let activities=[], noteDB={}, agendaDB={}, moodDB={}, rmMap={}, blocked=[];
let selectedCat='produktivitas';
let toastTimer=null, pendingUndo=null, pendingPerm=null;
let currentQuoteIdx=null, calY, calM, agKey=null, piSuka, piKurang;
let cycling=false, editingId=null, wasAllDone=false;

const el=id=>document.getElementById(id);
const esc=s=>String(s).replace(/[&<>"']/g,c=>({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
const pad=n=>String(n).padStart(2,'0');
const todayStr=(d=new Date())=>`${d.getFullYear()}-${pad(d.getMonth()+1)}-${pad(d.getDate())}`;
const uid=()=>Date.now().toString(36)+Math.random().toString(36).slice(2,7);
const dayOfYear=(d=new Date())=>Math.floor((d-new Date(d.getFullYear(),0,0))/86400000);
const orig=a=>a.origin||a.id;

function loadJ(key,fb){ try{ return JSON.parse(localStorage.getItem(key)) ?? fb; }catch{ return fb; } }
function load(){ const a=loadJ(KEY,[]); return Array.isArray(a)?a.filter(x=>x&&x.id&&x.name):[]; }
function save(){ try{ localStorage.setItem(KEY,JSON.stringify(activities)); }catch{} }
function loadNotes(){ const o=loadJ(NOTE_KEY,{}); return (o&&typeof o==='object'&&!Array.isArray(o))?o:{}; }
function saveNotes(){ try{ localStorage.setItem(NOTE_KEY,JSON.stringify(noteDB)); }catch{} }
function loadAgenda(){ const o=loadJ(AGENDA_KEY,{}); return (o&&typeof o==='object'&&!Array.isArray(o))?o:{}; }
function saveAgenda(){ try{ localStorage.setItem(AGENDA_KEY,JSON.stringify(agendaDB)); }catch{} }
function loadMood(){ const o=loadJ(MOOD_KEY,{}); return (o&&typeof o==='object'&&!Array.isArray(o))?o:{}; }
function saveMood(){ try{ localStorage.setItem(MOOD_KEY,JSON.stringify(moodDB)); }catch{} }
function loadRm(){ const o=loadJ(RM_KEY,{}); return (o&&typeof o==='object'&&!Array.isArray(o))?o:{}; }
function saveRm(){ try{ localStorage.setItem(RM_KEY,JSON.stringify(rmMap)); }catch{} }
function loadBlk(){ const a=loadJ(BLK_KEY,[]); return Array.isArray(a)?a:[]; }
function saveBlk(){ try{ localStorage.setItem(BLK_KEY,JSON.stringify(blocked)); }catch{} }
function todayNotes(){
  const k=todayStr();
  const o=noteDB[k]||(noteDB[k]={suka:[],kurang:[]});
  if(!Array.isArray(o.suka)) o.suka=[];
  if(!Array.isArray(o.kurang)) o.kurang=[];
  return o;
}

/* ---------- Kegiatan menetap ---------- */
function ensureAutoCarry(){
  const t=todayStr();
  for(const k of Object.keys(rmMap)) if(k!==t) delete rmMap[k];
  if(!Array.isArray(rmMap[t])) rmMap[t]=[];
  const dates=[...new Set(activities.map(a=>a.date))].filter(d=>d<t).sort();
  if(!dates.length){ saveRm(); return; }
  const src=dates[dates.length-1];
  const names=new Set(todaysList().map(a=>a.name.trim().toLowerCase()));
  let added=false;
  for(const a of activities.filter(x=>x.date===src)){
    const o=orig(a);
    if(blocked.includes(o)||rmMap[t].includes(o)) continue;
    if(names.has(a.name.trim().toLowerCase())) continue;
    activities.unshift({ id:uid(), origin:o, name:a.name, category:a.category,
      time:a.time||'', duration:a.duration??null, done:false, date:t });
    names.add(a.name.trim().toLowerCase()); added=true;
  }
  saveRm();
  if(added) save();
}

/* ---------- Render dasar ---------- */
function renderDate(){
  const d=new Date();
  el('dateLabel').textContent=`${DAYS[d.getDay()]}, ${d.getDate()} ${MONTHS[d.getMonth()]} ${d.getFullYear()}`.toLowerCase();
}
function setFade(id,txt){
  const q=el(id); q.textContent=txt;
  q.classList.remove('quote-in'); void q.offsetWidth; q.classList.add('quote-in');
}
function renderQuote(forceNew=false){
  const total=QUOTES.length;
  if(currentQuoteIdx===null) currentQuoteIdx=dayOfYear()%total;
  else if(forceNew){ let i; do{ i=Math.floor(Math.random()*total); }while(i===currentQuoteIdx); currentQuoteIdx=i; }
  setFade('quoteOfDay','\u201C'+QUOTES[currentQuoteIdx]+'\u201D');
}
function renderPrompts(){ setFade('sukaPrompt',P_SUKA[piSuka]); setFade('kurangPrompt',P_KURANG[piKurang]); }
function renderHeroMoon(fracOverride){
  const {frac,age}=moonPhase(new Date());
  const f=fracOverride!==undefined?fracOverride:frac;
  el('heroMoon').innerHTML=heroMoonSVG(f);
  el('phaseName').textContent=PHASES[seg(f)].name;
  if(fracOverride===undefined){
    el('phaseSay').textContent=PHASES[seg(f)].say;
    const ms=nextPhaseMs(.5);
    const s=new Date(); s.setHours(0,0,0,0);
    const dFull=Math.round((ms-s.getTime())/864e5);
    const words=dFull===0?'purnama malam ini':dFull===1?'purnama besok':`purnama ${dFull} hari lagi`;
    el('phaseMeta').textContent=`usia bulan ${age.toFixed(1).replace('.',',')} hari · ${words}`;
  }
}
function renderLaikaDate(){
  const d=new Date();
  el('laikaDate').textContent=`${d.getDate()} ${MONTHS[d.getMonth()].toLowerCase()} ${d.getFullYear()}`;
}

/* ---------- Progres & daftar ---------- */
function todaysList(){ return activities.filter(a=>a.date===todayStr()); }
function computeStreak(){
  const doneOn=key=>activities.some(a=>a.date===key&&a.done);
  const d=new Date();
  if(!doneOn(todayStr(d))) d.setDate(d.getDate()-1);
  let s=0; while(doneOn(todayStr(d))){ s++; d.setDate(d.getDate()-1); }
  return s;
}
function renderRing(){
  const items=todaysList();
  const done=items.filter(a=>a.done).length;
  const total=items.length;
  const pct=total?Math.round(done/total*100):0;
  el('ringProgress').setAttribute('stroke-dasharray',`${pct/100*CIRC} ${CIRC}`);
  el('ringPct').textContent=pct+'%';
  el('ringCount').textContent=`${done}/${total} selesai`;
  el('countText').textContent=total?`${done} dari ${total} selesai`:'belum ada aktivitas';
  const allDone=total>0&&done===total;
  const c=el('congrats');
  c.classList.toggle('hidden',!allDone);
  if(allDone&&!wasAllDone) c.textContent=CONGRATS[Math.floor(Math.random()*CONGRATS.length)];
  wasAllDone=allDone;
  const s=computeStreak();
  el('streakLabel').classList.toggle('hidden',s<1);
  el('streakNum').textContent=s;
}
function renderList(){
  const items=todaysList();
  const list=el('activityList');
  if(!items.length){
    list.innerHTML=`<li class="border border-dashed border-ink/25 bg-parchment/50 px-6 py-10 text-center">
      <p class="font-script text-2xl text-ink/45">belum ada catatan hari ini…</p>
      <p class="pl-[0.3em] mt-1 font-display text-[9px] uppercase tracking-[0.3em] text-ink/30">halaman menunggu tinta pertamamu</p>
    </li>`;
    return;
  }
  const CHECK=`<svg viewBox="0 0 24 24" width="20" height="20" fill="none" stroke="currentColor" stroke-width="3.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 13l4 4L19 7"/></svg>`;
  list.innerHTML=items.map(a=>{
    const c=CATS[a.category]||CATS.lainnya;
    const col=CCOL(c);
    const meta=[a.time,a.duration?a.duration+' mnt':null].filter(Boolean).join(' · ');
    const chkCls=a.done?'border-olive bg-olive text-paper':'border-ink/50 text-ink/30';
    return `<li data-id="${a.id}" class="act-row item-in flex items-start gap-3 border border-ink/15 bg-parchment px-4 py-4 shadow-card">
      <button type="button" data-action="toggle" aria-pressed="${a.done}"
        aria-label="${a.done?'Tandai belum selesai':'Tandai selesai'}"
        style="width:2.3rem;height:2.3rem;flex:none"
        class="chk mt-0.5 flex items-center justify-center rounded-full border-2 ${chkCls}">
        ${CHECK}
      </button>
      <div class="min-w-0 flex-1">
        <p class="break-words leading-snug ${a.done?'italic text-ink/40 line-through':''}">${esc(a.name)}</p>
        <div class="mt-1.5 flex flex-wrap items-center gap-2">
          <span class="badge inline-flex items-center gap-1.5" style="color:${col}">
            <span class="inline-block h-1.5 w-1.5 rounded-full" style="background:${col}"></span>${c.label}
          </span>
          ${meta?`<span class="font-display text-[9px] uppercase tracking-[0.2em] text-ink/45">${esc(meta)}</span>`:''}
        </div>
      </div>
      <button type="button" data-action="edit" aria-label="Ubah aktivitas" title="ubah"
        style="flex:none" class="mt-1 text-ink/35 transition-colors hover:text-gold">
        <svg viewBox="0 0 24 24" width="18" height="18" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4Z"/></svg>
      </button>
      <button type="button" data-action="delete" aria-label="Hapus aktivitas hari ini" title="hapus hari ini"
        style="flex:none" class="mt-1 text-ink/30 transition-colors hover:text-eurus">
        <svg viewBox="0 0 24 24" width="18" height="18" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg>
      </button>
    </li>`;
  }).join('');
}
function renderWeek(){
  let html=''; const tKey=todayStr();
  for(let i=6;i>=0;i--){
    const d=new Date(); d.setDate(d.getDate()-i);
    const key=todayStr(d);
    const items=activities.filter(a=>a.date===key);
    const done=items.filter(a=>a.done).length;
    const total=items.length;
    const frac=moonPhase(d).frac;
    const isToday=key===tKey;
    html+=`<div class="flex flex-col items-center gap-1.5 border py-2.5 ${isToday?'border-gold/70 bg-[rgba(185,145,63,.07)]':'border-ink/10'}">
      <span class="font-display text-[8px] uppercase tracking-[0.15em] ${isToday?'text-gold':'text-ink/45'}">${DAY_S[d.getDay()]}</span>
      ${tinyMoon(frac,24)}
      <span class="text-[11px] ${total?'text-ink/75':'text-ink/30'}">${done}<span class="text-ink/35">/${total}</span></span>
    </div>`;
  }
  el('weekStrip').innerHTML=html;
}

/* ---------- Kalender ---------- */
function renderCalendar(){
  const first=new Date(calY,calM,1);
  const dim=new Date(calY,calM+1,0).getDate();
  const off=(first.getDay()+6)%7;
  el('calTitle').textContent=`${MONTHS[calM]} ${calY}`;
  el('calEpi').textContent=EPITHETS[calM];
  const tKey=todayStr();
  let html='';
  for(let i=0;i<off;i++) html+='<div></div>';
  for(let day=1;day<=dim;day++){
    const d=new Date(calY,calM,day);
    const key=todayStr(d);
    const {frac}=moonPhase(d);
    const hol=holidayName(calY,calM,day);
    const ags=agendaDB[key]||[];
    const acts=activities.filter(a=>a.date===key);
    const done=acts.filter(a=>a.done).length;
    const mood=moodDB[key];
    const cls=['cal-cell'];
    if(key===tKey) cls.push('is-today');
    if(d.getDay()===0) cls.push('is-sun');
    if(hol) cls.push('is-holiday');
    const tips=[`${day} ${MONTHS[calM]} ${calY}`,PHASES[seg(frac)].name];
    if(hol) tips.push(hol);
    if(ags.length) tips.push('jadwal: '+ags.map(a=>a.text).join('; '));
    if(acts.length) tips.push(`${done}/${acts.length} aktivitas selesai`);
    if(mood) tips.push('mood: '+MOODS[mood].sub);
    let dots='';
    if(hol) dots+='<span class="hd dot-hol"></span>';
    if(acts.length) dots+=`<span class="hd ${done?'dot-gold':'dot-dim'}"></span>`;
    if(mood) dots+=`<span class="hd" style="background:${CCOL(MOODS[mood])}"></span>`;
    html+=`<button type="button" class="${cls.join(' ')}" data-date="${key}" title="${esc(tips.join(' · '))}">
      ${ags.length?'<span class="ag-pin">✦</span>':''}
      ${tinyMoon(frac,20)}<span class="num">${day}</span>
      <span class="dots">${dots}</span>
    </button>`;
  }
  el('calGrid').innerHTML=html;
  const now=new Date();
  el('calToday').classList.toggle('hidden',calY===now.getFullYear()&&calM===now.getMonth());
  renderRecap();
}
function renderRecap(){
  const box=el('monthRecap');
  const dim=new Date(calY,calM+1,0).getDate();
  let tot=0,don=0,daysActive=0;
  const catCount={}, doneByDay={}, moodCount={};
  for(let d=1;d<=dim;d++){
    const key=todayStr(new Date(calY,calM,d));
    const acts=activities.filter(a=>a.date===key);
    const dn=acts.filter(a=>a.done).length;
    tot+=acts.length; don+=dn;
    if(dn){ daysActive++; doneByDay[d]=dn; }
    acts.forEach(a=>{ const c=CATS[a.category]||CATS.lainnya; catCount[c.label]=(catCount[c.label]||0)+1; });
    const m=moodDB[key]; if(m) moodCount[MOODS[m].sub]=(moodCount[MOODS[m].sub]||0)+1;
  }
  if(!tot&&!Object.keys(moodCount).length){
    box.innerHTML='<p class="text-center font-script text-lg text-ink/45">masih halaman kosong untuk bulan ini — setiap centang akan tertulis di sini.</p>';
    return;
  }
  const pct=tot?Math.round(don/tot*100):0;
  const topCat=Object.entries(catCount).sort((a,b)=>b[1]-a[1])[0];
  const topMood=Object.entries(moodCount).sort((a,b)=>b[1]-a[1])[0];
  let best=0,cur=0;
  for(let d=1;d<=dim;d++){ if(doneByDay[d]){ cur++; if(cur>best)best=cur; } else cur=0; }
  box.innerHTML=`
    <p class="text-center font-script text-xl text-ink/70">bulan ini kau menulis ${tot} hal kecil, dan ${don} di antaranya tuntas (${pct}%).</p>
    <div class="mt-2 grid grid-cols-2 gap-x-3 gap-y-1 text-center sm:grid-cols-4">
      <div class="border border-ink/10 py-1.5"><p class="font-display text-sm">${daysActive}</p><p class="font-display text-[7px] uppercase tracking-[0.18em] text-ink/50">hari aktif</p></div>
      <div class="border border-ink/10 py-1.5"><p class="font-display text-sm">${best}</p><p class="font-display text-[7px] uppercase tracking-[0.18em] text-ink/50">run tuntas terbaik</p></div>
      <div class="border border-ink/10 py-1.5"><p class="text-[13px] leading-tight">${topCat?esc(topCat[0]):'—'}</p><p class="font-display text-[7px] uppercase tracking-[0.18em] text-ink/50">paling kau rawat</p></div>
      <div class="border border-ink/10 py-1.5"><p class="text-[13px] leading-tight">${topMood?esc(topMood[0]):'—'}</p><p class="font-display text-[7px] uppercase tracking-[0.18em] text-ink/50">mood sering</p></div>
    </div>
    <p class="mt-2 text-center font-script text-base text-ink/45">${best>=3?'angka kecil yang tumbuh diam-diam — seperti akar.':'satu pun run adalah permulaan yang sah.'}</p>`;
}
function renderNextPhases(){
  const NAMES=['Bulan Mati','Paruh Pertama','Purnama','Paruh Akhir'];
  const s=new Date(); s.setHours(0,0,0,0);
  el('nextPhases').innerHTML=[0,.25,.5,.75].map((t,i)=>{
    const ms=nextPhaseMs(t);
    const d=new Date(ms);
    const diff=Math.round((ms-s.getTime())/864e5);
    const when=diff===0?'malam ini':diff===1?'besok':`${diff} hari lagi`;
    return `<div class="flex flex-col items-center border border-ink/10 bg-paper/60 px-1 py-3">
      ${tinyMoon(t,t===.5?30:24)}
      <p class="mt-1.5 font-display text-[8px] uppercase tracking-[0.18em] text-ink/60">${NAMES[i]}</p>
      <p class="font-script text-lg leading-tight text-ink/75">${d.getDate()} ${MON_S[d.getMonth()]}</p>
      <p class="mt-0.5 font-display text-[8px] uppercase tracking-[0.15em] ${diff===0?'text-olive':'text-gold'}">${when}</p>
    </div>`;
  }).join('');
}
function renderFooterPhases(){
  el('footerPhases').innerHTML=[0,1,2,3,4,5,6,7].map(i=>tinyMoon(i/8,20)).join('');
}

/* ---------- Modal: jadwal + buku harian ---------- */
function renderAgendaList(){
  const arr=agendaDB[agKey]||[];
  const ul=el('agendaList');
  ul.innerHTML=arr.length?arr.map(it=>`
    <li data-id="${it.id}">
      <span class="mt-[9px] h-1.5 w-1.5 flex-none rotate-45" style="background:rgb(var(--gold))"></span>
      <p class="min-w-0 flex-1 break-words">${esc(it.text)}</p>
      <button type="button" data-action="del" aria-label="Hapus jadwal" class="del mt-0.5 flex-none">
        <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg>
      </button>
    </li>`).join('')
    :'<li class="empty-row">belum ada tanda — halaman ini masih lapang untuk rencana kecil…</li>';
}
function renderDiary(key){
  const box=el('agDiary');
  const acts=activities.filter(a=>a.date===key);
  const n=noteDB[key];
  const mood=moodDB[key];
  let html='';
  if(acts.length){
    html+='<p class="lbl">kegiatan hari itu</p><ul class="space-y-1.5">'+acts.map(a=>{
      const c=CATS[a.category]||CATS.lainnya;
      const col=CCOL(c);
      return `<li class="d-row">
        <span class="mt-[3px] flex-none font-display text-[10px]" style="color:${a.done?'rgb(var(--olive))':'rgba(var(--ink),.4)'}">${a.done?'✓':'○'}</span>
        <span class="min-w-0 flex-1 break-words ${a.done?'italic text-ink/50 line-through':''}">${esc(a.name)}</span>
        <span class="badge flex-none" style="color:${col}">${c.label}</span>
      </li>`;
    }).join('')+'</ul>';
  }
  if(mood) html+=`<p class="lbl mt-3">mood</p><p class="d-note">— ${esc(MOODS[mood].sub)} (${esc(MOODS[mood].label.toLowerCase())})</p>`;
  if(n&&Array.isArray(n.suka)&&n.suka.length)
    html+='<p class="lbl mt-3">yang disyukuri</p>'+n.suka.map(x=>`<p class="d-note text-ink/75">✦ ${esc(x.text)}</p>`).join('');
  if(n&&Array.isArray(n.kurang)&&n.kurang.length)
    html+='<p class="lbl mt-3">yang terasa kurang</p>'+n.kurang.map(x=>`<p class="d-note text-ink/75">✧ ${esc(x.text)}</p>`).join('');
  if(!html) html='<p class="font-script text-lg italic text-ink/45">halaman ini masih putih — belum ada jejak di tanggal itu.</p>';
  box.innerHTML=html;
}
function openAgenda(key){
  agKey=key;
  const [y,m,d]=key.split('-').map(Number);
  const dt=new Date(y,m-1,d);
  el('agTitle').textContent=`${DAYS[dt.getDay()]}, ${d} ${MONTHS[m-1]} ${y}`.toLowerCase();
  const {frac}=moonPhase(dt);
  const hol=holidayName(y,m-1,d);
  el('agSub').textContent=PHASES[seg(frac)].name+(hol?' · '+hol:'')+' — tandai yang penting, atau baca kembali jejak hari itu.';
  renderAgendaList();
  renderDiary(key);
  el('agendaModal').classList.add('open');
  el('agendaInput').value='';
  requestAnimationFrame(()=>{ try{ el('agendaInput').focus({preventScroll:true}); }catch{} });
}
function closeAgenda(){
  el('agendaModal').classList.remove('open');
  agKey=null;
}

/* ---------- Catatan evaluasi ---------- */
const EMPTY_MSG={ suka:'masih kosong — halaman ini menunggu tinta kecil darimu…', kurang:'kosong pun boleh. hari yang berat tak wajib langsung beres…' };
function fillCol(col,arr){
  const ul=el(col+'List');
  ul.innerHTML=arr.length?arr.map(it=>`
    <li class="note-in flex items-start gap-2.5" data-id="${it.id}">
      <span class="mt-[9px] h-1.5 w-1.5 flex-none rotate-45" style="background:${col==='suka'?'rgba(185,145,63,.7)':EM()}"></span>
      <p class="min-w-0 flex-1 break-words font-script text-xl leading-snug text-ink/75">${esc(it.text)}</p>
      <button type="button" data-action="del" aria-label="Hapus catatan" class="mt-1 flex-none text-ink/30 transition-colors hover:text-eurus">
        <svg viewBox="0 0 24 24" class="h-3.5 w-3.5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><path d="M6 6l12 12M18 6L6 18"/></svg>
      </button>
    </li>`).join('')
    :`<li class="font-script text-lg italic text-ink/35">${EMPTY_MSG[col]}</li>`;
  el(col+'Count').textContent=arr.length
    ?(col==='suka'?`${arr.length} hal kecil tersimpan malam ini`:`${arr.length} hal untuk dipeluk, lalu dicoba besok`)
    :'belum ditulis';
}
function renderNotes(){
  const n=todayNotes();
  fillCol('suka',n.suka); fillCol('kurang',n.kurang);
}
function deleteNote(col,id){
  const arr=todayNotes()[col];
  const idx=arr.findIndex(n=>n.id===id);
  if(idx<0) return;
  const [item]=arr.splice(idx,1);
  saveNotes(); renderNotes();
  showToast('catatan dihapus',{ undo(){ const a=todayNotes()[col]; a.splice(Math.min(idx,a.length),0,item); saveNotes(); renderNotes(); } });
}

/* ---------- Mood ---------- */
function buildMoodBtns(){
  el('moodBtns').innerHTML=Object.keys(MOODS).map(k=>`
    <button type="button" class="mood-btn" data-mood="${k}" style="--c:${CCOL(MOODS[k])}" aria-pressed="false">
      ${moodFace(k)}
      <span class="ml">${MOODS[k].label}</span>
      <span class="ms">${MOODS[k].sub}</span>
    </button>`).join('');
}
function renderMoodUI(){
  const key=todayStr();
  const sel=moodDB[key]||null;
  document.querySelectorAll('#moodBtns .mood-btn').forEach(b=>b.setAttribute('aria-pressed',String(b.dataset.mood===sel)));
  el('moodIcon').innerHTML=moodFace(sel||'biasa');
  const d=new Date();
  if(sel){
    setFade('moodSay',MOODS[sel].say);
    el('moodPicked').textContent=`kau memilih: ${MOODS[sel].sub} · ${d.getDate()} ${MONTHS[d.getMonth()].toLowerCase()} ${d.getFullYear()}`;
  }else{
    setFade('moodSay','langit menunggu jawabmu — pelan-pelan saja.');
    el('moodPicked').textContent='belum dipilih hari ini';
  }
}

/* ---------- Toast ---------- */
function showToast(msg,opts){
  opts=opts||{};
  el('toastMsg').textContent=msg;
  pendingUndo=opts.undo||null;
  pendingPerm=opts.perm||null;
  el('permBtn').classList.toggle('hidden',!opts.perm);
  const t=el('toast');
  t.classList.remove('opacity-0','translate-y-3','invisible');
  clearTimeout(toastTimer);
  toastTimer=setTimeout(hideToast,6000);
}
function hideToast(){
  el('toast').classList.add('opacity-0','translate-y-3','invisible');
  pendingUndo=null; pendingPerm=null;
}
el('undoBtn').addEventListener('click',()=>{ if(pendingUndo) pendingUndo(); hideToast(); });
el('permBtn').addEventListener('click',()=>{ if(pendingPerm) pendingPerm(); hideToast(); });

/* ---------- Render semuanya ---------- */
function renderAll(){
  renderDate();
  renderHeroMoon();
  renderRing();
  renderList();
  renderWeek();
  renderCalendar();
  renderNextPhases();
  renderQuote();
  renderNotes();
  renderPrompts();
  renderMoodUI();
  renderLaikaDate();
}

/* ---------- Saklar tema ---------- */
function themeIconSVG(){
  const ring=isEcl()?'rgba(233,228,210,.4)':'rgba(43,38,32,.4)';
  if(isEcl()) return `<svg viewBox="0 0 40 40" class="h-9 w-9" aria-hidden="true">
    <circle cx="20" cy="20" r="18.5" fill="none" stroke="${ring}" stroke-width="1" stroke-dasharray="1.5 4"/>
    <circle cx="20" cy="20" r="14.5" fill="url(#moonLitE)" stroke="rgba(126,53,38,.9)" stroke-width="1.5"/>
    <path d="M9.5 12.5 A15 15 0 0 0 27.5 32.8 A16.5 16.5 0 0 1 9.5 12.5 Z" fill="rgba(26,10,8,.62)"/>
  </svg>`;
  return `<svg viewBox="0 0 40 40" class="h-9 w-9" aria-hidden="true">
    <circle cx="20" cy="20" r="18.5" fill="none" stroke="${ring}" stroke-width="1" stroke-dasharray="1.5 4"/>
    <circle cx="20" cy="20" r="14.5" fill="url(#moonLit)" stroke="rgba(43,38,32,.55)" stroke-width="1.5"/>
    <g fill="rgba(43,38,32,.1)"><circle cx="15" cy="16" r="2.4"/><circle cx="24" cy="23" r="1.7"/><circle cx="17" cy="26" r="1.1"/></g>
  </svg>`;
}
function renderThemeToggle(){
  el('themeMoonIcon').innerHTML=themeIconSVG();
  el('themeName').textContent=THEME_LABEL();
  el('themeToggle').setAttribute('aria-label',`Tema saat ini: ${THEME_LABEL()} — sentuh untuk berganti`);
}
function setTheme(t){
  if(theme===t) return;
  theme=t;
  try{ localStorage.setItem(THEME_KEY,t); }catch{}
  document.documentElement.classList.toggle('theme-eclipse',isEcl());
  const mt=el('metaTheme');
  if(mt) mt.setAttribute('content',isEcl()?'#141821':'#EFE8D8');
  if(isEcl()) applyEclipseTexture();
  document.documentElement.classList.add('theme-fade');
  setTimeout(()=>document.documentElement.classList.remove('theme-fade'),750);
  buildMoodBtns(); seedZodiac(); renderFooterPhases();
  renderAll(); renderThemeToggle();
}
el('themeToggle').addEventListener('click',()=>setTheme(isEcl()?'full':'eclipse'));

/* ---------- Mode edit aktivitas ---------- */
const SUBMIT_HTML=el('submitBtn').innerHTML;
function enterEdit(a){
  editingId=a.id;
  el('actName').value=a.name;
  el('actTime').value=a.time||'';
  el('actDuration').value=a.duration??'';
  setCat(a.category);
  el('submitBtn').textContent='Perbarui Aktivitas';
  el('cancelEdit').classList.remove('hidden');
  el('formSection').scrollIntoView({behavior:'smooth',block:'start'});
  el('actName').focus();
}
function exitEdit(){
  editingId=null;
  el('activityForm').reset();
  setCat(selectedCat);
  el('submitBtn').innerHTML=SUBMIT_HTML;
  el('cancelEdit').classList.add('hidden');
}
el('cancelEdit').addEventListener('click',exitEdit);

/* ---------- Kategori ---------- */
function setCat(cat){
  selectedCat=cat;
  document.querySelectorAll('#categoryPills .cat-pill')
    .forEach(b=>b.setAttribute('aria-pressed',String(b.dataset.cat===cat)));
}
el('categoryPills').addEventListener('click',e=>{
  const btn=e.target.closest('.cat-pill');
  if(btn) setCat(btn.dataset.cat);
});

/* ---------- Tambah / perbarui aktivitas ---------- */
el('activityForm').addEventListener('submit',e=>{
  e.preventDefault();
  const nameEl=el('actName');
  const name=nameEl.value.trim();
  if(!name){
    nameEl.classList.add('input-error','animate-shake');
    nameEl.focus();
    setTimeout(()=>nameEl.classList.remove('animate-shake'),400);
    return;
  }
  nameEl.classList.remove('input-error');
  const time=el('actTime').value||'';
  const durRaw=el('actDuration').value;
  const duration=durRaw?Math.max(1,parseInt(durRaw,10)):null;
  if(editingId){
    const a=activities.find(x=>x.id===editingId);
    if(a){ a.name=name; a.category=selectedCat; a.time=time; a.duration=duration; }
    save(); exitEdit(); renderAll();
    return;
  }
  const id=uid();
  activities.unshift({ id, origin:id, name, category:selectedCat, time, duration, done:false, date:todayStr() });
  save();
  e.target.reset();
  setCat(selectedCat);
  renderAll();
  nameEl.focus();
});
el('actName').addEventListener('input',e=>e.target.classList.remove('input-error'));

/* ---------- Satu handler daftar ---------- */
el('activityList').addEventListener('click',e=>{
  const li=e.target.closest('li[data-id]');
  if(!li) return;
  const id=li.dataset.id;
  const btn=e.target.closest('[data-action]');
  const action=btn?btn.dataset.action:'toggle';
  if(action==='edit'){
    const a=activities.find(x=>x.id===id);
    if(a) enterEdit(a);
    return;
  }
  if(action==='delete'){
    const idx=activities.findIndex(x=>x.id===id);
    if(idx<0) return;
    const item=activities[idx];
    const o=orig(item);
    const t=todayStr();
    if(!rmMap[t].includes(o)) rmMap[t].push(o);
    const [removed]=activities.splice(idx,1);
    save(); saveRm(); renderAll();
    showToast('aktivitas dihapus untuk hari ini',{
      undo(){
        const r=rmMap[todayStr()];
        const i=r.indexOf(o); if(i>=0) r.splice(i,1);
        saveRm();
        activities.splice(Math.min(idx,activities.length),0,removed);
        save(); renderAll();
      },
      perm(){
        if(!blocked.includes(o)) blocked.push(o);
        saveBlk();
        activities=activities.filter(x=>orig(x)!==o);
        save(); renderAll();
      },
    });
    return;
  }
  const a=activities.find(x=>x.id===id);
  if(!a) return;
  a.done=!a.done;
  save(); renderAll();
  if(a.done){
    const b=el('activityList').querySelector(`li[data-id="${a.id}"] .chk`);
    if(b){ b.classList.remove('pop'); void b.offsetWidth; b.classList.add('pop'); }
  }
});

/* ---------- Kutipan lainnya ---------- */
el('quoteShuffle').addEventListener('click',()=>renderQuote(true));

/* ---------- Catatan evaluasi ---------- */
['suka','kurang'].forEach(col=>{
  el(col+'Form').addEventListener('submit',e=>{
    e.preventDefault();
    const inp=el(col+'Input');
    const v=inp.value.trim();
    if(!v){
      inp.classList.add('input-error','animate-shake');
      setTimeout(()=>inp.classList.remove('animate-shake'),400);
      return;
    }
    inp.classList.remove('input-error');
    todayNotes()[col].unshift({id:uid(),text:v});
    saveNotes(); inp.value=''; renderNotes();
  });
  el(col+'List').addEventListener('click',e=>{
    const b=e.target.closest('[data-action="del"]');
    if(!b) return;
    const li=e.target.closest('li[data-id]');
    if(li) deleteNote(col,li.dataset.id);
  });
  el(col+'PromptBtn').addEventListener('click',()=>{
    const P=col==='suka'?P_SUKA:P_KURANG;
    if(col==='suka') piSuka=(piSuka+1)%P.length;
    else piKurang=(piKurang+1)%P.length;
    renderPrompts();
  });
});

/* ---------- Kalender ---------- */
el('calPrev').addEventListener('click',()=>{ calM--; if(calM<0){calM=11;calY--;} renderCalendar(); });
el('calNext').addEventListener('click',()=>{ calM++; if(calM>11){calM=0;calY++;} renderCalendar(); });
el('calToday').addEventListener('click',()=>{ const n=new Date(); calY=n.getFullYear(); calM=n.getMonth(); renderCalendar(); });
el('calGrid').addEventListener('click',e=>{
  const c=e.target.closest('[data-date]');
  if(c) openAgenda(c.dataset.date);
});
el('agendaModal').addEventListener('click',e=>{
  if(e.target.closest('[data-close]')){ closeAgenda(); return; }
  const b=e.target.closest('[data-action="del"]');
  if(!b||!agKey) return;
  const li=b.closest('li[data-id]');
  if(!li) return;
  const arr=agendaDB[agKey]||(agendaDB[agKey]=[]);
  const idx=arr.findIndex(x=>x.id===li.dataset.id);
  if(idx<0) return;
  const [item]=arr.splice(idx,1);
  saveAgenda(); renderAgendaList(); renderCalendar();
  const k=agKey;
  showToast('jadwal dihapus',{
    undo(){ const a=agendaDB[k]||(agendaDB[k]=[]); a.splice(Math.min(idx,a.length),0,item); saveAgenda(); renderCalendar(); if(k===agKey) renderAgendaList(); },
  });
});
el('agendaForm').addEventListener('submit',e=>{
  e.preventDefault();
  const inp=el('agendaInput');
  const v=inp.value.trim();
  if(!v||!agKey){
    if(!v){ inp.classList.add('input-error','animate-shake'); setTimeout(()=>inp.classList.remove('animate-shake'),400); }
    return;
  }
  inp.classList.remove('input-error');
  (agendaDB[agKey]||(agendaDB[agKey]=[])).unshift({id:uid(),text:v});
  saveAgenda(); inp.value=''; renderAgendaList(); renderCalendar();
  inp.focus();
});
el('agendaInput').addEventListener('input',e=>e.target.classList.remove('input-error'));
document.addEventListener('keydown',e=>{ if(e.key==='Escape'&&el('agendaModal').classList.contains('open')) closeAgenda(); });

/* ---------- Mood ---------- */
el('moodBtns').addEventListener('click',e=>{
  const b=e.target.closest('.mood-btn');
  if(!b) return;
  const k=b.dataset.mood, key=todayStr();
  moodDB[key]=(moodDB[key]===k)?undefined:k;
  if(moodDB[key]===undefined) delete moodDB[key];
  saveMood(); renderMoodUI(); renderCalendar();
});

/* ---------- Sentuh bulan ---------- */
el('heroMoon').addEventListener('keydown',e=>{
  if(e.key==='Enter'||e.key===' '){ e.preventDefault(); e.target.click(); }
});
el('heroMoon').addEventListener('click',()=>{
  if(cycling) return;
  cycling=true;
  const base=moonPhase(new Date()).frac;
  const t0=performance.now(), dur=2800;
  const tick=t=>{
    const p=Math.min(1,(t-t0)/dur);
    if(p>=1){ renderHeroMoon(); cycling=false; return; }
    renderHeroMoon((base+p)%1);
    requestAnimationFrame(tick);
  };
  requestAnimationFrame(tick);
});

/* ---------- Ekspor / Impor ---------- */
el('exportBtn').addEventListener('click',()=>{
  const payload={ app:'moonlitminds', v:1, exportedAt:new Date().toISOString(),
    activities, notes:noteDB, agenda:agendaDB, mood:moodDB, blocked };
  const blob=new Blob([JSON.stringify(payload,null,2)],{type:'application/json'});
  const a=document.createElement('a');
  a.href=URL.createObjectURL(blob);
  a.download=`moonlitminds-cadangan-${todayStr()}.json`;
  document.body.appendChild(a); a.click(); a.remove();
  setTimeout(()=>URL.revokeObjectURL(a.href),2000);
  showToast('cadangan diunduh',{});
});
el('importBtn').addEventListener('click',()=>el('importFile').click());
el('importFile').addEventListener('change',e=>{
  const f=e.target.files&&e.target.files[0];
  if(!f) return;
  const r=new FileReader();
  r.onload=()=>{
    try{
      const o=JSON.parse(r.result);
      if(!o||typeof o!=='object'||(!Array.isArray(o.activities)&&!o.notes&&!o.agenda))
        throw new Error('format');
      if(!confirm('Pulihkan cadangan ini? Semua data saat ini akan diganti.')){ e.target.value=''; return; }
      activities=Array.isArray(o.activities)?o.activities.filter(x=>x&&x.id&&x.name):[];
      noteDB=(o.notes&&typeof o.notes==='object'&&!Array.isArray(o.notes))?o.notes:{};
      agendaDB=(o.agenda&&typeof o.agenda==='object'&&!Array.isArray(o.agenda))?o.agenda:{};
      moodDB=(o.mood&&typeof o.mood==='object'&&!Array.isArray(o.mood))?o.mood:{};
      blocked=Array.isArray(o.blocked)?o.blocked:[];
      rmMap={};
      save(); saveNotes(); saveAgenda(); saveMood(); saveBlk(); saveRm();
      ensureAutoCarry(); renderAll();
      showToast('data dipulihkan',{});
    }catch{
      alert('Berkas ini sepertinya bukan cadangan MoonlitMinds yang sah. Pulihkan dibatalkan.');
    }
    e.target.value='';
  };
  r.readAsText(f);
});

/* ---------- Hapus semua ---------- */
el('clearAll').addEventListener('click',()=>{
  if(confirm('Hapus SEMUA data (aktivitas, catatan, jadwal & mood) dari perangkat ini? Tindakan ini tidak bisa dibatalkan.')){
    activities=[]; noteDB={}; agendaDB={}; moodDB={}; rmMap={}; blocked=[];
    save(); saveNotes(); saveAgenda(); saveMood(); saveRm(); saveBlk();
    wasAllDone=false;
    renderAll();
  }
});

/* ---------- Kartu malam ini ---------- */
el('shareBtn').addEventListener('click',async()=>{
  try{ await document.fonts.ready; }catch{}
  const items=todaysList();
  const done=items.filter(a=>a.done).length;
  const total=items.length;
  const pct=total?Math.round(done/total*100):0;
  const {frac}=moonPhase(new Date());
  const ph=PHASES[seg(frac)];
  const d=new Date();
  const streak=computeStreak();
  const ecl=isEcl();
  const paper=ecl?'#141821':'#EFE8D8';
  const inkC=ecl?'#F2EDE0':'#2B2620';
  const goldC=ecl?'#D8B563':'#B9913F';
  const dispFont=ecl?'"Cormorant Garamond", serif':'"Julius Sans One", sans-serif';
  const scriptFont=ecl?'"Lora", serif':'"Caveat", cursive';
  const c=document.createElement('canvas'); c.width=900; c.height=1150;
  const g=c.getContext('2d');
  g.fillStyle=paper; g.fillRect(0,0,900,1150);
  for(let i=0;i<70;i++){
    g.fillStyle=`rgba(185,145,63,${(0.1+Math.random()*0.4).toFixed(2)})`;
    g.beginPath(); g.arc(Math.random()*900,Math.random()*1150,0.6+Math.random()*1.4,0,7); g.fill();
  }
  g.strokeStyle=inkC; g.globalAlpha=.55; g.lineWidth=2;
  g.strokeRect(30,30,840,1090);
  g.setLineDash([2,7]); g.strokeRect(44,44,812,1062);
  g.setLineDash([]); g.globalAlpha=1;
  g.textAlign='center'; g.textBaseline='middle';
  g.fillStyle=goldC; g.font='600 30px '+dispFont;
  g.fillText('✳  M O O N L I T M I N D S  ✳',450,112);
  const cx=450, cy=430, R=205;
  g.strokeStyle=inkC; g.globalAlpha=.22; g.lineWidth=3;
  g.beginPath(); g.arc(cx,cy,R,0,7); g.stroke(); g.globalAlpha=1;
  if(pct>0){
    g.strokeStyle=goldC; g.lineWidth=13; g.lineCap='round';
    g.beginPath(); g.arc(cx,cy,R,-Math.PI/2,-Math.PI/2+pct/100*2*Math.PI); g.stroke();
  }
  g.fillStyle=inkC; g.font='600 150px '+dispFont;
  g.fillText(pct+'%',cx,cy+8);
  g.fillStyle=inkC; g.globalAlpha=.6; g.font='600 34px '+dispFont;
  g.fillText(`${done}/${total} selesai`,cx,cy+105); g.globalAlpha=1;
  g.fillStyle=inkC; g.globalAlpha=.75; g.font='italic 52px '+scriptFont;
  g.fillText(`${DAYS[d.getDay()]}, ${d.getDate()} ${MONTHS[d.getMonth()]} ${d.getFullYear()}`,450,745);
  g.globalAlpha=1;
  g.fillStyle=goldC; g.font='600 32px '+dispFont;
  g.fillText(ph.name.toUpperCase(),450,830);
  g.fillStyle=inkC; g.globalAlpha=.7; g.font='italic 42px '+scriptFont;
  g.fillText(streak>=1?`${streak} hari beruntun — kau tetap datang`:'malam ini halamanmu menunggu',450,900);
  g.globalAlpha=.45; g.font='600 24px '+dispFont;
  g.fillText('TUMBUH PELAN · TANPA SERVER · MILIKMU SEPENUHNYA',450,1060);
  g.globalAlpha=1;
  c.toBlob(blob=>{
    const a=document.createElement('a');
    a.href=URL.createObjectURL(blob);
    a.download=`moonlit-malam-ini-${todayStr()}.png`;
    document.body.appendChild(a); a.click(); a.remove();
    setTimeout(()=>URL.revokeObjectURL(a.href),2000);
  });
});

/* ---------- Latar: bintang ---------- */
(function seedStars(){
  let html='';
  for(let i=0;i<18;i++){
    const size=(1+Math.random()*1.6).toFixed(1);
    html+=`<span class="tw" style="left:${(Math.random()*96+2).toFixed(1)}vw;top:${(Math.random()*92+2).toFixed(1)}vh;width:${size}px;height:${size}px;--d:${(2.2+Math.random()*3.5).toFixed(1)}s;animation-delay:${(Math.random()*4).toFixed(1)}s"></span>`;
  }
  [[7,14],[90,22],[82,68]].forEach(([x,y],i)=>{
    html+=`<svg class="spark" style="left:${x}vw;top:${y}vh;animation-delay:${(i*1.3).toFixed(1)}s" width="10" height="10" viewBox="0 0 10 10" aria-hidden="true"><path d="M5 0 L6 4 L10 5 L6 6 L5 10 L4 6 L0 5 L4 4 Z" fill="currentColor"/></svg>`;
  });
  el('starfield').innerHTML=html;
})();
function seedSpeck(id,n,x0,x1,y0,y1){
  const g=el(id); let s='';
  for(let i=0;i<n;i++){
    const x=(x0+Math.random()*(x1-x0)).toFixed(1);
    const y=(y0+Math.random()*(y1-y0)).toFixed(1);
    const r=(0.3+Math.random()*1).toFixed(2);
    const o=(0.15+Math.random()*0.55).toFixed(2);
    s+=`<circle cx="${x}" cy="${y}" r="${r}" fill="rgba(233,228,210,${o})"/>`;
  }
  g.innerHTML=s;
}

/* ---------- Tekstur gerhana via canvas ---------- */
let texURL=null;
function eclipseTexture(){
  if(texURL) return texURL;
  const s=560, c=document.createElement('canvas'); c.width=c.height=s;
  const g=c.getContext('2d');
  g.fillStyle='#10141d'; g.fillRect(0,0,s,s);
  for(let i=0;i<42;i++){
    const x=Math.random()*s, y=Math.random()*s, r=50+Math.random()*150;
    const light=Math.random()<.55;
    const gr=g.createRadialGradient(x,y,0,x,y,r);
    gr.addColorStop(0,light?`rgba(34,44,64,${0.18+Math.random()*.22})`:`rgba(6,8,14,${0.25+Math.random()*.25})`);
    gr.addColorStop(1,'rgba(0,0,0,0)');
    g.fillStyle=gr; g.beginPath(); g.arc(x,y,r,0,7); g.fill();
  }
  for(let i=0;i<120;i++){
    g.fillStyle=`rgba(216,181,99,${0.25+Math.random()*.7})`;
    g.beginPath(); g.arc(Math.random()*s,Math.random()*s,0.4+Math.random()*1.1,0,7); g.fill();
  }
  for(let i=0;i<10;i++){
    g.fillStyle=`rgba(159,216,206,${0.2+Math.random()*.3})`;
    g.beginPath(); g.arc(Math.random()*s,Math.random()*s,0.5+Math.random()*.8,0,7); g.fill();
  }
  for(let i=0;i<8;i++){
    g.fillStyle=`rgba(245,239,223,${0.25+Math.random()*.3})`;
    g.beginPath(); g.arc(Math.random()*s,Math.random()*s,0.5+Math.random()*.7,0,7); g.fill();
  }
  for(let i=0;i<2600;i++){
    g.fillStyle=`rgba(216,181,99,${0.02+Math.random()*.05})`;
    g.fillRect(Math.random()*s,Math.random()*s,1,1);
  }
  texURL=c.toDataURL();
  return texURL;
}
function applyEclipseTexture(){ el('eclipseTex').style.backgroundImage=`url(${eclipseTexture()})`; }

/* ---------- PWA: manifest inline ---------- */
(function(){
  const icon="data:image/svg+xml,"+encodeURIComponent(
    "<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'><rect width='512' height='512' fill='#EFE8D8'/><circle cx='256' cy='256' r='190' fill='#B9913F'/><circle cx='330' cy='230' r='160' fill='#EFE8D8'/></svg>");
  const man={name:'MoonlitMinds',short_name:'Moonlit',description:'Pelacak harian di bawah cahaya bulan',
    start_url:'.',display:'standalone',background_color:'#EFE8D8',theme_color:'#EFE8D8',
    icons:[{src:icon,sizes:'any',type:'image/svg+xml',purpose:'any'}]};
  const l=document.createElement('link');
  l.rel='manifest';
  l.href='data:application/manifest+json,'+encodeURIComponent(JSON.stringify(man));
  document.head.appendChild(l);
})();

/* ---------- Ganti hari otomatis ---------- */
let _today=todayStr();
setInterval(()=>{
  if(todayStr()!==_today){
    _today=todayStr();
    currentQuoteIdx=null; wasAllDone=false;
    const n=new Date();
    calY=n.getFullYear(); calM=n.getMonth();
    piSuka=dayOfYear()%P_SUKA.length;
    piKurang=dayOfYear()%P_KURANG.length;
    ensureAutoCarry();
    renderAll();
  }
},30000);

/* ---------- Init ---------- */
activities=load();
noteDB=loadNotes();
agendaDB=loadAgenda();
moodDB=loadMood();
rmMap=loadRm();
blocked=loadBlk();
const now=new Date();
calY=now.getFullYear(); calM=now.getMonth();
piSuka=dayOfYear()%P_SUKA.length;
piKurang=dayOfYear()%P_KURANG.length;
seedSpeck('laikaSpeck',70,10,250,10,310);
seedSpeck('felSpeck',70,10,250,10,310);
document.documentElement.classList.toggle('theme-eclipse',isEcl());
if(isEcl()) applyEclipseTexture();
ensureAutoCarry();
buildMoodBtns();
seedZodiac();
renderFooterPhases();
setCat(selectedCat);
renderThemeToggle();
renderAll();
})();
</script>
</body>
</html>
