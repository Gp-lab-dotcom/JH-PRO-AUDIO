# JH PRO AUDIO DLMS (Web App / APK)

Aplikasi kontrol DSP via **Web Bluetooth**. Dipasang lewat GitHub Pages, lalu bisa di-install ke HP seperti aplikasi.

## 1. Upload ke GitHub
1. Buat repository baru di github.com (misal `jhpro-app`), **Public**.
2. Upload semua isi folder ini (termasuk folder `.github` dan `icons`).
3. Buka **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Tab **Actions**: tunggu workflow "Deploy ke GitHub Pages" hijau.
5. Alamat aplikasi: `https://USERNAME.github.io/jhpro-app/`

## 2. Install di Android (paling mudah)
Buka alamat di atas pakai **Chrome**, menu ⋮ → **Install app / Tambahkan ke layar utama**.

## 3. Jadi file APK
1. Buka https://www.pwabuilder.com
2. Tempel alamat GitHub Pages Anda → Start → Package for stores → **Android**.
3. Download APK/AAB hasilnya dan install.

## Catatan penting
- Web Bluetooth hanya jalan di **Chrome/Edge Android** dan butuh **HTTPS**. APK "WebView" biasa tidak mendukungnya, makanya dipakai PWA/TWA (APK dari PWABuilder jalan lewat Chrome).
- Tidak jalan di iPhone/Safari.
- Setelah update `index.html`, ganti `V` di `sw.js` (mis. `jhpro-v2`) agar cache diperbarui.
