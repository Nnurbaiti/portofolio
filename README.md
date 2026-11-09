# Portofolio — Nurbaiti Nasiroh (Dark Theme)

Portofolio pribadi bertema dark mode + aksen biru, berbasis HTML & CSS statis, siap dipakai lewat GitHub Pages.

## Isi folder
```
index.html   -> halaman utama
style.css    -> semua styling
README.md    -> panduan ini
```

## Cara publish ke GitHub Pages

1. Buat repository baru di GitHub, misalnya beri nama `portofolio` atau `nurbaitinasiroh.github.io`
   (nama `username.github.io` akan langsung jadi domain utama akun kamu).
2. Upload `index.html` dan `style.css` ke repository tersebut
   (lewat tombol **Add file → Upload files** di GitHub, atau lewat `git push` dari komputer).
3. Buka tab **Settings** di repository → pilih menu **Pages** di sidebar kiri.
4. Di bagian **Build and deployment**, pilih **Source: Deploy from a branch**,
   lalu pilih branch `main` dan folder `/root`, klik **Save**.
5. Tunggu 1–2 menit, situs akan aktif di:
   - `https://<username>.github.io/<nama-repo>/` (jika nama repo bukan `username.github.io`), atau
   - `https://<username>.github.io/` (jika nama repo persis `username.github.io`)

## Sebelum upload, cek dua hal ini

- **Tombol "Unduh CV"** mengarah ke file bernama `cv.pdf`. Taruh file CV kamu di folder yang sama
  dengan `index.html` dan beri nama persis `cv.pdf`, supaya tombolnya langsung berfungsi.
- **Avatar** saat ini masih inisial "NN". Kalau mau pakai foto asli, ganti bagian ini di `index.html`:
  ```html
  <div class="avatar-circle">
    <span class="avatar-initials">NN</span>
  </div>
  ```
  dengan:
  ```html
  <div class="avatar-circle">
    <img src="foto.jpg" alt="Nurbaiti Nasiroh" style="width:100%;height:100%;object-fit:cover;border-radius:50%;">
  </div>
  ```
  lalu upload foto tersebut (misal `foto.jpg`) ke folder yang sama.

## Kalau mau edit warna
Semua warna ada di `style.css`, di bagian `:root{ ... }` paling atas file —
tinggal ganti kode warna `--accent` (biru) di sana kalau suatu saat ingin ganti aksen warna.
