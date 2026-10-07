# Dompetku – versi uji coba APK

Aplikasi pencatat keuangan (PWA). Alamat setelah diunggah:
https://tofanhidayat94.github.io/dompetku/

## Isi repo
- `dompetku/`  : aplikasi (index.html, manifest, service worker, ikon)
- `.well-known/assetlinks.json` : penghubung domain dengan APK (menghilangkan bilah alamat)
- `.nojekyll`  : agar GitHub Pages menyajikan folder `.well-known`

## Catatan versi uji coba
- Data tersimpan di HP (penyimpanan lokal). Belum ada sinkronisasi antar HP.
- Scan struk belum aktif di versi ini.
- Akun dan data bersifat lokal di perangkat; jangan pakai kata sandi asli.

## Langkah singkat
1. Unggah semua isi folder ini ke repo `tofanhidayat94.github.io` (akar repo).
2. Settings -> Pages -> Deploy from a branch -> main / (root).
3. Buka https://tofanhidayat94.github.io/dompetku/ di Chrome HP dan pastikan tampil.
4. Buat APK di pwabuilder.com (Android, mode Standalone), catat Package ID.
5. Dari zip PWABuilder, salin SHA-256 di `signing-key-info.txt`.
6. Isi `.well-known/assetlinks.json` (package_name dan fingerprint), commit.
7. Buka https://tofanhidayat94.github.io/.well-known/assetlinks.json, harus langsung tampil JSON.
8. Hapus APK lama, pasang APK baru. Bilah alamat di atas akan hilang.
Simpan file keystore dari PWABuilder; dibutuhkan untuk memperbarui APK nanti.
