# 🎓 Student Habits & Academic Performance Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **"Does watching Netflix all night actually ruin your grades?"**

Proyek Data Science ini bertujuan untuk menganalisis pengaruh kebiasaan sehari-hari (lifestyle), kesehatan mental, dan faktor demografis terhadap performa akademik mahasiswa. Proyek ini diakhiri dengan pembuatan **Sistem Prediksi Nilai** berbasis Machine Learning sederhana.

## 📋 Table of Contents
- [Overview](#-overview)
- [Dataset Features](#-dataset-features)
- [Tech Stack](#-tech-stack)
- [Project Workflow](#-project-workflow)
- [Key Insights](#-key-insights)
- [How to Run](#-how-to-run)

## 📖 Overview
Dalam era digital, mahasiswa dihadapkan pada banyak distraksi seperti media sosial dan layanan streaming. Notebook ini mencoba menjawab pertanyaan:
1. Seberapa besar pengaruh **Jam Belajar vs. Jam Main Sosmed** terhadap nilai ujian?
2. Apakah mahasiswa yang rutin berolahraga memiliki nilai akademik yang lebih baik?
3. Bagaimana peran latar belakang orang tua terhadap prestasi mahasiswa?

## 📂 Dataset Features
Dataset ini terdiri dari **1000 baris data** dengan fitur-fitur berikut:

| Kategori | Fitur | Deskripsi | Tipe Data |
| :--- | :--- | :--- | :--- |
| **Target** | `exam_score` | Nilai ujian akhir mahasiswa (0-100) | Float |
| **Academic** | `study_hours_per_day` | Rata-rata jam belajar per hari | Float |
| | `attendance_percentage` | Persentase kehadiran di kelas | Float |
| **Lifestyle** | `sleep_hours` | Rata-rata jam tidur per hari | Float |
| | `social_media_hours` | Durasi penggunaan media sosial harian | Float |
| | `netflix_hours` | Durasi menonton Netflix harian | Float |
| | `exercise_frequency` | Frekuensi olahraga (kali/minggu) | Int |
| | `diet_quality` | Kualitas pola makan (Poor/Fair/Good) | Categorical |
| **Demographic** | `age` | Usia mahasiswa | Int |
| | `gender` | Jenis kelamin | Categorical |
| | `parental_education_level` | Tingkat pendidikan orang tua | Categorical |
| **Other** | `part_time_job` | Status bekerja paruh waktu (Yes/No) | Categorical |
| | `internet_quality` | Kualitas koneksi internet | Categorical |
| | `mental_health_rating` | Penilaian kesehatan mental diri sendiri (1-10) | Int |
| | `extracurricular_participation`| Ikut kegiatan ekskul (Yes/No) | Categorical |

> **Catatan Data:** Terdapat *missing values* pada kolom `parental_education_level` yang telah ditangani dalam proses *data cleaning*.

## 🛠 Tech Stack
Proyek ini dikerjakan menggunakan **Python** dengan library:
* **Pandas**: Pembersihan dan manipulasi data (Data Cleaning).
* **NumPy**: Operasi numerik.
* **Seaborn & Matplotlib**: Visualisasi data (Heatmap, Scatter plot, Bar chart).
* **Scikit-Learn**: Membangun model prediksi (Linear Regression/Random Forest).

## 🚀 Project Workflow
1.  **Data Loading & Inspection**: Memeriksa tipe data dan kelengkapan nilai (handling null values pada kolom pendidikan orang tua).
2.  **Exploratory Data Analysis (EDA)**:
    * Menganalisis distribusi nilai ujian.
    * Mencari korelasi antara *Study Hours* dan *Exam Score*.
    * Membandingkan rata-rata nilai berdasarkan *Gender* dan *Part-time Job*.
3.  **Feature Engineering**: Mengubah data kategorikal (seperti `gender`, `diet_quality`) menjadi format numerik agar bisa diproses oleh model.
4.  **Modeling**: Melatih model untuk memprediksi nilai ujian.
5.  **Prediction System**: Membuat input interaktif di mana pengguna bisa memasukkan data kebiasaan mereka dan mendapatkan prediksi nilai.

## 📊 Key Insights (Contoh)
* Terdapat korelasi positif yang kuat antara **Persentase Kehadiran** dengan **Nilai Ujian**.
* Mahasiswa dengan **Kualitas Tidur** yang baik cenderung memiliki stabilitas mental dan nilai yang lebih tinggi.
* Penggunaan **Media Sosial** yang berlebihan (> 4 jam) menunjukkan tren penurunan pada performa akademik.

## 💻 How to Run
1.  Clone repositori ini:
    ```bash
    git clone [https://github.com/username-kamu/student-performance-analysis.git](https://github.com/username-kamu/student-performance-analysis.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  Jalankan Jupyter Notebook:
    ```bash
    jupyter notebook "Student_Habits_Performance.ipynb"
    ```

---
*Created by Rizcy - 2025*
