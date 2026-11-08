# Tetris Console (Windows)

Game Tetris berbasis teks (console) yang ditulis dengan C++. Dilengkapi sistem slot simpanan, leaderboard, pencarian pemain, dan hapus save.

> **Catatan:** Hanya berjalan di **Windows**, karena memakai `conio.h` dan `windows.h`.

## Fitur
- Permainan Tetris di terminal
- Simpan & muat game lewat slot (default 10 slot)
- Leaderboard skor tertinggi
- Cari data pemain berdasarkan nama
- Hapus data simpanan

## Kontrol
| Tombol | Aksi |
|--------|------|
| `A` | Geser kiri |
| `D` | Geser kanan |
| `W` | Putar blok |
| `S` | Turun |
| `Q` | Keluar & simpan |

## Cara Kompilasi
Butuh compiler C++ untuk Windows (misalnya [MinGW-w64](https://www.mingw-w64.org/) atau MSVC).

**Dengan g++:**
```bash
g++ -std=c++11 -O2 tetris.cpp -o tetris.exe
```

**Atau dengan make:**
```bash
make
```

**Dengan MSVC (Developer Command Prompt):**
```bash
cl /EHsc /std:c++14 tetris.cpp
```

Lalu jalankan:
```bash
tetris.exe
```

## Konfigurasi
Jumlah slot simpanan dapat diubah di `tetris.cpp`:
```cpp
const int JUMLAH_SLOT = 10; // ubah ke 100 jika perlu
```

## Lisensi
MIT — lihat file [LICENSE](LICENSE).
