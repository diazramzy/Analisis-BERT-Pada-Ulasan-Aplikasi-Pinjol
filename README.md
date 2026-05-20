# Analisis Aspek dan Emosi Ulasan Aplikasi Pinjaman Online di Indonesia Menggunakan IndoBERT

Proyek penelitian ini mengimplementasikan framework klasifikasi *multiclass* dua tahap untuk menganalisis ulasan pengguna aplikasi pinjaman online (pinjol) di Indonesia. Dengan menggunakan model **IndoBERT**, proyek ini mengidentifikasi aspek layanan spesifik dan respon emosional pengguna dari 15.751 ulasan Google Play Store.

## 📌 Ringkasan Proyek
Penelitian ini melampaui analisis sentimen tradisional (positif/negatif) dengan memetakan hubungan antara masalah layanan dengan emosi pengguna. 

**Tahap Klasifikasi:**
1.  **Service Aspects**: Debt Collection, High Interest/Fees, Privacy, dan Accessibility.
2.  **Emotional Traits**: Anger, Disappointed, Joy, dan Fear.

## 🛠️ Alatan & Teknologi (Tools)
* **Bahasa Pemrograman**: Python
* **Model Bahasa**: IndoBERT (Bidirectional Encoder Representations from Transformers untuk Bahasa Indonesia)
* **Environment**: Google Colab / Jupyter Notebook
* **Library Utama**:
    * `transformers` (Hugging Face) - Untuk fine-tuning model IndoBERT.
    * `scikit-learn` - Untuk evaluasi metrik (F1-Score, Confusion Matrix).
    * `pandas` & `numpy` - Pengolahan data 15.751 ulasan.
    * `matplotlib` & `seaborn` - Visualisasi pola aspek-emosi.

## 📊 Hasil Penelitian & Metrik
Berdasarkan hasil eksperimen dan fine-tuning hyperparameter, framework ini mencapai:
* **Macro F1-Score**: **0.82** untuk kedua tahap (Aspek dan Emosi).
* **Performa Tertinggi**: Klasifikasi pada aspek *Privacy* dan *Accessibility* menunjukkan hasil yang paling kuat.
* **Tantangan**: Aspek *High Interest/Fees* dan emosi *Disappointed* memiliki tumpang tindih semantik yang tinggi, memberikan tantangan tersendiri dalam klasifikasi teks yang halus.

## 📁 Struktur Data
Dataset terdiri dari ulasan yang dianotasi secara manual ke dalam:
* **4 Aspek Layanan**: Penagihan hutang, bunga tinggi, privasi, dan aksesibilitas.
* **4 Kategori Emosi**: Marah, Kecewa, Senang, dan Takut.

## 💡 Implikasi Praktis
Hasil dari proyek ini memberikan wawasan terstruktur bagi regulator dan pengembang platform untuk:
1.  Mengidentifikasi praktik penagihan yang berbahaya secara otomatis.
2.  Memantau pelanggaran privasi berdasarkan laporan pengguna.
3.  Meningkatkan kualitas layanan berdasarkan titik emosional pengguna.

---
**Diaz Ramzy Naufal**
*Informatika - Universitas Telkom*
