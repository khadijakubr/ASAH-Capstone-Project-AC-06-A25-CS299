# Customer Segmentation — AC-06 Capstone Project (A25-CS299)

Repository ini berisi **notebook analisis dan eksperimen untuk customer segmentation** pada use case AC-06. Proyek ini dibuat sebagai bagian dari capstone project kelompok **A25-CS299**, dengan fokus melakukan segmentasi pelanggan menggunakan pendekatan **RFM** dan **clustering** (K-Means).

Tujuan utama repository ini adalah sebagai dokumentasi proses analisis, modelling, interpretasi cluster, serta rekomendasi strategi pemasaran berbasis data.

---

## 🎯 Latar Belakang Masalah

Perusahaan ritel online sering kali menjalankan kampanye promosi yang sama untuk seluruh pelanggan tanpa melihat perilaku pembelian yang berbeda-beda. Dampaknya:

- Banyak promosi yang tidak efektif  
- Biaya pemasaran meningkat  
- Tingkat keterlibatan (engagement) pelanggan rendah  

Dengan memanfaatkan data transaksi, perusahaan dapat membangun **segmentasi pelanggan** berdasarkan perilaku dan nilai belanja. Segmentasi ini memungkinkan perusahaan untuk:

- Menargetkan pelanggan dengan promosi yang lebih personal  
- Menggunakan anggaran pemasaran lebih efisien  
- Meningkatkan retensi dan loyalitas pelanggan  

---

## 📌 Ruang Lingkup Proyek

1. Melakukan analisis data transaksi pelanggan dari **Online Retail Dataset (UCI)**.
2. Membangun model **RFM (Recency, Frequency, Monetary)**.
3. Menerapkan beberapa variasi kombinasi RFM seperti:
   - `RFM (Recency, Frequency, Monetary)`
   - `RFM (Recency, Frequency, AvgPurchase)`
   - `RFM (Recency, Frequency, CLV)`
4. Melakukan segmentasi pelanggan menggunakan **K-Means clustering** dan mengevaluasi cluster dengan:
   - Elbow Method  
   - Silhouette Score  
5. Menghasilkan label segmen pelanggan seperti:
   - **Champions / VIP**
   - **Loyal Customers**
   - **Big Spenders / Whales**
   - **New Customers**
   - **Hibernating / At Risk**

---

## 📂 Isi Notebook

Notebook utama berisi:

- **Data preprocessing & EDA**
  - Handling missing values
  - Filtering transaksi tidak valid
  - Feature engineering (`TotalValue`, `AvgPurchase`, `CLV`)
- **Pembangunan nilai RFM**
- **Scaling dan clustering**
- **Visualisasi cluster dengan pairplot**
- **Interpretasi cluster lengkap**
- **Rekomendasi pemasaran per segment**

Setiap variasi RFM divisualisasikan dan dianalisis untuk menemukan segmentasi paling informatif.

---

## 🧠 Metodologi Utama

### 1. RFM Analysis
- **Recency**: Seberapa baru pelanggan melakukan pembelian  
- **Frequency**: Seberapa sering mereka bertransaksi  
- **Monetary**: Total nilai belanja pelanggan  

Tambahan fitur:
- `AvgPurchase` = `Monetary / Frequency`  
- `CLV` = `Frequency × AvgPurchase`

### 2. Clustering dengan K-Means
- Menentukan jumlah cluster menggunakan **Elbow Method**  
- Validasi cluster menggunakan **Silhouette Score**  
- Visualisasi cluster untuk interpretasi bisnis  

### 3. Segmentasi Pelanggan
Setiap cluster diberi label persona berdasarkan pola perilaku pelanggan, misalnya: *Champions*, *Loyalists*, *Potential Loyalists*, *Hibernating*, *Lost*, dll.

---

## 👥 Tim Pengembang (A25-CS299)

| NIM | Nama | Track | Status |
|-----|-----------------------------|----------------|---------|
| **M452D5Y0431** | Danu Sisda Rafiyandi | Machine Learning | Aktif |
| **M197D5X0961** | Khadijatul Kubro | Machine Learning | Aktif |
| **M180D5Y1360** | Muhammad Razzan Ramadhana | Machine Learning | Aktif |

---

## 📎 Dataset

Dataset yang digunakan:

- **Online Retail Dataset (UCI Machine Learning Repository)**  
- Versi yang digunakan tersedia di Kaggle dengan nama *Online Retail Dataset*

---

## 🚀 Tujuan Akhir

- Menghasilkan **model segmentasi pelanggan** yang membantu perusahaan memahami perilaku pelanggan
- Memberikan dasar strategi pemasaran yang **lebih personal, efisien, dan berbasis data**
- Menjadi referensi bagi pengembangan sistem rekomendasi atau CRM di masa depan

---
