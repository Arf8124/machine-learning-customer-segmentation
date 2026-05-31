## 📌 Project Overview
**Customer Personality Analysis** adalah analisis mendalam terhadap pelanggan ideal sebuah perusahaan. Proyek ini bertujuan untuk membantu bisnis memahami pelanggan mereka dengan lebih baik, sehingga memudahkan tim pemasaran (marketing) untuk memodifikasi produk atau merancang strategi kampanye yang tepat sasaran berdasarkan kebutuhan, perilaku, dan profil segmen pelanggan tertentu.

Daripada menghabiskan anggaran pemasaran untuk mengiklankan produk baru ke seluruh basis pelanggan, perusahaan dapat menganalisis segmen mana yang paling mungkin membeli produk tersebut dan memfokuskan strategi pemasaran hanya pada segmen tersebut.

## 📊 Dataset & Features
Dataset yang digunakan dalam proyek ini mencakup informasi perilaku dan demografi pelanggan, yang meliputi:
*   **People:** Umur, tingkat pendidikan, status pernikahan, pendapatan rumah tangga, jumlah anak, dan tanggal bergabung sebagai pelanggan.
*   **Products:** Jumlah pengeluaran untuk berbagai kategori produk (Anggur, Buah-buahan, Daging, Ikan, Manisan, dan Emas).
*   **Promotion:** Jumlah pembelian yang dilakukan menggunakan diskon/promo dan respons terhadap kampanye pemasaran sebelumnya.
*   **Place:** Jumlah pembelian yang dilakukan melalui berbagai saluran (Web, Katalog, Toko Fisik, dan jumlah kunjungan ke Web perusahaan).

## 🛠️ Workflow & Methodology
Proyek ini diselesaikan melalui beberapa tahapan utama menggunakan *Machine Learning pipeline*:

1.  **Data Preprocessing & Cleaning:**
    *   Penanganan *missing values* dan *outliers*.
    *   *Feature Engineering* (pembuatan fitur baru seperti total pengeluaran, usia pelanggan, total anak, dll).
    *   Skalasi data menggunakan `StandardScaler` untuk menyamakan rentang nilai antar fitur.
2.  **Dimensionality Reduction (PCA):**
    *   Menggunakan **Principal Component Analysis (PCA)** untuk mereduksi dimensi data yang kompleks dan meminimalkan redundansi multikolinieritas, tanpa kehilangan informasi penting.
3.  **Clustering (K-Means):**
    *   Menentukan jumlah kluster optimal menggunakan *Elbow Method*.
    *   Menerapkan algoritma **K-Means Clustering** untuk mengelompokkan pelanggan ke dalam beberapa segmen kepribadian yang berbeda.
4.  **Evaluation & Profiling:**
    *   Visualisasi hasil kluster menggunakan diagram 2D/3D dari komponen PCA.
    *   Analisis karakteristik profil dari setiap kelompok pelanggan untuk ditarik kesimpulan bisnis (*business insights*).

## 🚀 Technologies Used
*   **Language:** Python
*   **Libraries:** 
    *   Data Manipulation: `pandas`, `numpy`
    *   Data Visualization: `matplotlib`, `seaborn`, `plotly`
    *   Machine Learning: `scikit-learn` (PCA, KMeans, StandardScaler)
