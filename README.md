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

### 📊 Visualisasi Progres
- **Ring Progress** — lingkaran persentase selesai hari ini
- **7-Day History** — jejak aktivitas seminggu terakhir dengan progress ring individual
- **Streak Counter** — hitung hari beruntun menyelesaikan ≥1 aktivitas

### 💭 Kutipan Motivasi Harian
- 42 kutipan inspiratif yang berganti setiap hari
- Deterministik — kutipan yang sama untuk satu hari
- Tombol shuffle untuk mengacak kutipan sewaktu-waktu

### 🎉 Perayaan Pencapaian
- Ucapan selamat otomatis saat semua aktivitas selesai
- Streak celebration untuk konsistensi Anda

### 💾 Simpan Lokal, Aman Pribadi
- Semua data disimpan di perangkat Anda menggunakan localStorage
- **Tanpa server, tanpa cloud** — privasi terjamin
- Fungsi undo untuk aktivitas yang dihapus (5 detik)

## 🎨 Desain & Estetika

**Palet Warna Khusus:**
- Paper: `#EFE8D8` — latar utama hangat
- Parchment: `#F5EFDF` — latar form
- Ink: `#2B2620` — teks utama
- Olive: `#5F6B4A` — aksen earthy
- Gold: `#B9913F` — highlight dan progress
- Notos, Eurus, Boreas — warna kategori

**Typography:**
- Display: Julius Sans One (judul, label)
- Script: Caveat (kutipan, aksen playful)
- Body: Spectral (deskripsi, isi)

**Elemen Visual:**
- Paper noise texture overlay
- SVG dekoratif (bintang, bulan, ornamen)
- Responsive design (mobile-first)
- Accessible (ARIA labels, focus management)

## 🛠 Stack Teknis

- **Frontend:** HTML5, CSS3 (Tailwind), Vanilla JavaScript
- **Storage:** LocalStorage (localStorage API)
- **Icons & Graphics:** SVG inline
- **Fonts:** Google Fonts (Julius Sans One, Caveat, Spectral)
- **Styling Framework:** Tailwind CSS 3
- **Tidak ada dependency eksternal** (pure vanilla stack)

## 📱 Browser Support

Mendukung semua browser modern dengan:
- ES6+ JavaScript
- CSS Grid & Flexbox
- LocalStorage API
- SVG support

## 🚀 Cara Penggunaan

### 1. Buka Website
Buka `index.html` di browser Anda (atau deploy ke hosting statis).

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

## 🔧 Struktur Data

Aktivitas disimpan sebagai object dalam array dengan struktur:

```javascript
{
  id: "unique-timestamp-based-id",
  name: "Nama Aktivitas",
  category: "produktivitas" | "kesehatan" | "hiburan" | "lainnya",
  time: "HH:MM" | "",
  duration: 30 | null,  // dalam menit
  done: boolean,
  date: "YYYY-MM-DD"
}
```

Disimpan di `localStorage` dengan key: `harian.v1`

## 🎯 Fitur Teknis Detail

### Kutipan Deterministik
- Menggunakan `dayOfYear()` untuk menghitung hari ke-berapa dalam setahun
- `currentQuoteIdx = dayOfYear() % QUOTES.length` — sama untuk satu hari
- Tombol shuffle manual untuk variasi

### Perhitungan Streak
- Iterasi mundur dari hari ini, cek apakah ada aktivitas selesai (`done: true`)
- Berhenti saat menemukan hari tanpa aktivitas selesai
- Display otomatis muncul saat streak ≥ 1

### Auto-refresh Harian
- `setInterval` setiap 30 detik mengecek `todayStr()`
- Jika berubah hari, reset `currentQuoteIdx` untuk kutipan baru
- Render ulang semua elemen

### Undo Mechanism
- Saat delete, simpan item dan indexnya di `lastDeleted`
- Toast muncul 5 detik dengan tombol "Urungkan"
- Jika diklik, item di-splice kembali di index yang sama

## 🌱 Development

### Modifikasi Kutipan
Edit array `QUOTES` dalam `<script>` untuk menambah/mengubah kutipan.

### Ubah Warna
Edit `tailwind.config` di tag `<style>` untuk mengubah palet warna.

### Tambah Kategori
Tambahkan key baru di object `CATS`, lalu tambahkan button di section kategori.

## 📄 Lisensi

Bebas digunakan, dimodifikasi, dan didistribusikan sesuai kebutuhan Anda.

## 🤝 Kontribusi

Ide, saran, atau perbaikan sangat diterima! Silakan buat issue atau diskusi untuk:
- Fitur baru
- Improvement desain
- Bug reports
- Saran kutipan

