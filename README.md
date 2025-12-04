# Health-Insurance-Pricing---Risk-Estimation
  Analisis biaya asuransi kesehatan berbasis data + risk scoring + scenario analysis

## Overview
Project ini bertujuan untuk memprediksi biaya asuransi kesehatan (insurance charges) serta mengembangkan risk scoring sederhana untuk mendukung pengambilan keputusan bisnis: penetapan premi, identifikasi pelanggan berisiko tinggi, dan simulasi dampak kebijakan harga.

## Dataset
Sumber: Medical Insurance Cost Dataset (https://www.kaggle.com/datasets/mosapabdelghany/medical-insurance-cost-dataset)
Jumlah data: 1338 rows
Fitur utama:
- age: usia
- sex: gender
- bmi: body mass index
- children: jumlah tanggungan
- smoker: perokok / bukan
- region: area tempat tinggal
- charges: biaya asuransi (target)
  
## Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn (EDA)
- Scikit-Learn (regression & modeling)
- Plotly (nteractive chart)
- Jupyter Notebook

## Objectives
- Membuat risk scoring berdasarkan fitur risiko (age, BMI, smoker).
- Memprediksi insurance charges menggunakan model regresi (Linear Regression / Random Forest).
- Melakukan scenario analysis (misal pengurangan BMI, non-smoker simulation).
- Menghasilkan business insights yang dapat digunakan untuk pricing & strategi pelanggan.

## Workflow
1. Data Cleaning
- Cek missing values
- Cek distribusi & outlier
- Encoding categorical features
2. EDA Visualization
- Korelasi
- Distribusi charges
- Pengaruh usia, BMI, dan smoker
3. Risk Scoring
- Menetapkan bobot risiko
- Menghasilkan skor risiko 0–100
4. Regression Modeling
- Train-test split
- Evaluasi model (MAE, RMSE, R²)
- Feature importance
5. Scenario Analysis
- Simulasi perubahan BMI
- Simulasi menjadi non-smoker
- Dampak terhadap prediksi biaya

## Business Insights (Ringkasan)

1. Faktor risiko terbesar

   <img width="558" height="451" alt="image" src="https://github.com/user-attachments/assets/fba52fdf-3c5e-452f-b996-361ca410ab73" />
- Smoker meningkatkan biaya hingga 200–300% dibanding non-smoker.

     <img width="720" height="470" alt="image" src="https://github.com/user-attachments/assets/e2c909d7-5a83-4759-9378-cc14184d777c" />
     
- BMI tinggi berhubungan dengan biaya yang lebih besar.
- Usia berpengaruh stabil dan signifikan.

- <img width="713" height="470" alt="image" src="https://github.com/user-attachments/assets/6513066c-fc10-4910-a2aa-9c89f38cfca2" />


  
2. Pelanggan smoker + BMI tinggi = segmen biaya tertinggi
- Cocok untuk targeted health program (diet, stop-smoking support).

3. Scenario Analysis menunjukkan
- Menurunkan BMI 5 poin bisa menurunkan biaya prediksi signifikan.
- Perubahan status dari smoker → non-smoker memberikan penurunan terbesar.

4. Implikasi bisnis
- Premi dapat di-tier menggunakan risk scoring.
- Memberikan diskon premi untuk pelanggan yang mengikuti program kesehatan.
