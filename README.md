# Machine-Learning-Bank-Marketing
Model untuk memprediksi nasabah yang akan berlangganan deposito, dengan **ROC-AUC 0.81**.

##  Dataset

- Sumber: UCI Machine Learning Repository
- File: `bank-additional-full.csv`
- Target: `y` (yes/no → 1/0)

##  Langkah-langkah

1. **Load Data**:
   - Mengimpor dataset CSV menggunakan `pandas`
   - Melihat struktur data (shape, info, head)

2. **Data Preparation**:
   - Mengganti nilai `'unknown'` dengan `NaN`
   - Menghapus kolom yang tidak relevan (`duration`)
   - Mengubah label target menjadi numerik (`yes` → 1, `no` → 0)

3. **Exploratory Data Analysis (EDA)**:
   - Distribusi umur, pekerjaan, dan target
   - Boxplot & countplot fitur terhadap target
   - Korelasi antar fitur numerik (heatmap)

4. **Preprocessing**:
   - Imputasi nilai hilang (median/categorical)
   - One-hot encoding untuk fitur kategorikal
   - Train-test split (stratified)

5. **Modeling**:
   - Logistic Regression
   - Random Forest Classifier

6. **Evaluasi**:
   - Akurasi, ROC AUC
   - Classification Report

7. **Modeling Pipeline** 🧱:
   - Menggunakan `Pipeline` dari Scikit-learn untuk menyatukan proses:
     - Imputasi missing value
     - Encoding fitur kategorikal
     - Training model (Logistic Regression / Random Forest)
   - Pipeline memastikan preprocessing dan model training terjadi dalam satu alur yang konsisten.


##  Tools

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

##  Hasil

- Akurasi: 89%
- Model terbaik: Random Forest

##  Struktur Folder

Machine Learning-Bank Marketing/ 
├── data/ 
│	 └── bank-additional-full.csv
├── model/
│	 ├── Bank_Marleting-ML.ipynb
│	 └── best_model.pkl
├── requirements.txt 
├── README.md 


##  Author

Irpan Maulana  
GitHub: [@Voldigord](https://github.com/Voldigord)
