# Portfolio Prompt Generator

Tool berbasis web untuk menghasilkan prompt terstruktur yang siap di-copy-paste ke AI (Claude, ChatGPT, dll.) untuk membuat website portfolio satu halaman (single-page) dalam satu file HTML.

## Cara Penggunaan

1. **Buka `index.html`** di browser (double-click atau drag ke browser).
2. **Isi data diri** — 4 langkah wizard: Identitas → Layanan → Proyek → Desain.
3. Atau pakai **"Coba Data Demo"** di header — pilih profesi, semua field terisi otomatis.
4. Klik **"Generate Prompt Sekarang"**.
5. **Copy** prompt yang muncul.
6. **Paste** ke AI (Claude, ChatGPT, Gemini, dll.) dan kirim.

## Yang Akan Dihasilkan AI

Satu file `index.html` siap pakai dengan:
- Navbar sticky + glassmorphism
- Hero section dengan CTA
- Tentang Saya + 3 keunggulan
- Layanan + Cara Kerja (timeline)
- Portfolio grid dengan filter
- Testimoni fiktif
- Kontak + footer
- Fully responsive, animasi scroll, custom scrollbar

## Jika AI Berhenti di Tengah Jalan

Prompt yang dihasilkan cukup panjang sehingga AI kadang berhenti sebelum kode selesai. Ini solusinya:

### 1. Minta Lanjutkan

Ketik perintah berikut di chat yang sama:

```
Lanjutkan dari bagian yang terpotong. Pastikan tidak ada kode yang hilang.
```

### 2. Split Prompt (Alternatif)

Kalau AI sering berhenti di percobaan pertama, kirim prompt bertahap:

**Batch 1 — Struktur & CSS:**
```
(Paste seluruh prompt, lalu tambahkan:)
Untuk saat ini, cukup berikan struktur HTML dan CSS lengkap dulu. Belum perlu JavaScript.
```

**Batch 2 — JavaScript:**
```
Sekarang berikan JavaScript untuk interaksi yang dibutuhkan: scroll navbar, IntersectionObserver animasi, filter proyek, hamburger menu, dan smooth scroll. Gabungkan ke dalam file HTML yang sudah kamu buat sebelumnya.
```

### 3. Gunakan AI dengan Output Lebih Panjang

Beberapa AI memiliki batas output yang berbeda:
- **Claude** — paling stabil untuk output kode panjang
- **ChatGPT GPT-4o** — bisa menghasilkan kode lengkap
- **Gemini 1.5 Pro** — konteks sangat besar, cocok untuk prompt kompleks
- **DeepSeek** — alternatif gratis dengan output panjang

Gunakan AI yang memiliki konteks besar agar kode tidak terpotong.

### 4. Generate Ulang dengan Prompt Lebih Ringkas

Jika masih bermasalah, buka **Edit Lagi** lalu kurangi jumlah proyek (cukup 2-3) atau layanan (cukup 2). Hasilnya akan lebih pendek dan AI lebih mungkin menyelesaikannya dalam satu respons.
