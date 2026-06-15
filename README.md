# 💖 Heart Protocol v2.0

An interactive, premium 3D Heart presentation with an encrypted terminal decryption interface. Built using **React**, **Three.js / React Three Fiber**, **Tailwind CSS**, and **Framer Motion**.

---

## 🚀 Fitur Utama

- **Encrypted Terminal Intro**: Animasi bertema terminal ala hacker sebelum menampilkan konten utama.
- **Interactive 3D Heart**: Model jantung 3D yang interaktif, indah, dan responsif.
- **Glassmorphism Design**: Tampilan antarmuka modern dengan efek blur kaca dan skema warna gelap-pink yang harmonis.
- **Single HTML Bundle Ready**: Terkonfigurasi otomatis menggunakan `vite-plugin-singlefile` agar seluruh aset dibundel menjadi satu file HTML mandiri (`dist/index.html`) yang sangat portabel.

---

## 🛠️ Cara Menjalankan secara Lokal

### Prasyarat
Pastikan kamu sudah menginstal [Node.js](https://nodejs.org/).

### Langkah-langkah
1. **Instal Dependensi**:
   ```bash
   npm install
   ```

2. **Jalankan Server Development**:
   ```bash
   npm run dev
   ```
   Aplikasi akan berjalan secara lokal di `http://localhost:3000`.

3. **Build untuk Produksi**:
   ```bash
   npm run build
   ```
   Hasil build berupa file HTML tunggal akan berada di folder `dist/index.html`.

---

## 🌐 Cara Hosting (Deploy) ke GitHub Pages

Karena project ini dibuild menjadi file statis tunggal, kamu bisa menghostingnya dengan mudah di **GitHub Pages** menggunakan **GitHub Actions**.

### 1. Inisialisasi Git & Push ke GitHub
Jika kamu baru pertama kali mengunggahnya ke GitHub:
```bash
# Inisialisasi Git
git init

# Tambahkan semua file (.gitignore akan otomatis mengabaikan node_modules)
git add .

# Buat commit pertama
git commit -m "Initial commit"

# Hubungkan ke repositori GitHub kamu
git remote add origin https://github.com/USERNAME_KAMU/NAMA_REPO.git
git branch -M main
git push -u origin main
```

### 2. Buat File Deployment Workflow
1. Buat folder `.github/workflows/` di project kamu.
2. Buat file `deploy.yml` di dalamnya, lalu isi dengan script deployment GitHub Actions (gunakan template GitHub Pages untuk Vite).
3. Setelah di-push, pergi ke **Settings -> Pages** di repositori GitHub kamu, lalu ubah **Source** menjadi **GitHub Actions**.
