# 🎂 Birthday Quest — untuk Ataya Ranissa Haruna Putri

Ucapan ulang tahun berbentuk mini-game retro. Satu file HTML, tanpa library,
tanpa internet — tinggal buka `index.html` di browser (paling enak dibuka di HP).

## Alur gamenya

| Stage | Main apa | Yang kebuka |
|---|---|---|
| **0** | Title screen, tekan **START** | — |
| **1 — Nyalain Lilin** | Tap 5 lilin di kue sampai nyala | **"SELAMAT ULANG TAHUN BUY!!"** + Memory #1 |
| **2 — Tangkep Doa** | Geser karakter buat nangkep 8 bintang | Doa panjangnya ("Panjang umur, sehat selalu…") + Memory #2 |
| **3 — Hype Boss** | Mash tombol sampai HYPE 100% | Layar goyang + slam **"BOCIL ULANG TAHUN WOYYYYYY"** + Memory #3 |
| **4 — Buka Kado** | Tap kado 3x sampai kebuka | Pesan soal hadiah ("Maafin aku ya…") + Memory #4 |
| **5 — Sebarin Bahagia** | Tap di mana aja sampai semua orang happy | "Semoga di hari ulang tahun dedek…" + Memory #5 |
| **Ending** | — | **"I LOVE YOU SO MUCH BUY"** + album polaroid semua foto |

Tiap stage kelar, satu foto kenangan kebuka sebagai hadiah (kotak kecil di HUD
kanan atas = progress memory).

## Masukin fotonya

Dua cara, bebas pilih:

1. **Taruh file** — masukkan 5 foto ke folder `photos/` dengan nama `foto1.jpg`
   sampai `foto5.jpg`. Detail urutan + caption ada di [`photos/README.md`](photos/README.md).
2. **Pilih dari HP** — buka gamenya, tekan **📷** di pojok kanan atas, tap tiap
   kotak buat ambil foto dari galeri. Tersimpan di browser HP itu saja.

Game tetap jalan normal walau fotonya belum diisi — slot yang kosong cuma jadi
polaroid kosong yang ngasih tau cara ngisinya.

## Kontrol

- **Sentuh / klik** untuk semuanya
- **Spasi / Enter** — lanjut dialog, dan mash di Stage 3
- **← →** — geser karakter di Stage 2
- **🔊** — matiin/nyalain musik (ada melodi Happy Birthday chiptune di latar)
- Tap teks yang lagi ngetik = langsung tampil penuh

## Cara buka

Dobel klik `index.html`. Atau kalau mau lewat server lokal:

```bash
npx http-server . -p 8080   # lalu buka http://localhost:8080
```

Semua efek (sprite pixel-art, confetti, chiptune) digambar/dibangkitkan langsung
di dalam file — nggak ada aset eksternal selain foto kamu sendiri.
