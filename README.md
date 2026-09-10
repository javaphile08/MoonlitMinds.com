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

*"Satu langkah kecil hari ini lebih berat daripada seribu niat untuk besok."*