---

**Dibuat dengan 💙 untuk mereka yang ingin tumbuh perlahan, dengan konsisten, di bawah cahaya bulan.**

*"Satu langkah kecil hari ini lebih berat daripada seribu niat untuk besok."*<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title></title>
<meta name="description" content="Pelacak aktivitas harian dengan gaya stationery The Oh Hellos.">

<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Crect width='100' height='100' fill='%235F6B4A'/%3E%3Ccircle cx='50' cy='50' r='32' fill='none' stroke='%23C9A45C' stroke-width='6'/%3E%3C/svg%3E">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Julius+Sans+One&family=Caveat:wght@500;600&family=Spectral:ital,wght@0,300;0,400;0,500;1,300&display=swap" rel="stylesheet">

<script src="https://cdn.tailwindcss.com"></script>
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          paper:     '#EFE8D8',
          parchment: '#F5EFDF',
          ink:       '#2B2620',
          olive:     '#5F6B4A',
          gold:      '#B9913F',
          notos:     '#3A4A66',
          eurus:     '#93312E',
          boreas:    '#26241F',
        },
        fontFamily: {
          display: ['"Julius Sans One"', 'sans-serif'],
          script:  ['Caveat', 'cursive'],
          body:    ['Spectral', 'Georgia', 'serif'],
        },
        boxShadow: {
          card: '0 1px 2px rgba(43,38,32,.06), 0 18px 36px -24px rgba(43,38,32,.45)',
        },
      }
    }
  }
</script>

