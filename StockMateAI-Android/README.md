# StockMate AI - Android (APK)

Membungkus `StockMate_AI_V2_Gemini.html` ke dalam WebView
(file ada di `app/src/main/assets/index.html`). Data & API key tersimpan
di localStorage perangkat, sama seperti saat dibuka di browser.

## Cara 1 - Build online (tanpa Android Studio)
1. Buat repository baru di GitHub, upload SEMUA isi folder ini
   (termasuk folder tersembunyi `.github`).
2. Buka tab Actions -> workflow "Build APK" -> tunggu +-3-5 menit sampai hijau.
3. Buka run tersebut -> bagian Artifacts -> unduh `StockMateAI-apk` (zip) -> ekstrak
   -> `app-debug.apk`.
4. Kirim ke HP, izinkan "Install dari sumber tidak dikenal", lalu install.

## Cara 2 - Android Studio
File -> Open folder ini -> tunggu Gradle sync -> Build -> Build APK(s).
Hasil: `app/build/outputs/apk/debug/app-debug.apk`.

## Mengubah isi aplikasi
Ganti `app/src/main/assets/index.html` dengan HTML baru, lalu build ulang.
