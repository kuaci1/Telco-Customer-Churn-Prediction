# 📉 Telco Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Pandas%20|%20ScikitLearn%20|%20Seaborn-green)
![Status](https://img.shields.io/badge/Status-Completed-orange)

## 📌 Project Overview
Proyek ini bertujuan untuk memprediksi perilaku **Customer Churn** (pelanggan yang berhenti berlangganan) pada industri telekomunikasi. Menggunakan dataset dari Kaggle, analisis ini tidak hanya membangun model Machine Learning, tetapi juga memberikan **Business Insights** yang dapat ditindaklanjuti untuk menurunkan tingkat churn.

## 💼 Business Understanding
* **Masalah:** Tingkat Churn saat ini berada di angka **26.6%**, yang mengindikasikan potensi kehilangan pendapatan (*revenue leakage*) yang signifikan.
* **Tujuan:** Mengidentifikasi pola pelanggan yang berisiko tinggi untuk pindah dan memberikan rekomendasi strategi retensi yang tepat sasaran.
* **Dampak:** Mempertahankan pelanggan jauh lebih murah (5-25x) dibandingkan mengakuisisi pelanggan baru.

## 🛠️ Tech Stack
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Logistic Regression, Random Forest)
* **Data Preprocessing:** One-Hot Encoding, StandardScaler, SMOTE (Optional)

## 📊 Key Insights (EDA)
Berdasarkan Exploratory Data Analysis, kami menemukan profil pelanggan "High Risk":
1.  **Layanan Internet:** Pengguna **Fiber Optic** memiliki tingkat churn tertinggi (kemungkinan karena masalah harga/kualitas).
2.  **Kontrak:** Pengguna dengan kontrak **Month-to-month** sangat rentan berpindah dibandingkan kontrak tahunan.
3.  **Pembayaran:** Metode **Electronic Check** memiliki korelasi kuat dengan keputusan churn.

## 🤖 Model Performance
Model terbaik menggunakan algoritma **Random Forest** dengan hasil evaluasi sebagai berikut:
* **Accuracy:** ~79-80%
* **Top 3 Features:**
    1.  `TotalCharges` (Sensitivitas Harga)
    2.  `MonthlyCharges` (Beban Bulanan)
    3.  `tenure` (Loyalitas/Durasi Langganan)

## 💡 Business Recommendations
Strategi untuk mengurangi Churn berdasarkan data:
1.  **Fokus pada "Golden Window":** Berikan perhatian khusus pada pelanggan baru (0-6 bulan pertama) karena mereka paling rentan.
2.  **Konversi Kontrak:** Tawarkan insentif diskon bagi pelanggan bulanan untuk beralih ke kontrak 1 atau 2 tahun.
3.  **Edukasi Pembayaran:** Dorong penggunaan *Auto-pay* (Kartu Kredit/Transfer Otomatis) untuk mengurangi "pain of paying" setiap bulan.

---
**Author:** [Nama Anda]
**Dataset:** [Telco Customer Churn on Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn)
