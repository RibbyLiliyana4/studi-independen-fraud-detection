 Transaksi Keuangan Berbasis Pembelajaran Mesin Lanjut dan Rekayasa Fitur Matematika Keuangan.
# 🚀 Financial Fraud Detection & Transaction Intelligence System

<div align="center">

[![Status: Coming Soon](https://img.shields.io/badge/Status-Coming%20Soon-orange?style=for-the-badge&logo=github)](https://github.com/)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100%2B-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</div>

> **Purwarupa Sistem Intelijen Transaksi Finansial** berbasis *Machine Learning* tingkat lanjut, rekayasa fitur matematika keuangan, evaluasi sensitif biaya (*cost-sensitive evaluation*), serta dilengkapi dengan *Explainable AI* (SHAP) dan modul pelindungan data pribadi[span_3](start_span)[span_3](end_span)[span_4](start_span)[span_4](end_span).

---

## 📌 Tentang Proyek
Proyek akhir ini dikembangkan sebagai bagian dari program Studi Independen Bersertifikat bersama **PT Vinix Seven Aurum (VINIX7)** pada divisi *Python Data Science Engineer*[span_5](start_span)[span_5](end_span). Sistem ini dirancang untuk mendeteksi anomali penipuan transaksi keuangan (seperti *account takeover* dan pengurasan saldo) pada dataset simulasi transaksi skala besar (**PaySim**) serta divalidasi dengan dataset eksternal[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span)[span_8](start_span)[span_8](end_span).

Berbeda dari sistem deteksi konvensional yang hanya berfokus pada akurasi metrik atau aturan statis (*rule-based*), sistem ini menguji performa model secara empiris melalui pendekatan berbasis biaya bisnis (*expected loss*), serta menjaga akuntabilitas keputusan melalui transparansi model[span_9](start_span)[span_9](end_span)[span_10](start_span)[span_10](end_span)[span_11](start_span)[span_11](end_span).

---

## 🛠️ Arsitektur & Fitur Utama (Coming Soon)

*   🔒 **Lapisan Etika & Pelindungan Data**: Implementasi pseudonimisasi dan *masking* atribut identitas mengacu pada **Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi (UU PDP)**[span_12](start_span)[span_12](end_span).
*   📊 **Rekayasa Fitur Matematika Keuangan**: 
    *   *Error Balance* (deviasi buku besar pengirim/penerima)[span_13](start_span)[span_13](end_span).
    *   Rasio pengurasan saldo (*balance drainage ratio*)[span_14](start_span)[span_14](end_span).
    *   Kecepatan perputaran dana (*velocity*) pada rekening tujuan[span_15](start_span)[span_15](end_span).
    *   Indikator penyimpangan distribusi digit pertama (*Benford's Law*)[span_16](start_span)[span_16](end_span).
*   ⚖️ **Perbandingan 4 Skema Eksperimen**:
    *   **Eksperimen A:** Baseline *Rule-Based* (Sistem ambang *IF-THEN* industri)[span_17](start_span)[span_17](end_span).
    *   **Eksperimen B:** XGBoost pada fitur mentah (*raw features*) dengan *SMOTE* vs *Class Weighting*[span_18](start_span)[span_18](end_span).
    *   **Eksperimen C:** XGBoost pada fitur rekayasa matematika keuangan[span_19](start_span)[span_19](end_span)[span_20](start_span)[span_20](end_span).
    *   **Eksperimen D:** *Autoencoder* untuk deteksi anomali tak terawasi (*unsupervised anomaly detection*)[span_21](start_span)[span_21](end_span).
*   💰 **Evaluasi Sensitif Biaya (*Cost-Sensitive Evaluation*)**: Optimasi ambang batas keputusan (*decision threshold*) berbasis kerangka *Expected Loss* untuk meminimalkan kerugian bersih[span_22](start_span)[span_22](end_span)[span_23](start_span)[span_23](end_span).
*   🔍 **Explainable AI (XAI)**: Integrasi **SHAP** untuk menyajikan atribusi kontribusi fitur pada setiap transaksi yang ditandai sebagai dasar akuntabilitas keputusan[span_24](start_span)[span_24](end_span)[span_25](start_span)[span_25](end_span).
*   🚀 **Deployment & Dasbor**: 
    *   **REST API** backend menggunakan `FastAPI` lengkap dengan dokumentasi `Swagger`[span_26](start_span)[span_26](end_span).
    *   **Interactive Dashboard** menggunakan `Streamlit` untuk pemantauan aliran transaksi secara real-time dan simulatif[span_27](start_span)[span_27](end_span).

---

## 📂 Struktur Repositori (Rencana)

```text
financial-fraud-detection/
│
├── data/                  # Direktori data (PaySim & dataset eksternal)
├── notebooks/             # Jupyter Notebook untuk EDA & Eksperimen A-D
├── src/                   # Source code pipeline, feature engineering, & model
├── api/                   # Layanan REST API berbasis FastAPI
├── dashboard/             # Antarmuka dasbor pemantauan Streamlit
├── reports/               # Laporan teknikal & dokumentasi eksperimen
├── requirements.txt       # Daftar pustaka Python
└── README.md              # Dokumentasi proyek

📅 Roadmap & Linimasa Pengembangan
 * [x] Minggu 1-2: Akuisisi data, eksplorasi SQL lanjutan, dan pembersihan data skala besar (PaySim).
 * [x] Minggu 3-4: Analisis statistik, uji hukum Benford, EDA, dan perancangan lapisan etika data.
 * [ ] Minggu 5-6: Rekayasa fitur matematika keuangan, pembangunan baseline rule-based, dan pelatihan XGBoost (Eksperimen A, B, & C).
 * [ ] Minggu 7-8: Implementasi model unsupervised (Autoencoder) & evaluasi sensitif biaya.
 * [ ] Minggu 9-11: Integrasi XAI (SHAP), pembangunan REST API FastAPI, dasbor Streamlit, serta finalisasi laporan akhir.
👥 Tim Pengembang
 * Ribby Liliyana Susan (24031554041) - S1 Sains Data, Universitas Negeri Surabaya
 * Mitra Industri: PT Vinix Seven Aurum (VINIX7) – Divisi Python Data Science Engineer
 * Dosen Pembimbing Lapangan: Dr. Atik Wintarti, M.Kom.
<div align="center">
<p><i>Project in active development as part of Independent Study Program 2026. Stay tuned for updates!</i> 🚀</p>
</div>

