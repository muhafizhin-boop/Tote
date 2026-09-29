# Strategi Berurutan (APK)

Cara mendapatkan APK tanpa memasang Android Studio:

1. Buat akun GitHub (kalau belum punya), lalu buat repository baru (boleh private).
2. Upload SEMUA isi folder ini ke repository tersebut, termasuk folder `.github`.
   Pastikan file `.github/workflows/build-apk.yml` ikut terunggah.
3. Buka tab **Actions** di repository. Workflow "Build APK" akan jalan otomatis
   (atau klik "Run workflow"). Tunggu sekitar 5-10 menit sampai centang hijau.
4. Klik run yang berhasil, lalu unduh **strategi-berurutan-apk** di bagian Artifacts.
   Ekstrak zip-nya, hasilnya `app-debug.apk`.
5. Kirim APK ke HP, buka, dan izinkan "Pasang dari sumber tidak dikenal" jika diminta.

Mengubah isi aplikasi: edit `www/index.html`, commit, dan workflow akan membuat APK baru.

Catatan: ini APK debug (cukup untuk dipakai pribadi). Untuk Play Store diperlukan
build release yang ditandatangani.