<style>
  .paper-noise{
    opacity:.07; mix-blend-mode:multiply;
    background-image:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='240' height='240'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='2' stitchTiles='stitch'/%3E%3CfeColorMatrix type='saturate' values='0'/%3E%3C/filter%3E%3Crect width='240' height='240' filter='url(%23n)'/%3E%3C/svg%3E");
  }

  ::selection{ background:rgba(185,145,63,.35); }
  :focus-visible{ outline:2px solid rgba(185,145,63,.85); outline-offset:2px; }

  .lbl{ display:block; font-family:'Julius Sans One',sans-serif; font-size:10px;
        letter-spacing:.3em; text-transform:uppercase; color:rgba(43,38,32,.55); margin-bottom:.45rem; }
  .inp{ width:100%; background:transparent; border:0; border-radius:0;
        border-bottom:1px solid rgba(43,38,32,.3); padding:.45rem .1rem;
        font-family:'Spectral',Georgia,serif; font-size:1rem; color:#2B2620; transition:border-color .2s; }
  .inp:focus{ outline:none; border-color:#5F6B4A; }
  .inp::placeholder{ color:rgba(43,38,32,.35); font-style:italic; }
  .input-error{ border-color:#93312E !important; }

  .cat-pill{ display:inline-flex; align-items:center; gap:.55rem; --c:#26241F;
             border:1px solid rgba(43,38,32,.25); background:transparent;
             padding:.45rem .85rem; font-size:.66rem; letter-spacing:.18em;
             text-transform:uppercase; color:rgba(43,38,32,.65); cursor:pointer; transition:all .18s; }
  .cat-pill .dot{ width:.55rem; height:.55rem; border-radius:9999px; background:var(--c); flex:none; }
  .cat-pill:hover{ border-color:var(--c); color:var(--c); }
  .cat-pill[aria-pressed="true"]{ border-color:var(--c); color:var(--c); box-shadow:inset 0 0 0 1px var(--c);
             background:rgba(0,0,0,.05); background:color-mix(in srgb, var(--c) 12%, transparent); }

  .badge{ font-size:10px; letter-spacing:.18em; text-transform:uppercase;
          border:1px solid; padding:1px 8px; white-space:nowrap; }

  @keyframes itemIn{ from{opacity:0; transform:translateY(-8px);} to{opacity:1; transform:translateY(0);} }
  .item-in{ animation:itemIn .35s ease both; }
  @keyframes shake{ 0%,100%{transform:translateX(0);} 25%{transform:translateX(-5px);} 75%{transform:translateX(5px);} }
  .animate-shake{ animation:shake .3s ease 1; }
  .chk{ transition:transform .12s ease, background-color .2s, border-color .2s; }
  .chk:active{ transform:scale(.85); }

  /* ★ BARU: animasi kutipan harian */
  @keyframes fadeUp{ from{opacity:0; transform:translateY(8px);} to{opacity:1; transform:translateY(0);} }
  .quote-in{ animation:fadeUp .6s ease both; }
</style>
</head>

<body class="min-h-screen bg-paper text-ink font-body antialiased">

  <div class="paper-noise pointer-events-none fixed inset-0 z-40" aria-hidden="true"></div>
  <svg viewBox="0 0 100 100" fill="currentColor" aria-hidden="true"
       class="pointer-events-none fixed right-[5%] top-24 w-24 text-ink opacity-[0.14] hidden md:block">
    <circle cx="50" cy="50" r="3"/><circle cx="62" cy="42" r="1.6"/><circle cx="40" cy="60" r="2.2"/>
    <circle cx="70" cy="58" r="1.2"/><circle cx="33" cy="40" r="1.4"/><circle cx="55" cy="66" r="1"/>
  </svg>
  <svg viewBox="0 0 100 100" fill="currentColor" aria-hidden="true"
       class="pointer-events-none fixed left-[4%] bottom-24 w-20 text-gold opacity-[0.22] hidden md:block">
    <circle cx="45" cy="55" r="2.6"/><circle cx="58" cy="46" r="1.4"/><circle cx="35" cy="42" r="1.8"/>
    <circle cx="62" cy="62" r="1.1"/><circle cx="50" cy="35" r="1.2"/>
  </svg>

  <main class="relative z-10 mx-auto w-full max-w-2xl px-4 sm:px-6 pb-16">

    <!-- ================= HEADER ================= -->
    <header class="pt-8 sm:pt-12 text-center select-none">
      <p class="font-display uppercase text-[11px] sm:text-xs tracking-[0.6em] pl-[0.6em] text-ink/55">Pelacak Aktivitas</p>

      <div class="relative mx-auto mt-8 h-44 w-44 sm:h-52 sm:w-52">
        <svg viewBox="0 0 160 160" class="h-full w-full -rotate-90" aria-hidden="true">
          <defs>
            <linearGradient id="goldGrad" x1="0" y1="0" x2="1" y2="1">
              <stop offset="0%" stop-color="#D8B563"/><stop offset="100%" stop-color="#A8842F"/>
            </linearGradient>
          </defs>
          <circle cx="80" cy="80" r="70" fill="none" stroke="#2B2620" stroke-opacity="0.12" stroke-width="2.5"/>
          <circle id="ringProgress" cx="80" cy="80" r="70" fill="none" stroke="url(#goldGrad)" stroke-width="5"
                  stroke-linecap="round" stroke-dasharray="0 439.82"
                  style="transition:stroke-dasharray .7s cubic-bezier(.4,0,.2,1)"/>
          <circle cx="80" cy="80" r="62" fill="none" stroke="#B9913F" stroke-opacity="0.35" stroke-width="1.2" stroke-dasharray="46 344"/>
          <circle cx="80" cy="80" r="76" fill="none" stroke="#2B2620" stroke-opacity="0.16" stroke-width="1" stroke-dasharray="1.5 6"/>
          <g fill="#B9913F" opacity="0.5">
            <circle cx="14" cy="34" r="2"/><circle cx="146" cy="26" r="1.4"/><circle cx="150" cy="112" r="2.2"/>
            <circle cx="10" cy="120" r="1.3"/><circle cx="132" cy="150" r="1.6"/>
          </g>
        </svg>
        <div class="absolute inset-0 flex flex-col items-center justify-center">
          <span id="ringPct" class="font-display text-3xl sm:text-4xl">0%</span>
          <span id="ringCount" class="mt-1 font-display uppercase text-[9px] tracking-[0.35em] pl-[0.35em] text-ink/55">0/0 selesai</span>
        </div>
      </div>

      <h1 class="font-display mt-8 text-[2.4rem] sm:text-5xl tracking-[0.45em] pl-[0.45em]">HARIAN</h1>
      <p class="font-script mt-2 text-2xl sm:text-[1.7rem] text-ink/60"><span id="dateLabel">…</span></p>

      <!-- ★ BARU: KATA MOTIVASI HARI INI -->
      <figure class="mx-auto mt-7 max-w-md">
        <div class="flex items-center justify-center gap-3">
          <span class="h-px w-8 bg-gold/60"></span>
          <figcaption class="font-display uppercase text-[9px] tracking-[0.35em] pl-[0.35em] text-gold">Kata Hari Ini</figcaption>
          <span class="h-px w-8 bg-gold/60"></span>
        </div>
        <blockquote id="quoteOfDay"
                    class="mt-2 font-script text-[1.6rem] sm:text-[1.8rem] leading-snug text-ink/70">
          …
        </blockquote>
        <button id="quoteShuffle" type="button"
                class="mt-2 font-display uppercase text-[9px] tracking-[0.3em] pl-[0.3em] text-ink/35 transition-colors hover:text-gold">
          ✳ kutipan lainnya
        </button>
      </figure>
    </header>

    <!-- ================= FORMULIR ================= -->
    <section class="mt-10 sm:mt-12">
      <div class="flex items-center gap-4">
        <span class="h-px flex-1 bg-ink/15"></span>
        <h2 class="font-display uppercase text-[11px] tracking-[0.4em] pl-[0.4em] text-ink/70">Catat Aktivitas</h2>
        <span class="h-px flex-1 bg-ink/15"></span>
      </div>

      <form id="activityForm" novalidate
            class="mt-5 border border-ink/15 bg-parchment p-5 sm:p-7 shadow-card">
        <label class="lbl" for="actName">Nama aktivitas</label>
        <input id="actName" type="text" class="inp" maxlength="80" autocomplete="off"
               placeholder="mis. Lari pagi keliling komplek">

        <p class="lbl mt-6">Kategori</p>
        <div id="categoryPills" class="mt-1 flex flex-wrap gap-2" role="group" aria-label="Pilih kategori">
          <button type="button" class="cat-pill" data-cat="produktivitas" style="--c:#3A4A66" aria-pressed="false"><span class="dot"></span>Produktivitas</button>
          <button type="button" class="cat-pill" data-cat="kesehatan"     style="--c:#5F6B4A" aria-pressed="false"><span class="dot"></span>Kesehatan</button>
          <button type="button" class="cat-pill" data-cat="hiburan"       style="--c:#93312E" aria-pressed="false"><span class="dot"></span>Hiburan</button>
          <button type="button" class="cat-pill" data-cat="lainnya"       style="--c:#26241F" aria-pressed="false"><span class="dot"></span>Lainnya</button>
        </div>

        <div class="mt-6 grid grid-cols-1 gap-6 sm:grid-cols-2">
          <div>
            <label class="lbl" for="actTime">Waktu · opsional</label>
            <input id="actTime" type="time" class="inp">
          </div>
          <div>
            <label class="lbl" for="actDuration">Durasi (menit) · opsional</label>
            <input id="actDuration" type="number" class="inp" min="1" max="1440" placeholder="mis. 30">
          </div>
        </div>

        <button type="submit"
                class="mt-8 inline-flex w-full items-center justify-center gap-3 bg-ink py-3.5 font-display uppercase
                       text-xs sm:text-sm tracking-[0.3em] pl-[0.3em] text-paper transition-colors hover:bg-olive active:translate-y-px">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round">
            <line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/>
          </svg>
          Catat Aktivitas
        </button>
      </form>
    </section>

    <!-- ================= DAFTAR HARI INI ================= -->
    <section class="mt-12">
      <div class="flex items-center gap-4">
        <span class="h-px flex-1 bg-ink/15"></span>
        <h2 class="font-display uppercase text-[11px] tracking-[0.4em] pl-[0.4em] text-ink/70">Kegiatan Hari Ini</h2>
        <span class="h-px flex-1 bg-ink/15"></span>
      </div>
      <p id="countText" aria-live="polite"
         class="mt-3 text-center font-display uppercase text-[10px] tracking-[0.3em] pl-[0.3em] text-ink/45">0 aktivitas</p>

      <!-- ★ BARU: label streak -->
      <p id="streakLabel" class="mt-2 hidden text-center font-display uppercase text-[10px] tracking-[0.3em] pl-[0.3em] text-gold">
        ✳ <span id="streakNum">0</span> hari beruntun
      </p>

      <ul id="activityList" class="mt-2"></ul>
      <p id="congrats" class="mt-6 hidden text-center font-script text-2xl text-olive"></p>
    </section>

    <!-- ================= RIWAYAT 7 HARI ================= -->
    <section class="mt-12">
      <div class="flex items-center gap-4">
        <span class="h-px flex-1 bg-ink/15"></span>
        <h2 class="font-display uppercase text-[11px] tracking-[0.4em] pl-[0.4em] text-ink/70">Tujuh Hari Terakhir</h2>
        <span class="h-px flex-1 bg-ink/15"></span>
      </div>
      <div id="weekStrip" class="mt-6 grid grid-cols-7 gap-1 sm:gap-2"></div>
    </section>

    <!-- ================= FOOTER ================= -->
    <footer class="mt-16 border-t border-ink/10 pt-10">
      <div class="flex items-center justify-center gap-5 select-none" aria-hidden="true">
        <div class="-rotate-6 border border-ink/25 bg-parchment p-1 shadow-sm">
          <div class="border border-dashed border-ink/40 px-4 py-2 text-center">
            <p class="font-display text-[8px] tracking-[0.35em] pl-[0.35em] text-ink/60">Satu Hari</p>
            <p class="font-script text-xl leading-tight text-ink/70">satu catatan kecil</p>
            <p class="font-display text-[8px] tracking-[0.35em] pl-[0.35em] text-ink/60">✳ Satu Langkah ✳</p>
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
            <textPath href="#pmCircle">HARIAN • POSTA • LOKAL •</textPath>
          </text>
          <text x="46" y="50" text-anchor="middle" font-size="12" fill="currentColor">✳</text>
        </svg>
      </div>
      <p class="mt-8 text-center font-display uppercase text-[10px] tracking-[0.25em] pl-[0.25em] text-ink/40">
        Data tersimpan otomatis di perangkat ini · tanpa server ·
        <button id="clearAll" class="underline underline-offset-4 transition-colors hover:text-eurus">hapus semua data</button>
      </p>
    </footer>
  </main>

  <div id="toast" role="status" aria-live="polite"
       class="pointer-events-none fixed bottom-6 left-1/2 z-50 -translate-x-1/2 translate-y-3 opacity-0 transition-all duration-300">
    <div class="flex items-center gap-4 bg-ink py-3 pl-5 pr-3 text-paper shadow-lg">
      <span class="font-display uppercase text-[11px] tracking-[0.2em]">Aktivitas dihapus</span>
      <button id="undoBtn"
              class="border border-gold/60 px-3 py-1.5 font-display uppercase text-[10px] tracking-[0.25em] pl-[0.25em] text-gold transition-colors hover:text-[#E4C57C]">
        Urungkan
      </button>
    </div>
  </div>

<script>
(function () {
  'use strict';

  /* ---------- Konstanta & util ---------- */
  const KEY = 'harian.v1';
  const CATS = {
    produktivitas: { label: 'Produktivitas', color: '#3A4A66' },
    kesehatan:     { label: 'Kesehatan',     color: '#5F6B4A' },
    hiburan:       { label: 'Hiburan',       color: '#93312E' },
    lainnya:       { label: 'Lainnya',       color: '#26241F' },
  };
  const CIRC  = 2 * Math.PI * 70;
  const CIRC2 = 2 * Math.PI * 16;
  const DAYS  = ['Minggu','Senin','Selasa','Rabu','Kamis','Jumat','Sabtu'];
  const MONTHS= ['Januari','Februari','Maret','April','Mei','Juni','Juli','Agustus','September','Oktober','November','Desember'];

  /* ★ BARU: 42 kutipan motivasi orisinal — berganti otomatis tiap hari */
  const QUOTES = [
    'Langit tak pernah terlambat berganti warna — begitu pula kamu.',
    'Satu langkah kecil hari ini lebih berat daripada seribu niat untuk besok.',
    'Akar tumbuh diam-diam di tempat gelap. Begitu pula usahamu.',
    'Musim tidak berlomba; ia datang tepat waktu. Kamu pun boleh begini.',
    'Hujan hari ini adalah air untuk bunga bulan depan.',
    'Yang penting bukan seberapa cepat, melainkan tetap berjalan.',
    'Pohon besar dulunya biji yang tak diperhatikan siapa pun.',
    'Istirahat bukan menyerah — sungai pun berkolam sebelum melanjutkan arus.',
    'Mencoba lagi bukan berarti gagal dua kali; itu tanda kamu belum menyerah.',
    'Matahari tak minta izin untuk terbit. Kamu tak perlu menunggu sempurna.',
    'Kerjakan yang terjangkau hari ini; sisanya, biar angin yang menyambung.',
    'Setiap daun yang gugur adalah keberanian untuk tumbuh lagi.',
    'Kamu tidak harus menyala tiap hari — bara kecil pun tetap hangat.',
    'Jadilah lembut pada dirimu; kamu sedang tumbuh, bukan berpacu.',
    'Awan berlalu, badai berlalu — kamu yang tetap berdiri di sini.',
    'Disiplin adalah memilih yang paling penting, bukan mengurus semuanya.',
    'Hari yang biasa saja pun berarti: kamu hadir, dan itu cukup.',
    'Bintang butuh langit gelap agar terlihat. Masa sulit pun begitu.',
    'Mulailah kecil, mulailah jujur, mulailah hari ini.',
    'Tak semua hari dibuat untuk produktif; sebagian dibuat untuk bernapas.',
    'Burung tak takut cabangnya retak, karena percaya pada sayapnya.',
    'Menulis ulang ceritamu dimulai dari satu kalimat hari ini.',
    'Apa yang kamu rawat hari ini adalah kekuatanmu esok hari.',
    'Pelankan langkah bukan berarti kalah — itu cara menyiasati jalan.',
    'Setiap centang kecil adalah janji yang kamu tepati pada dirimu sendiri.',
    'Angin musim semi selalu datang setelah musim terdingin.',
    'Gagal adalah data, bukan identitas.',
    'Kebaikan kecil yang rutin mengalahkan usaha besar yang sesekali.',
    'Hari ini mungkin berat, tapi kamu lebih kuat daripada kemarin.',
    'Jangan menunggu motivasi; mulailah, dan ia akan menyusul.',
    'Tumbuh tak selalu terlihat — percayalah pada akar.',
    'Waktu terbaik menanam adalah kemarin; waktu berikutnya adalah sekarang.',
    'Setiap pagi adalah halaman kosong — tulis dengan tinta emas.',
    'Yang konsisten mengalahkan yang sempurna.',
    'Ucapkan terima kasih pada dirimu yang kemarin memilih bertahan.',
    'Angin tak bertanya arah; ia bertiup, lalu jalannya menjadi jalan.',
    'Lambat bukan hambatan — itu jeda untuk berakar lebih dalam.',
    'Bandingkan dirimu hari ini dengan dirimu kemarin, bukan dengan orang lain.',
    'Segala yang berat sedang membentuk sayap yang belum kamu lihat.',
    'Selesai lebih baik daripada sempurna.',
    'Hari ini milikmu — isi dengan hal yang membuatmu bertumbuh.',
    'Senja tak pernah menyesal telah bersinar sepanjang hari. Kamu juga tak perlu.',
  ];

  /* ★ BARU: ucapan selamat acak saat semua selesai */
  const CONGRATS = [
    'semua selesai — angin hari ini berpihak padamu ✳',
    'tuntas! tarik napas panjang, kamu luar biasa ✳',
    'seluruh centang terkumpul — selamat beristirahat ✳',
    'hari ini ditutup sempurna. terima kasih sudah gigih ✳',
    'tak ada sisa! akar kebiasaanmu tumbuh makin kuat ✳',
  ];

  const el   = id => document.getElementById(id);
  const esc  = s => String(s).replace(/[&<>"']/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
  const pad  = n => String(n).padStart(2, '0');
  const todayStr = (d = new Date()) => `${d.getFullYear()}-${pad(d.getMonth()+1)}-${pad(d.getDate())}`;
  const uid = () => Date.now().toString(36) + Math.random().toString(36).slice(2, 7);

  /* ★ BARU: hari ke-berapa dalam setahun (untuk rotasi kutipan) */
  function dayOfYear(d = new Date()) {
    return Math.floor((d - new Date(d.getFullYear(), 0, 0)) / 86400000);
  }

  /* ---------- State ---------- */
  let activities = [];
  let selectedCat = 'produktivitas';
  let lastDeleted = null;
  let toastTimer  = null;
  let currentQuoteIdx = null; // ★

  function load() {
    try {
      const arr = JSON.parse(localStorage.getItem(KEY) || '[]');
      return Array.isArray(arr) ? arr.filter(a => a && a.id && a.name) : [];
    } catch { return []; }
  }
  function save() { try { localStorage.setItem(KEY, JSON.stringify(activities)); } catch {} }

  /* ---------- Render ---------- */
  function renderDate() {
    const d = new Date();
    el('dateLabel').textContent =
      `${DAYS[d.getDay()]}, ${d.getDate()} ${MONTHS[d.getMonth()]} ${d.getFullYear()}`.toLowerCase();
  }

  /* ★ BARU: kutipan harian — deterministik per hari, bisa diacak manual */
  function renderQuote(forceNew = false) {
    const total = QUOTES.length;
    if (currentQuoteIdx === null) {
      currentQuoteIdx = dayOfYear() % total;          // kutipan tetap untuk hari ini
    } else if (forceNew) {
      let idx;
      do { idx = Math.floor(Math.random() * total); } while (idx === currentQuoteIdx);
      currentQuoteIdx = idx;
    }
    const q = el('quoteOfDay');
    q.textContent = '\u201C' + QUOTES[currentQuoteIdx] + '\u201D';
    q.classList.remove('quote-in');
    void q.offsetWidth;                                // restart animasi
    q.classList.add('quote-in');
  }
  el('quoteShuffle').addEventListener('click', () => renderQuote(true));

  function todaysList() { return activities.filter(a => a.date === todayStr()); }

  /* ★ BARU: streak — hari beruntun menyelesaikan ≥1 aktivitas */
  function computeStreak() {
    const doneOn = key => activities.some(a => a.date === key && a.done);
    const d = new Date();
    if (!doneOn(todayStr(d))) d.setDate(d.getDate() - 1); // hari ini belum selesai → hitung dari kemarin
    let s = 0;
    while (doneOn(todayStr(d))) { s++; d.setDate(d.getDate() - 1); }
    return s;
  }
  function renderStreak() {
    const s = computeStreak();
    const lbl = el('streakLabel');
    if (s >= 1) { lbl.classList.remove('hidden'); el('streakNum').textContent = s; }
    else lbl.classList.add('hidden');
  }

  function renderRing() {
    const items = todaysList();
    const done  = items.filter(a => a.done).length;
    const total = items.length;
    const pct   = total ? Math.round(done / total * 100) : 0;
    el('ringProgress').setAttribute('stroke-dasharray', `${pct / 100 * CIRC} ${CIRC}`);
    el('ringPct').textContent   = pct + '%';
    el('ringCount').textContent = `${done}/${total} selesai`;
    el('countText').textContent = total ? `${done} dari ${total} selesai` : 'belum ada aktivitas';

    const allDone = total > 0 && done === total;
    const c = el('congrats');
    c.classList.toggle('hidden', !allDone);
    if (allDone) c.textContent = CONGRATS[Math.floor(Math.random() * CONGRATS.length)]; // ★ acak
    renderStreak(); // ★
  }

  function renderList() {
    const items = todaysList();
    const list  = el('activityList');

    if (!items.length) {
      list.innerHTML = `
        <li class="list-none py-10 text-center">
          <div class="mx-auto h-24 w-24 rounded-full border-2 border-dashed border-ink/25"></div>
          <p class="font-script mt-4 text-3xl text-ink/60">belum ada catatan hari ini…</p>
          <p class="mt-1 font-display uppercase text-[10px] tracking-[0.3em] pl-[0.3em] text-ink/40">tulis aktivitas pertamamu di formulir atas</p>
        </li>`;
      return;
    }

    list.innerHTML = items.map(a => {
      const c    = CATS[a.category] || CATS.lainnya;
      const meta = [a.time, a.duration ? a.duration + ' mnt' : null].filter(Boolean).join(' · ');
      return `
      <li data-id="${a.id}" class="group flex items-center gap-3 border-b border-ink/10 py-3.5 transition-opacity ${a.done ? 'opacity-60' : ''}">
        <button type="button" data-action="toggle" aria-pressed="${a.done}"
                title="${a.done ? 'Tandai belum selesai' : 'Tandai selesai'}"
                class="chk flex h-6 w-6 shrink-0 items-center justify-center rounded-full border-2
                       ${a.done ? 'border-gold bg-gold' : 'border-ink/35 hover:border-gold'}">
          <svg viewBox="0 0 24 24" class="h-3.5 w-3.5 text-paper ${a.done ? 'opacity-100' : 'opacity-0'}"
               fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round">
            <polyline points="20 6 9 17 4 12"/>
          </svg>
        </button>
        <div class="min-w-0 flex-1">
          <p class="truncate ${a.done ? 'line-through decoration-ink/40' : ''}">${esc(a.name)}</p>
          <div class="mt-1 flex flex-wrap items-center gap-x-2 gap-y-1">
            <span class="badge" style="color:${c.color};border-color:${c.color}66">${c.label}</span>
            ${meta ? `<span class="uppercase text-[11px] tracking-[0.14em] text-ink/45">${meta}</span>` : ''}
          </div>
        </div>
        <button type="button" data-action="delete" title="Hapus aktivitas"
                class="shrink-0 p-2 text-ink/35 transition-all hover:text-eurus focus:text-eurus
                       opacity-70 md:opacity-0 md:group-hover:opacity-100">
          <svg viewBox="0 0 24 24" class="h-4 w-4" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round">
            <line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/>
          </svg>
        </button>
      </li>`;
    }).join('');
  }

  function renderWeek() {
    const strip = el('weekStrip');
    const DAY_S = ['Min','Sen','Sel','Rab','Kam','Jum','Sab'];
    const MON_S = ['Jan','Feb','Mar','Apr','Mei','Jun','Jul','Agu','Sep','Okt','Nov','Des'];
    let html = '';
    for (let i = 6; i >= 0; i--) {
      const d = new Date(); d.setDate(d.getDate() - i);
      const key   = todayStr(d);
      const items = activities.filter(a => a.date === key);
      const done  = items.filter(a => a.done).length;
      const total = items.length;
      const frac  = total ? done / total : 0;
      const isToday = i === 0;
      html += `
        <div class="flex flex-col items-center gap-1"
             title="${DAYS[d.getDay()]}, ${d.getDate()} ${MON_S[d.getMonth()]}${isToday ? ' (hari ini)' : ''} — ${done}/${total} selesai">
          <svg width="40" height="40" viewBox="0 0 40 40" class="-rotate-90" aria-hidden="true">
            <circle cx="20" cy="20" r="16" fill="none" stroke="rgba(43,38,32,.12)" stroke-width="2"
                    ${total ? '' : 'stroke-dasharray="3 4"'}/>
            <circle cx="20" cy="20" r="16" fill="none" stroke="#B9913F" stroke-width="3" stroke-linecap="round"
                    stroke-dasharray="${frac * CIRC2} ${CIRC2}" style="transition:stroke-dasharray .6s ease"/>
          </svg>
          <span class="text-[10px] tracking-widest ${isToday ? 'font-medium text-ink border-b-2 border-gold' : 'text-ink/45'}">${DAY_S[d.getDay()]}</span>
          <span class="text-[9px] text-ink/40">${done}/${total}</span>
        </div>`;
    }
    strip.innerHTML = html;
  }

  function renderAll() { renderDate(); renderRing(); renderList(); renderWeek(); renderQuote(); }

  /* ---------- Kategori ---------- */
  function setCat(cat) {
    selectedCat = cat;
    document.querySelectorAll('#categoryPills .cat-pill').forEach(btn =>
      btn.setAttribute('aria-pressed', String(btn.dataset.cat === cat)));
  }
  el('categoryPills').addEventListener('click', e => {
    const btn = e.target.closest('.cat-pill');
    if (btn) setCat(btn.dataset.cat);
  });

  /* ---------- Tambah aktivitas ---------- */
  el('activityForm').addEventListener('submit', e => {
    e.preventDefault();
    const nameEl = el('actName');
    const name   = nameEl.value.trim();
    if (!name) {
      nameEl.classList.add('input-error', 'animate-shake');
      nameEl.focus();
      setTimeout(() => nameEl.classList.remove('animate-shake'), 400);
      return;
    }
    nameEl.classList.remove('input-error');
    const time     = el('actTime').value || '';
    const durRaw   = el('actDuration').value;
    const duration = durRaw ? Math.max(1, parseInt(durRaw, 10)) : null;

    activities.unshift({ id: uid(), name, category: selectedCat, time, duration, done: false, date: todayStr() });
    save();
    e.target.reset();
    setCat(selectedCat);
    renderAll();
    const first = el('activityList').firstElementChild;
    if (first && first.dataset.id) first.classList.add('item-in');
    nameEl.focus();
  });
  el('actName').addEventListener('input', e => e.target.classList.remove('input-error'));

  /* ---------- Centang & hapus ---------- */
  el('activityList').addEventListener('click', e => {
    const btn = e.target.closest('[data-action]');
    if (!btn) return;
    const li = e.target.closest('li[data-id]');
    if (!li) return;
    const id = li.dataset.id;

    if (btn.dataset.action === 'toggle') {
      const a = activities.find(x => x.id === id);
      if (a) { a.done = !a.done; save(); renderAll(); }
    }
    if (btn.dataset.action === 'delete') {
      const idx = activities.findIndex(x => x.id === id);
      if (idx < 0) return;
      lastDeleted = { item: activities[idx], index: idx };
      activities.splice(idx, 1);
      save(); renderAll(); showToast();
    }
  });

  /* ---------- Toast urungkan ---------- */
  function showToast() {
    const t = el('toast');
    t.classList.remove('opacity-0', 'translate-y-3', 'pointer-events-none');
    clearTimeout(toastTimer);
    toastTimer = setTimeout(hideToast, 5000);
  }
  function hideToast() {
    el('toast').classList.add('opacity-0', 'translate-y-3', 'pointer-events-none');
  }
  el('undoBtn').addEventListener('click', () => {
    if (lastDeleted) {
      activities.splice(Math.min(lastDeleted.index, activities.length), 0, lastDeleted.item);
      lastDeleted = null;
      save(); renderAll();
    }
    hideToast();
  });

  /* ---------- Hapus semua ---------- */
  el('clearAll').addEventListener('click', () => {
    if (confirm('Hapus SEMUA data aktivitas dari perangkat ini? Tindakan ini tidak bisa dibatalkan.')) {
      activities = []; save(); renderAll();
    }
  });

  /* ---------- Ganti hari otomatis ---------- */
  let _today = todayStr();
  setInterval(() => {
    const t = todayStr();
    if (t !== _today) {
      _today = t;
      currentQuoteIdx = null; // ★ paksa ambil kutipan hari baru
      renderAll();
    }
  }, 30000);

  /* ---------- Init ---------- */
  activities = load();
  setCat(selectedCat);
  renderAll();
})();
</script>
</body>
</html>
