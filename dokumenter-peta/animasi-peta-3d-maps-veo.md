# Animasi Peta 3D dari Google Maps (Gemini + Veo 3)

Sumber: @buildfastwithai, Instagram (2026-04-22) — https://www.instagram.com/reel/DXbv7HACMT4/
Status: alur kerja + templat (teks prompt asli kreator dikunci di balik komentar).

## Alur kerja (3 langkah)
1. **Google Maps** — cari landmark, ambil tangkapan layar petanya.
2. **Gemini (gambar)** — unggah tangkapan layar, hasilkan 2 gambar:
   - Gambar A (frame awal): peta + tangan menancapkan pin merah (pushpin) di lokasi.
   - Gambar B (frame akhir): gabungan peta + foto asli landmark menjadi model 3D landmark di atas peta.
3. **Veo 3** — unggah Gambar A sebagai frame awal dan Gambar B sebagai frame akhir, pakai prompt video di bawah → animasi ±8 detik: peta "robek terbuka" dan landmark muncul 3D.

## Templat prompt gambar (Gemini)
```
Photorealistic top-down view of a printed map of [NAMA TEMPAT], a human hand placing a large red pushpin exactly on [LANDMARK], soft daylight, shallow depth of field, ultra detailed, 16:9
```
```
Combine this map screenshot with the photo of [LANDMARK]: a detailed 3D miniature model of [LANDMARK] rising from the map surface at the pinned location, photorealistic, cinematic lighting, 16:9
```

## Templat prompt video (Veo 3)
```
Seamless cinematic animation: the map surface tears open at the pushpin and a 3D model of [LANDMARK] rises and assembles in place, camera slowly pushing in, dust and paper particles, photorealistic, smooth motion, 8 seconds
```
