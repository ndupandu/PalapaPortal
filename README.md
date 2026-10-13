# Palapanet STB (WebView APK)

Aplikasi Android sederhana yang membuka `https://palapanetstb.duckdns.org:121/c`.

## Cara pakai
1. Buat repo baru di GitHub, lalu push seluruh isi folder ini ke branch `main`.
2. Buka tab **Actions** → workflow **Build APK** berjalan otomatis.
3. Setelah selesai, unduh APK di bagian **Artifacts** (`PalapanetSTB-debug`).
4. Pasang APK di HP (izinkan "Install dari sumber tidak dikenal").

## Ganti URL / nama aplikasi
- URL: `app/build.gradle` → `START_URL`
- Nama: `app/src/main/res/values/strings.xml`
- Ikon: `app/src/main/res/drawable/ic_launcher.xml`

## Fitur
Tombol back navigasi web, tarik-untuk-refresh, progress bar, upload file, unduhan,
halaman error saat offline, dan cookie/session tersimpan.

## Catatan sertifikat SSL
Jika situs memakai sertifikat self-signed, halaman akan gagal dimuat (perilaku aman).
Solusi terbaik: pakai sertifikat valid (mis. Let's Encrypt untuk domain DuckDNS).
