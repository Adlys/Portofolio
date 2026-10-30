# 🎓 Auto-OCR for Student Tuition Payment Slips
### Pengolahan Citra Digital untuk Otomatisasi Data Keuangan Mahasiswa

**Background:** Selama 8 tahun sebagai Kepala Bidang Data Keuangan Mahasiswa (15.000 mahasiswa), saya menemukan proses input slip pembayaran manual memakan 40 jam kerja/bulan dan error rate 12%.

**Solution:** Sistem OCR otomatis menggunakan Image Processing untuk membaca slip pembayaran kuliah.

**Tech Stack:**
- Python, OpenCV, Tesseract OCR
- YOLOv8 untuk deteksi area slip
- Image Preprocessing: Grayscale, Adaptive Threshold, Perspective Correction
- MySQL untuk integrasi dengan Sistem Keuangan Mahasiswa

**Workflow:**
1. Input: Foto slip pembayaran (HP / Scan)
2. Preprocessing: Deteksi tepi slip -> Luruskan (Perspective Transform) -> Bersihkan noise
3. OCR: Baca NIM, Nama, Nominal, Tanggal Bayar
4. Validasi: Cocokkan dengan database mahasiswa
5. Output: Otomatis update status bayar di database

**Result:**
- Akurasi OCR: 94.5% (uji 200 slip)
- Waktu proses: 3 detik / slip (vs 2 menit manual)
- Menghemat 38 jam kerja / bulan

**Future Improvement:** Integrasi dengan FinTech API untuk verifikasi pembayaran real-time.

Author: [Namamu] | S2 Teknik Informatika - Image Processing | 8 Years Head of Student Finance Data
