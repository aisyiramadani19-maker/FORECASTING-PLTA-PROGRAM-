# FORECASTING-PLTA-PROGRAM-
Program Forecasting PLTA Proyek
==================================================
README
PROGRAM FORECASTING POTENSI PLTA
==================================================

Nama Program   : Aplikasi Forecasting Potensi PLTA
Bahasa         : Python
Framework      : Streamlit
Mata Kuliah    : Algoritma Data dan Pemrograman
Topik          : Energi Terbarukan (PLTA)

--------------------------------------------------
1. DESKRIPSI PROGRAM
--------------------------------------------------

Program ini merupakan aplikasi berbasis Python yang digunakan
untuk melakukan forecasting potensi Pembangkit Listrik Tenaga Air (PLTA)
dengan mempertimbangkan faktor iklim, yaitu curah hujan, suhu,
dan kelembaban udara.

Aplikasi ini dibuat dalam bentuk web app menggunakan Streamlit
sehingga pengguna dapat berinteraksi langsung melalui browser
untuk memasukkan data dan melihat hasil analisis.

--------------------------------------------------
2. STRUKTUR FILE PROGRAM
--------------------------------------------------

Struktur folder program adalah sebagai berikut:

- streamlit_plta/
  - app.py
  - README.txt

Keterangan:
- app.py     : File utama program forecasting PLTA
- README.txt : Dokumen penjelasan program

--------------------------------------------------
3. PERSIAPAN SEBELUM MENJALANKAN PROGRAM
--------------------------------------------------

Sebelum menjalankan program, pastikan hal-hal berikut:

1. Python sudah terinstal di komputer
   (disarankan Python versi 3.8 atau lebih baru)

2. Streamlit dan library pendukung telah terinstal

Library yang digunakan:
- streamlit
- numpy
- pandas
- matplotlib

--------------------------------------------------
4. INSTALASI LIBRARY
--------------------------------------------------

Langkah instalasi library dilakukan melalui Command Prompt
atau Anaconda Prompt.

1. Buka Command Prompt / Anaconda Prompt
2. Ketik perintah berikut:

   pip install streamlit numpy pandas matplotlib

3. Tunggu hingga proses instalasi selesai

--------------------------------------------------
5. LANGKAH MENJALANKAN PROGRAM (STEP-BY-STEP)
--------------------------------------------------

Langkah-langkah menjalankan program adalah sebagai berikut:

1. Buka Command Prompt atau Anaconda Prompt

2. Masuk ke folder tempat file app.py berada.
   Contoh:
   cd C:\Users\NamaUser\Documents\streamlit_plta

3. Setelah berada di folder yang benar,
   jalankan perintah berikut:

   streamlit run app.py

4. Tunggu beberapa saat hingga Streamlit berjalan.

5. Browser akan terbuka secara otomatis
   (biasanya di alamat http://localhost:8501)

6. Jika browser tidak terbuka otomatis,
   salin alamat yang muncul di terminal
   lalu buka secara manual melalui browser.

--------------------------------------------------
6. CARA MENGGUNAKAN APLIKASI
--------------------------------------------------

Setelah aplikasi terbuka di browser:

1. Masukkan nama sungai pada kolom "Nama Sungai"
2. Masukkan debit rata-rata sungai (m3/s)
3. Masukkan nilai head / tinggi jatuh air (m)
4. Pilih bulan yang ingin dianalisis
5. Masukkan data faktor iklim untuk setiap bulan:
   - Curah hujan (mm)
   - Suhu udara (°C)
   - Kelembaban (%)
6. Klik tombol "Jalankan Forecast"

--------------------------------------------------
7. OUTPUT PROGRAM
--------------------------------------------------

Setelah tombol "Jalankan Forecast" ditekan,
program akan menampilkan:

- Tabel hasil forecasting debit sungai
- Tabel hasil forecasting daya PLTA
- Grafik batang debit sungai per bulan
- Grafik batang daya PLTA per bulan
- Informasi status kelayakan PLTA
  (PLTA Mikro / PLTA Mini)

--------------------------------------------------
8. KELAYAKAN PLTA
--------------------------------------------------

Kelayakan PLTA ditentukan berdasarkan debit rata-rata
hasil forecasting sebagai berikut:

- Debit ≥ 5 m3/s   → Sangat Layak (PLTA Mini)
- 1 ≤ Debit < 5    → Layak (PLTA Mikro)
- Debit < 1 m3/s   → Kurang Layak

--------------------------------------------------
9. KESIMPULAN
--------------------------------------------------

Program ini dapat digunakan sebagai alat bantu analisis awal
untuk mengetahui potensi sungai sebagai sumber energi listrik
tenaga air. Dengan adanya input faktor iklim, hasil forecasting
yang diperoleh lebih realistis dan dapat digunakan sebagai
referensi awal perencanaan PLTA.

==================================================
