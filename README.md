<img width="1584" height="785" alt="image" src="https://github.com/user-attachments/assets/4450483a-c861-47a1-92f0-f29d1e25015f" />## Bahari Analytics Portfolio

Proyek ini mendemonstrasikan kapabilitas analisis data end-to-end dari sistem My Horeca (VB6) ke Cloud Ecosystem.

# Bahari Analytics Portfolio 🚀

Proyek ini mendemonstrasikan kapabilitas analisis data end-to-end, mulai dari ekstraksi sistem legacy, migrasi arsitektur ke Cloud Ecosystem (Supabase/PostgreSQL), hingga visualisasi analitik tingkat lanjut untuk kebutuhan eksekutif.

---

## 🛠️ Tech Stack & Arsitektur Sistem
* **Core Database:** Cloud Supabase (PostgreSQL Engine)
* **Data Processing & Analytics:** Python (Pandas, SQLAlchemy)
* **Data Visualization Engine:** Seaborn, Matplotlib, & Google Looker Studio
* **Development Environment:** Google Colab Sandbox Integration

---

## 📂 Dokumentasi Proyek & Komponen Utama

### 1. Data Visualisasi & Jupyter Notebook (`Interactive`)
Analisis kontribusi pendapatan berdasarkan metode pembayaran yang diproses secara dinamis menggunakan Python. Notebook ini dilengkapi dengan fitur arsitektur hibrida (*local fallback system*) untuk menjaga integritas eksekusi dalam lingkungan sandbox.

* **Buka Script Interaktif:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/silayoga/bahari-analytics-portfolio/blob/main/New_Bahari_Analitycs.ipynb)
* **File Mentah:** [Lihat Notebook di Sini](New_Bahari_Analitycs.ipynb)

### 2. Business Intelligence Dashboard (`Executive Report`)
Dashboard interaktif yang dirancang untuk kebutuhan manajemen puncak (*C-Level Executive*) guna memantau metrik performa sales, tren transaksi, dan distribusi pembayaran secara real-time.

* **Tautan Dashboard:** [Buka Google Looker Studio Report](https://lookerstudio.google.com/reporting/UBAH_DENGAN_ID_LAPORAN_BAPAK) *(Pastikan hak akses tautan sudah diatur ke Public/Anyone with link can view)*

---

## 📈 Fitur Analisis Utama dalam Proyek
1. **Automated Data Formatting:** Konversi otomatis nilai angka sales mentah ke format representasi mata uang finansial yang bersih (Format Rupiah Terbaca).
2. **Hybrid Connectivity System:** Penanganan error tingkat jaringan (*network unreachable*) menggunakan metode repositori sandbox lokal agar alur analitik bisnis tidak terputus.
3. **Data Aggregation:** Pengelompokan data transaksi transaksional secara granular berdasarkan jenis pembayaran (Cash, Debit Card, Credit Card, dll).

---
*Maintained by Kadek Ngurah Silayoga — Senior IT Specialist & Management*
