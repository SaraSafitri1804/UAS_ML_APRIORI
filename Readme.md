📊 Penerapan Algoritma Apriori untuk Market Basket Analysis

> Implementasi Algoritma Apriori secara manual (without Apriori library) menggunakan Python untuk menemukan pola pembelian pelanggan (Market Basket Analysis).




---

📌 Informasi Project

Informasi	Keterangan

Mata Kuliah	Machine Learning
Metode	Algoritma Apriori
Bahasa	Python
Tools	Jupyter Notebook
Dataset	Market Basket Optimisation
Total Transaksi	7.501
Jumlah Item	120



---

🎯 Tujuan

Project ini bertujuan untuk:

Mengimplementasikan algoritma Apriori tanpa library khusus.

Menghitung Support, Confidence, dan Lift secara manual.

Menemukan Frequent Itemset.

Membentuk Association Rules.

Menganalisis pola pembelian pelanggan.



---

📂 Struktur Repository

UAS_ML_APRIORI
│
├── Apriori_Market_Basket.ipynb
├── Market_Basket_Optimisation.csv
├── README.md
└── assets/


---

⚙️ Library yang Digunakan

pandas
numpy
matplotlib
itertools
collections
time

Install library

pip install pandas numpy matplotlib


---

🔄 Alur Algoritma

Dataset
      │
      ▼
Preprocessing
      │
      ▼
Hitung Support
      │
      ▼
Frequent 1-itemset
      │
      ▼
Generate Candidate
      │
      ▼
Frequent 2-itemset
      │
      ▼
Join
      │
      ▼
Apriori Property
      │
      ▼
Pruning
      │
      ▼
Frequent 3-itemset
      │
      ▼
Association Rule
      │
      ▼
Confidence
      │
      ▼
Lift


---

📈 Hasil Frequent Itemset

Level	Candidate	Frequent

1	120	53
2	1.378	50
3	61	0



---

📊 Rumus

Support

Support(A)=\frac{\text{Jumlah transaksi mengandung A}}{\text{Jumlah seluruh transaksi}}


---

Confidence

Confidence(A→B)=
\frac{Support(A∩B)}
{Support(A)}


---

Lift

Lift=
\frac{Confidence(A→B)}
{Support(B)}


---

📌 Apriori Property

> Jika suatu itemset tidak memenuhi minimum support, maka seluruh superset yang mengandung item tersebut juga tidak mungkin memenuhi minimum support.



Prinsip ini digunakan untuk mengurangi jumlah kandidat (pruning) sehingga proses pencarian menjadi lebih efisien.


---

🚀 Cara Menjalankan

Clone repository

git clone https://github.com/SaraSafitri1804/UAS_ML_APRIORI.git

Masuk ke folder

cd UAS_ML_APRIORI

Install library

pip install pandas numpy matplotlib

Jalankan

jupyter notebook

Buka file

Apriori_Market_Basket.ipynb


---

📊 Hasil Analisis

Implementasi berhasil menemukan pola pembelian pelanggan menggunakan Algoritma Apriori.

Dengan minimum support 2%, diperoleh:

53 Frequent 1-itemset

50 Frequent 2-itemset

Tidak ditemukan Frequent 3-itemset


Association Rules kemudian dibentuk menggunakan nilai Confidence dan Lift.


---

📷 Output Program

Tambahkan hasil screenshot seperti:

assets/
├── dataset.png
├── support.png
├── frequent_itemset.png
├── association_rules.png
└── lift.png

Lalu tampilkan pada README:

## Hasil Program

### Dataset

![Dataset](assets/dataset.png)

### Frequent Itemset

![Frequent](assets/frequent_itemset.png)

### Association Rules

![Rules](assets/association_rules.png)


---

👩‍💻 Author

Juwita Sara Safitri
NIM: 24260006
Program Studi Teknik Informatika
Universitas Nahdlatul Ulama Indonesia Bogor
