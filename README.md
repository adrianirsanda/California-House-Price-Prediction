# California-House-Price-Prediction

## 1. Business Overview

### Latar Belakang
Sebagai perusahaan agen properti yang beroperasi di wilayah California, kami menghadapi tantangan besar dalam menentukan harga jual rumah yang kompetitif dan realistis. Nilai rumah di California sangat ebrvariasi yang dipengaruhi oleh lokasi geografis, usia bangunan, jumlah kamar, kepadatan penduduk dan tingkat pendapatan masyarakat sekitar.

### Data Utama
Model menggunakan 8 fitur kunci:
1. Distribusi Pendapatan dan Nilai Rumah (`median_income`, `median_house_value`)
2. Karakteristik Hunian (`housing_median_age`, `total_rooms`, `total_bedrooms`)
3. Kepadatan Penduduk (`population`, `households`)
4. Lokasi Geografis (`longitude`, `latitude`)
5. Tipe Rumah (`ocean_proximity`)


---

## 2. Data Sources

- **Dataset:** California House Pricing

### Deskripsi Kolom:


| Nama Kolom           | Deskripsi                                                                     |
| -------------------- | ----------------------------------------------------------------------------- |
| `longitude`          | Garis bujur lokasi rumah (dalam derajat)                                      |
| `latitude`           | Garis lintang lokasi rumah (dalam derajat)                                    |
| `housing_median_age` | Usia median bangunan rumah di area tersebut (dalam tahun)                     |
| `total_rooms`        | Jumlah total kamar di area blok                                               |
| `total_bedrooms`     | Jumlah total kamar tidur di area blok                                         |
| `population`         | Jumlah total penduduk di area blok                                            |
| `households`         | Jumlah total rumah tangga di area blok                                        |
| `median_income`      | Pendapatan median penduduk di area tersebut (dalam satuan puluhan ribu dolar) |
| `ocean_proximity`    | Kategori lokasi relatif terhadap laut (misalnya: `<1H OCEAN`, `INLAND`, dll.) |
| `median_house_value` | Nilai median rumah di area tersebut (dalam dolar AS)                          |
---

## 3. Technologies Used

- **Bahasa Pemrograman:** Python
- **Library Machine Learning:**  
  - Scikit-learn  
  - XGBoost  
- **Visualisasi:** Seaborn, Matplotlib
- **Pengelolaan Proyek:** Jupyter Notebook, Git

---

## 4. Models Used & Evaluation

### Model Regresi yang Digunakan:

- Linear Regression  
- Ridge Reggresion
- Lasso Regresion
- KNeighbors Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGB Regressor
- Gradien Boosting Regressor
- Ada Boost Regressor

Model akhir yang digunakan adalah XG Boost Regressor karena memiliki nilai MAE, MAPE, RMSE terkecil dibanding model lainnya

---
### Metrik Evaluasi:

- Mean absolute error (MAE) 
- Mean absolute percentage error(MAPE)

Model fokus melihat niali MAE dan MAPE untuk mempermudah interpretasi

---
**Performa Model**

Model XG Boost Regressor menunjukkan hasil terbaik dari seluruh metrik evaluasi:

| RMSE       | MAPE         | MAE          |
|--------------|---------------|---------------|
| $40.529,03          | 16.2%     | $27.901,88     |

---
**Limitasi model**

Hanya dapat menggunakan fitur tertentu dan wilayah california saja
