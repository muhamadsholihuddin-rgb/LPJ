# Form Laporan Penggunaan Dana PPSE

Situs statis (HTML + jsPDF dari CDN) untuk membuat PDF Laporan Penggunaan Dana Bantuan Sosial PPSE.
Semua proses terjadi di browser; data dan foto tidak dikirim ke server.

## Deploy ke Vercel
1. Buat repository GitHub baru, upload `index.html` dan `README.md` (di root repo).
2. Di vercel.com: **Add New → Project** → pilih repository tersebut.
3. Framework Preset: **Other**. Kosongkan Build Command dan Output Directory. Klik **Deploy**.

## Halaman
- `index.html` = laporan lengkap: unggah scan halaman 1–3 yang sudah bertanda tangan basah, isi RAB dan foto, lalu digabung jadi satu PDF.
- `surat.html` = pembuat halaman 1–3 (surat laporan, daftar lampiran, surat pernyataan) untuk dicetak dan ditandatangani.

## Catatan
- Data pendamping, kota, dan tahun disimpan di localStorage browser agar tidak perlu diisi ulang.
- Membutuhkan koneksi internet untuk memuat jsPDF dan pdf.js dari cdnjs.cloudflare.com.
- Unggah proposal PDF (format "Profil Penerima Manfaat PPSE") akan mengisi nama, NIK, telepon, alamat, nominal, dan RAB otomatis.
