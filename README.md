# Analisis Prediktif Karakteristik Bangunan Tahan Gempa 🏢🚀

## Pendahuluan

### Latar Belakang
Gempa bumi merupakan bencana alam yang seringkali menimbulkan kerusakan besar, baik dari segi korban jiwa maupun material. Analisis karakteristik bangunan yang tahan gempa menjadi krusial untuk meminimalisir dampak buruk. Artikel ini menggali potensi model prediktif menggunakan XGBoost Classifier untuk meramalkan tingkat kerusakan bangunan saat gempa.

### Rumusan Masalah
1. Apa saja karakteristik bangunan yang memiliki tingkat kerusakan rendah setelah terkena gempa?
2. Bagaimana memilih model prediksi yang tepat berdasarkan fitur-fitur bangunan?
3. Seberapa akurat hasil prediksi model yang telah dipilih?

### Tujuan
1. Menemukan karakteristik bangunan yang tahan gempa.
2. Memilih model prediksi terbaik berdasarkan fitur-fitur bangunan.
3. Mengevaluasi akurasi hasil prediksi dari model yang dipilih.

### Manfaat
1. Memberikan panduan untuk perbaikan standar pembangunan bangunan tahan gempa.
2. Menjadi referensi bagi peneliti dan kontribusi pada pemahaman metode antisipasi bencana alam.

## Metode

### Perangkat Lunak
- Python v3.9.16
- Conda v22.11.1
- Libraries: jupyter, pandas, numpy, scikit-learn, xgboost, pickle, matplotlib, seaborn, cudatoolkit
- Microsoft Excel

### Dataset
Dataset awal terdiri dari dua file csv: train.csv dan test.csv. Dilakukan normalisasi dan penanganan nilai kosong.

### Algoritma
1. **Frequent Category Imputation:** Imputasi menggunakan nilai modus pada kolom kategorikal dengan persentase nilai kosong kurang dari 10%.
2. **K-Nearest Neighbour Imputation:** Imputasi menggunakan algoritma K-Nearest Neighbour pada kolom numerik.
3. **Gradient Boosting Machines (XGBoost):** Model prediksi untuk analisis tingkat kerusakan bangunan.

### Data Cleaning
Pembersihan data melibatkan penghapusan baris dengan nilai kosong yang signifikan dan normalisasi kolom-kolom tertentu.

### Feature Engineering
Pemisahan matriks fitur dan target, label encoding untuk kolom kategorikal, dan penanganan nilai kosong pada kolom numerik.

## Analisis Data Eksplorasi dan Model Prediksi

### Analisis Data Eksplorasi
- Analisis univariat dan bivariat menunjukkan pola kerusakan bangunan berdasarkan tipe pondasi, jenis lantai dasar, jenis beton, bahan perekat dinding, dan material dinding.

### Model Prediksi
- Model XGBoost Classifier diimplementasikan dan dioptimalkan menggunakan GridSearchCV.
- Evaluasi model dilakukan pada Kaggle Competition dengan metrics f1-score, menghasilkan akurasi sebesar 0.31614.

## Kesimpulan

Hasil analisis data eksplorasi memberikan wawasan tentang karakteristik bangunan yang tahan gempa. Meskipun model XGBoost Classifier memberikan hasil yang memuaskan, disarankan untuk terus mencari model dan tuning parameter yang lebih baik. Analisis ini diharapkan dapat menjadi landasan untuk perbaikan standar pembangunan bangunan yang lebih tahan gempa di masa depan. 🌐🏗️

*Catatan: Dataset dapat diakses [di sini](https://drive.google.com/drive/folders/1Y5IyCeOs2yeOXFYkx6ZSHzK3QfnZR769?hl=id).*
