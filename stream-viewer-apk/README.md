# Jangrana Stream APK

APK WebView ringan untuk membuka viewer streaming Jangrana.

Default URL:

```text
https://stream.jangrana.my.id/mobile.html?v=34
```

Fallback URL saat gagal:

```text
https://live.jangrana.my.id/mobile.html?v=34
https://watch.jangrana.my.id/mobile.html?v=34
https://video.jangrana.my.id/mobile.html?v=34
https://cctv.jangrana.my.id/
https://jangrana.my.id/
```

## Build Tanpa Android Studio

Gunakan GitHub Actions:

1. Upload isi folder `stream-viewer-apk` ke repository GitHub baru.
2. Buka tab `Actions`.
3. Pilih workflow `Build APK`.
4. Klik `Run workflow`.
5. Download artifact `jangrana-stream-debug-apk`.

Output APK:

```text
app-debug.apk
```

## Build Lokal Jika Ada Gradle

```bash
gradle assembleDebug
```

APK akan dibuat di:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## Catatan

Debug APK cukup untuk install manual di HP, tapi akan muncul warning karena belum signed release.
Untuk distribusi luas, buat signing release key.
