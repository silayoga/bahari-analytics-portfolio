# Bahari Analytics Portfolio 🚀

Proyek ini mendemonstrasikan kapabilitas analisis data end-to-end, mulai dari ekstraksi sistem legacy (VB6), migrasi arsitektur ke Cloud Ecosystem (Supabase/PostgreSQL), hingga visualisasi analitik tingkat lanjut untuk kebutuhan eksekutif manajemen puncak (C-Level) dan IT Auditing.

---

## 🛠️ Tech Stack & Arsitektur Sistem
* **Core Database:** Cloud Supabase (PostgreSQL Engine)
* **Data Processing & Analytics:** Python (Pandas, NumPy, SQLAlchemy)
* **Data Visualization Engine:** Seaborn, Matplotlib, & Google Looker Studio
* **Development Environment:** Google Colab Sandbox Integration

---

## 📂 Dokumentasi Proyek & Komponen Utama

### 1. Data Visualisasi & Jupyter Notebook (`Interactive`)
Notebook ini dirancang menggunakan arsitektur hibrida (*local fallback system*) untuk memastikan integritas eksekusi sistem tetap berjalan optimal meskipun port cloud diblokir oleh infrastruktur sandbox lingkungan pengeksekusi:

* **Modul A: Distribusi Pendapatan Berdasarkan Metode Pembayaran**
  * *Penjelasan:* Analisis makro aliran kas masuk (*cash inflow*) berdasarkan instrumen pembayaran (Cash, Debit, Credit, Bon/Piutang, Compliment). Bermanfaat untuk memetakan likuiditas harian dan mengukur ketergantungan operasional pada uang tunai fisik vs non-tunai.
* **Modul B: Analisis Jam Operasional & Manajemen Risiko Arus Kas**
  * *Penjelasan:* Memetakan produktivitas penjualan berbasis jam transaksi (24-hour format) untuk mengidentifikasi fenomena *double-peak operational hours*. Dilengkapi dengan klasifikasi kesehatan dana (*Cash Flow Risk Composition*) guna memisahkan dana likuid seketika dengan risiko tertunda (piutang).
* **Modul C (Security & Audit): IT Audit Dashboard (Void Rate Anomaly)**
  * *Penjelasan:* Implementasi *Internal Fraud Control* berbasis statistik. Sistem menghitung rasio batalan nota (*Void Rate*) dinamis per operator kasir asli dari database untuk mendeteksi anomali perilaku yang melewati ambang batas aman (Threshold 2.0%).
* **Modul D (Executive Strategic): Analisis Departemen & Tren Musiman (Seasonality)**
  * *Penjelasan:* Visualisasi kontribusi omzet per departemen (F&B vs Room Rental) dikombinasikan dengan tren pertumbuhan penjualan bulanan (Month-over-Month Growth) untuk mendeteksi pola musiman (*peak & low seasons*).

* **Buka Script Interaktif:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/silayoga/bahari-analytics-portfolio/blob/main/New_Bahari_Analitycs.ipynb)
* **File Mentah:** [Lihat Notebook di Sini](New_Bahari_Analitycs.ipynb)

### 2. Business Intelligence Dashboard (`Executive Report`)
Dashboard interaktif yang dirancang untuk memantau metrik performa sales, tren transaksi harian, dan kesehatan kas secara real-time.
* **Tautan Dashboard:** [Buka Google Looker Studio Report](https://lookerstudio.google.com/reporting/UBAH_DENGAN_ID_LAPORAN_BAPAK)

---

## 📈 Bedah Logika & Key Business Insights

### A. Metodologi Deteksi Anomali Void (IT Security & Fraud Control)
Asumsi tersembunyi dalam operasional POS hospitality adalah setiap tindakan *Void* (pembatalan transaksi) merupakan kesalahan input manusia. Namun, secara kritis, tingginya angka pembatalan pada operator tertentu dapat mengindikasikan celah manipulasi kas (*pencurian terselubung setelah struk dicetak*).
* **Formula Kontrol:** $$\text{Void Rate (\%)} = \left( \frac{\text{Total Transaksi Void}}{\text{Total Transaksi Sukses}} \right) \times 100$$
* **Rekomendasi Struktur:** Operator dengan *Void Rate* > 2.0% (misalnya: `Ketut Kasir`) diprioritaskan untuk audit silang log sistem fisik (*CCTV vs POS Timestamp*) ketimbang sekadar *retraining*.

### B. Sinkronisasi Kapasitas vs Pola Musiman (Revenue Strategy)
Melalui analisis tren bulanan dan kontribusi kategori bisnis (didominasi oleh Food & Beverage), manajemen dapat mengambil keputusan taktis berbasis data (*Data-Driven Decision*):
* **Optimasi Operasional:** Struktur pendapatan menunjukkan *F&B* dan *Room Rental* sebagai *core engine* bisnis. Lonjakan pendapatan pada bulan-bulan *peak season* (seperti Desember) memerlukan kesiapan infrastruktur IT berupa optimasi query database agar tidak terjadi *bottle-neck* saat beban transaksi memuncak.
* **Manajemen Kas:** Kategori pembayaran non-tunai yang tinggi memangkas risiko *cash handling error*, namun porsi *Bon / Piutang* harus diawasi agar tidak mengganggu rasio likuiditas modal kerja harian.

* ### 📊 Executive Slide Decks (Interactive HTML)
* 🖥️ [Buka Presentasi Tokopaedi Case Study](https://htmlpreview.github.io/?https://github.com/silayoga/bahari-analytics-portfolio/blob/main/documentation/remade_tokopaedi_presentation.html)
* 🖥️ [Buka Presentasi Python Case Study — By Kadek Ngurah Silayoga](https://htmlpreview.github.io/?https://github.com/silayoga/bahari-analytics-portfolio/blob/main/documentation/Strategic Data Analytics Portfolio.html)

---
*Maintained by Kadek Ngurah Silayoga — Senior IT Specialist & IT Manager*
