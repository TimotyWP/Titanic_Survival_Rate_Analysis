readme_content_id = """
# Analisis Titanic Passenger Survival Rate

![Titanic]([https://www.exampleimage.com/titanic-banner](https://images.unsplash.com/photo-1510132310763-2df322eed83f?q=80&w=1931&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D))

## Gambaran Proyek
Proyek ini bertujuan untuk menganalisis tingkat kelangsungan hidup penumpang di atas kapal Titanic dengan menggunakan berbagai model machine learning. Proyek ini memfokuskan untuk mencari penyebab dari hasil analisis Survival Rate dari Titanic Dataset

## Tujuan
Tujuan utama dari analisis ini adalah untuk:
- Mengeksplorasi dan memvisualisasikan hubungan antara berbagai atribut penumpang (usia, jenis kelamin, kelas, dll.) dengan tingkat kelangsungan hidup.
- Membangun model prediktif menggunakan machine learning untuk mengklasifikasikan penumpang berdasarkan kemungkinan mereka bertahan hidup.

## Dataset
Dataset yang digunakan untuk analisis ini bersumber dari dataset Titanic di Kaggle. Anda dapat mengakses dataset tersebut [di sini](https://www.kaggle.com/competitions/titanic/data).  

### Fitur dalam Dataset:
- **PassengerId:** ID unik untuk setiap penumpang.
- **Pclass:** Kelas penumpang (1 = Atas, 2 = Menengah, 3 = Bawah).
- **Name:** Nama penumpang.
- **Sex:** Jenis kelamin penumpang.
- **Age:** Usia penumpang.
- **SibSp:** Jumlah saudara kandung atau pasangan yang ikut.
- **Parch:** Jumlah orang tua atau anak yang ikut.
- **Ticket:** Nomor tiket.
- **Fare:** Biaya tiket penumpang.
- **Cabin:** Nomor kabin.
- **Embarked:** Pelabuhan embarkasi (C = Cherbourg, Q = Queenstown, S = Southampton).
- **Survived:** Status kelangsungan hidup (0 = Tidak, 1 = Ya).

## Pendekatan Analisis
1. **Eksplorasi dan Pra-pemrosesan Data:**
   - Menangani data yang hilang.
   - Memvisualisasikan distribusi usia, tarif, dan variabel lainnya.
   - Melakukan encoding fitur kategorikal (misalnya, jenis kelamin).

2. **Visualisasi Data:**
   - Heatmap korelasi untuk mengidentifikasi hubungan signifikan.
   - Bar plot dan grafik tingkat kelangsungan hidup untuk mendapatkan wawasan tentang demografi.

3. **Model Machine Learning:**
   - **Random Forest Classifier:** Digunakan karena kemampuannya yang tangguh dalam menangani dataset besar.
   - **Support Vector Classifier (SVC):** Dikenal karena akurasinya dalam tugas klasifikasi.
   - **Logistic Regression:** Model yang sederhana dan mudah diinterpretasikan untuk klasifikasi biner.
   - **XG Boosting:** Dikenal karena kecepatan dan kinerjanya yang sangat baik dalam menangani dataset besar serta kemampuannya untuk mencegah overfitting.
   
4. **Metrik Evaluasi:**
   - **Akurasi:** Untuk mengevaluasi kinerja keseluruhan.
   - **Confusion Matrix:** Untuk memahami hasil klasifikasi.

## Temuan Utama
- Tingkat kelangsungan hidup lebih tinggi pada wanita dan anak-anak.
- Penumpang di kelas yang lebih tinggi memiliki peluang kelangsungan hidup yang lebih baik.
- Usia dan tarif juga memainkan peran dalam menentukan kemungkinan kelangsungan hidup.

## Dependensi
- Python 3.7+
- Perpustakaan: 
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

Untuk menginstal dependensi, jalankan:
```bash
pip install -r requirements.txt
