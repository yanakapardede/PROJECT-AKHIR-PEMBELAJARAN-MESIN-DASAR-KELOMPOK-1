# Prediksi Viralitas Konten TikTok Menggunakan Machine Learning

## Deskripsi Proyek
Proyek ini bertujuan untuk memprediksi viralitas konten TikTok berdasarkan data engagement pengguna menggunakan metode Machine Learning. Data yang digunakan berasal dari dataset **TikTok 2025** yang diperoleh dari Kaggle dan terdiri dari informasi seperti *likes, comments, shares,* dan *plays*.
Penelitian dilakukan melalui beberapa tahapan mulai dari preprocessing data, penanganan ketidakseimbangan kelas menggunakan SMOTE, seleksi fitur menggunakan SelectKBest, hingga pembangunan model klasifikasi menggunakan Support Vector Machine (SVM) dan Multi Layer Perceptron (MLP).

## Anggota Kelompok 1
| No | Nama                      | NIM         |
| -- | ------------------------- | ----------- |
| 1  | Yanaka Sofia Pardede      | 24031554065 |
| 2  | Ayu Wulan Anggraeni Putri | 24031554177 |
| 3  | Annisa Ramadhani          | 24031554206 |
Kelas: **2024B**

## Dataset
* Dataset: TikTok 2025 Dataset
* Sumber: Kaggle
* Jumlah Data: 7.225 konten TikTok

### Fitur yang Digunakan
| Fitur    | Deskripsi              |
| -------- | ---------------------- |
| Likes    | Jumlah suka pada video |
| Comments | Jumlah komentar        |
| Shares   | Jumlah dibagikan       |
| Plays    | Jumlah tayangan video  |

## Tahapan Penelitian
1. Dataset Collection
2. Data Understanding
3. Data Preprocessing
4. Data Balancing (SMOTE)
5. Exploratory Data Analysis (EDA)
6. Feature Selection (SelectKBest)
7. Data Splitting
8. Model Development
9. Model Evaluation
10. Result Analysis

## Metode yang Digunakan
### Feature Selection
* SelectKBest (ANOVA F-Test)

### Data Balancing
* SMOTE (Synthetic Minority Oversampling Technique)

### Machine Learning Models
* Support Vector Machine (SVM)
* Multi Layer Perceptron (MLP)

## Hasil Feature Selection

| Ranking | Feature  |   Score |
| ------- | -------- | ------: |
| 1       | Plays    | 1947.20 |
| 2       | Likes    | 1580.23 |
| 3       | Shares   |  738.03 |
| 4       | Comments |  317.73 |
Hasil menunjukkan bahwa fitur **plays** menjadi faktor paling berpengaruh dalam proses klasifikasi viralitas konten TikTok.

## Hasil Evaluasi Model
| Model | Accuracy | Precision |  Recall | F1-Score |
| ----- | -------: | --------: | ------: | -------: |
| SVM   |   97.92% |    92.61% | 100.00% |   96.16% |
| MLP   |  100.00% |   100.00% | 100.00% |  100.00% |
Model **MLP** memberikan performa terbaik pada dataset yang digunakan dalam penelitian ini.

## Kesimpulan
Berdasarkan hasil penelitian, data engagement TikTok dapat dimanfaatkan untuk melakukan klasifikasi konten viral dan tidak viral dengan tingkat akurasi yang sangat tinggi. Fitur plays, likes, shares, dan comments terbukti memiliki pengaruh terhadap viralitas konten, dengan fitur plays menjadi variabel paling dominan.
Dari dua metode yang diuji, Multi Layer Perceptron (MLP) menghasilkan performa terbaik dengan accuracy, precision, recall, dan F1-score sebesar 100%, sedangkan SVM memperoleh accuracy sebesar 97,92%.
