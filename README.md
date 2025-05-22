# 📊 LATIHAN 3 – Portofolio Excel: VLOOKUP dan IF

Latihan ini merupakan bagian dari portofolio saya dalam mempelajari analisis data menggunakan Microsoft Excel. Fokus utama adalah penggunaan rumus `VLOOKUP` dan `IF` untuk mengolah data akademik berdasarkan dua tabel referensi, yaitu data mata kuliah dan data dosen.

---

## 🎯 Tujuan Proyek
- Mengambil informasi otomatis dari daftar referensi menggunakan `VLOOKUP`.
- Menganalisis beban SKS dosen dan memberikan status "OK" atau "OVER".
- Mengembangkan keterampilan mengelola data tabular dalam Excel.

---

## 📁 Dataset
- **LIST_MK**: berisi ID Mata Kuliah, Nama MK, SKS, Semester, dan Sifat.
- **LIST_DOSEN**: berisi ID Dosen, Nama Dosen, dan Umur.
- **LATIHAN 3**: tempat simulasi pengolahan data berdasarkan input ID MK dan ID Dosen.

---

## 🛠️ Tools & Rumus Excel

### Fungsi `VLOOKUP`:
Mengambil data dari tabel referensi:

```excel
=VLOOKUP(A2; 'LIST MK'!$A$2:$F$100; 2; 0)   // Nama MK
=VLOOKUP(A2; 'LIST MK'!$A$2:$F$100; 3; 0)   // SKS
=VLOOKUP(A2; 'LIST MK'!$A$2:$F$100; 4; 0)   // Semester
=VLOOKUP(A2; 'LIST MK'!$A$2:$F$100; 5; 0)   // Sifat
=VLOOKUP(F2; 'LIST DOSEN'!$A$2:$C$100; 2; 0) // Nama Dosen
=VLOOKUP(F2; 'LIST DOSEN'!$A$2:$C$100; 3; 0) // Umur Dosen

