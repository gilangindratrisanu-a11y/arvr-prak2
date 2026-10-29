# Tugas AR Minggu 2 — Scene v1

## Isi proyek
- `index.html`: scene AR berbasis A-Frame + AR.js.
- `assets/tekstur.jpg`: tekstur untuk kotak.

## Menjalankan
1. Jalankan local server dari folder proyek, misalnya VS Code Live Server.
2. Buka alamat server di HP yang terhubung ke Wi-Fi yang sama.
3. Izinkan akses kamera.
4. Arahkan kamera ke marker Hiro.

Untuk akses kamera HP, HTTPS lebih disarankan. HTTP lokal kadang diblokir browser modern.

## Checklist pengujian
- [ ] Alas transparan terlihat.
- [ ] Kubus biru muncul di kiri.
- [ ] Bola oranye bergerak naik-turun.
- [ ] Silinder hijau berputar dan penandanya terlihat bergerak.
- [ ] Kotak bertekstur muncul di depan.
- [ ] Scene berhasil diuji di HP.
- [ ] Screenshot/foto hasil disimpan.

## Catatan eksperimen
Isi hasil setelah pengujian nyata.

| No | Perubahan | Prediksi | Hasil pengamatan |
|---|---|---|---|
| 1 | Posisi kubus Y: `0.25` → `0.75` | Kubus naik | ... |
| 2 | Rotasi kubus: `0 45 0` | Kubus berputar 45° | ... |
| 3 | Skala bola: `1 2 1` | Bola menjadi lonjong | ... |
| 4 | Animasi silinder ke `36 0 0` | Silinder jungkir-balik | ... |
| 5 | Posisi kotak Z: `0.7` → `-0.7` | Kotak pindah ke sisi lain | ... |
| 6 | Ambient `0.6` → `0.1` | Objek lebih gelap | ... |
| 7 | Hapus directional light | Objek lebih datar | ... |
| 8 | Metalness `0.9`, roughness `0.1` | Bola lebih mengilap | ... |

## Git
```bash
git add index.html assets/tekstur.jpg README.md
git commit -m "feat: scene v1 objek material lighting animasi"
git tag scene-v1
git push origin main --tags
```
Jika branch utama bernama `master`, ganti `main` menjadi `master`.
