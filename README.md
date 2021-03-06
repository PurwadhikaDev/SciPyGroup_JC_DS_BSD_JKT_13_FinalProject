# SciPyGroup_JC_DS_BSD_JKT_13_FinalProject

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Daftar Isi</summary>
  <ol>
    <li>
      <a href="#project-description">Project Description</a>
    </li>
    <li>
      <a href="#bussiness-problem">Business Problem</a>
    </li>
    <li>
      <a href="#data-understanding">Data Understanding</a>
    </li>
    <li><a href="#eda">EDA</a></li>
    <li><a href="#preprocessing">Preprocessing</a></li>
    <li><a href="#methodology">Methodology</a></li>
    <li><a href="#conclusion-and-recommendation">Conclusion and Recommendation</a></li>
    <li><a href="#contributor">Contributor</a></li>
  </ol>
</details>


<!-- project description -->
## Project Description

Proyek ini menggunakan data mobil bekas di Inggris yang diambil dari <a href="https://www.kaggle.com/adityadesai13/used-car-dataset-ford-and-mercedes?select=audi.csv">Kaggle</a>. 
Tujuan dari proyek ini adalah untuk memprediksi kisaran harga seseorang dalam menjual atau membeli mobil lama dibandingkan dengan harga yang beredar dipasaran. 
Project ini dibuat dengan menggunakan JupyterNotebook dan model Machine Learningnya menggunakan CatBoostRegressor dan Hyperopt untuk melakukan optimasi parameter 
dan MAE Score sebagai scoring matrix. Interpretasi model dilakukan dengan menggunakan SHAP.
* [Jupyter Notebook](https://jupyter.org/)
* [CatBoostRegressor](https://catboost.ai/)
* [Hyperopt](http://hyperopt.github.io/hyperopt/)


<!-- bussiness problem -->
## Bussiness Problem

* **Problem Statement**: Bagaimana cara untuk memprediksi kisaran harga jual mobil bekas sehingga harganya sesuai dengan harga jual yang ada pada pasaran?
* **Value**: harga mobil bekas.
* **Goals**: mendapatkan harga mobil bekas sehingga harganya sesuai dengan harga yang ada pada pasaran.
* **Konteks project**: suatu platform yang mampu memberikan kisaran harga mobil bekas berdasarkan data yang didapatkan dari dealer-dealer mobil bekas di UK, dengan target pengguna platformnya adalah masyarakat umum (end-user).



<!-- data understanding -->
## Data Understanding

| Feature      	| Description                                                                                                                                                                                                               	|
|--------------	|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
| model        	| Tipe mobil                                                                                                                                                                                                                	|
| year         	| Tahun pertama registrasi mobil                                                                                                                                                                                            	|
| price        	| Nilai harga mobil                                                                                                                                                                                                         	|
| transmission 	| Tipe transmisi dari mobil                                                                                                                                                                                                 	|
| mileage      	| Total jarak yang telah ditempuh oleh mobil                                                                                                                                                                                	|
| fuelType     	| Jenis bahan bakar yang digunakan pada mobil                                                                                                                                                                               	|
| tax          	| Nilai pajak mobil                                                                                                                                                                                                         	|
| mpg          	| Miles per gallon; Total jarak tempuh mobil berdasarkan total konsumsi bahan bakar yg digunakan. semakin besar nilai mpg berarti konsumsi bahan bakar yg digunakan akan semakin sedikit (semakin irit)                     	|
| engineSize   	| Engine capacity atau engine displacement (kapasitas mesin); volume total silinder mesin. secara umum, semakin besar nilai kapasitas mesin akan meningkatkan kebutuhan konsumsi bahan bakar (kendaraan akan semakin boros) 	|
| brand        	| Merk mobil                                                                                                                                                                                                                	|
| age          	| Umur mobil dari tahun pertama registrasi mobil hingga tahun saat ini                                                                                                                                                      	|


**FEATURE** = model, transmission, mileage, fuelType, tax, mpg, engineSize, brand, dan age. \
**LABEL** = price.


<!-- eda -->
## EDA

Pada tahap ini akan dilakukan analisa singkat data, sebagai berikut:
* Distribusi data 
* Korelasi data
* Kardinalitas data
* Visualisasi data secara umum
* Mengidentifikasi missing value, anomali dan duplikat data
* Uji Analisa



<!-- preprocessing -->

## Preprocessing
Pada tahap ini akan dilakukan persiapan dan pengolahan data sebelum digunakan sebagai data model, sebagai berikut: 
* Handling missing value
* Mengubah tipe data
* Handling anomaly data
* Menghilangkan data yang terindikasi duplikat
* Feature Engineering


<!-- Methodology -->

## Methodology
Pada tahap ini akan dilakukan pembuatan dan melakukan optimasi model machine learning, sebagai berikut:
1. Memuat model benchmark
2. Model Improvement dengan categorical feature
3. Model Improvement dengan hyperparameter tuning
4. Penentuan feature importance
5. Melakukan validasi model terhadap data testing 
6. Interpretasi model menggunakan SHAP



<!-- conclusion recommendation -->
## Conclusion and Recommendation

Pada tahap ini akan menjelaskan kesimpulan project serta rekomendasi berdasarkan model machine learning yang sudah dibuat.


<!-- contributor -->
## Contributor

Muhammad Fariz Tiowiradin (fariz.tiowiradin@gmail.com) & Endah Sari (endahsari0590@gmail.com)
