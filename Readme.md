# 📊 Penerapan Algoritma Apriori untuk Market Basket Analysis

## 📖 Deskripsi Proyek

Project ini merupakan implementasi *Algoritma Apriori* secara *manual (without library Apriori)* menggunakan Python untuk menemukan pola pembelian pelanggan (Market Basket Analysis).

Implementasi dilakukan tanpa menggunakan library khusus seperti mlxtend.frequent_patterns.apriori, sehingga seluruh proses mulai dari pembentukan kandidat, perhitungan support, pruning, hingga pembentukan association rules dibuat secara mandiri.

Project ini dibuat sebagai tugas mata kuliah *Machine Learning*.

---

## 🎯 Tujuan

- Mengimplementasikan algoritma Apriori dari awal.
- Menemukan Frequent Itemset.
- Membentuk Association Rules.
- Menghitung Support, Confidence, dan Lift.
- Memahami proses kerja Apriori secara manual.

---

## 📂 Dataset

Dataset yang digunakan:

*Market Basket Optimisation Dataset*

- Jumlah transaksi : *7.501*
- Jumlah produk : *120 item*

Dataset berisi transaksi pembelian pelanggan supermarket yang digunakan untuk mencari pola hubungan antar produk.

---

## ⚙️ Tahapan Algoritma

Implementasi terdiri dari beberapa tahapan berikut:

1. Import Library
2. Load Dataset
3. Data Preprocessing
4. Membentuk Transaction List
5. Mengubah Data menjadi Set
6. Menghitung Support
7. Candidate Generation
8. Frequent Itemset
9. Apriori Property (Pruning)
10. Association Rule
11. Perhitungan Confidence
12. Perhitungan Lift
13. Visualisasi Hasil

---

## 📈 Parameter

| Parameter | Nilai |
|-----------|--------|
| Minimum Support | 0.02 (2%) |

---

## 📊 Hasil Frequent Itemset

| Level | Kandidat | Frequent Itemset |
|-------|----------:|-----------------:|
| Level 1 | 120 | 53 |
| Level 2 | 1.378 | 50 |
| Level 3 | 61 | 0 |

---

## 📚 Rumus yang Digunakan

### Support

\[
Support(A)=\frac{Jumlah\ transaksi\ yang\ mengandung\ A}{Jumlah\ seluruh\ transaksi}
\]

---

### Confidence

\[
Confidence(A→B)=
\frac{Support(A∩B)}
{Support(A)}
\]

---

### Lift

\[
Lift=
\frac{Confidence(A→B)}
{Support(B)}
\]

---

## 🔄 Alur Algoritma

text
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
Pruning (Apriori Property)
   │
   ▼
Frequent 3-itemset
   │
   ▼
Association Rules
   │
   ▼
Confidence
   │
   ▼
Lift


---

## 📌 Apriori Property

Algoritma Apriori menggunakan prinsip:

> *Jika suatu itemset tidak memenuhi minimum support, maka semua superset yang mengandung item tersebut juga tidak mungkin memenuhi minimum support.*

Prinsip ini digunakan untuk melakukan *pruning* sehingga proses pencarian menjadi lebih efisien.

---

## 📊 Visualisasi

Project ini menampilkan beberapa visualisasi, antara lain:

- Distribusi transaksi
- Top Frequent Item
- Top Frequent Itemset
- Scatter Plot Support vs Confidence
- Top Association Rules berdasarkan Lift

---

## 🛠️ Teknologi

- Python
- Pandas
- NumPy
- Matplotlib
- itertools
- collections
- time

---

## 📁 Struktur Project


├── Apriori_Market_Basket.ipynb
├── Market_Basket_Optimisation.csv
├── README.md


---

## 🚀 Cara Menjalankan

1. Clone repository

bash
git clone https://github.com/username/repository.git


2. Masuk ke folder project

bash
cd repository


3. Install library

bash
pip install pandas numpy matplotlib


4. Jalankan notebook

bash
jupyter notebook


Kemudian buka file:


Apriori_Market_Basket.ipynb


---

## 📌 Kesimpulan

Implementasi berhasil menemukan pola pembelian pelanggan menggunakan Algoritma Apriori secara manual. Dengan menerapkan proses *candidate generation, **Apriori Property, **support, **confidence, dan **lift*, sistem mampu menghasilkan association rules yang dapat dimanfaatkan sebagai dasar rekomendasi produk, strategi promosi, serta penataan produk pada Market Basket Analysis.

---

## 👩‍💻 Author

*Juwita Sara Safitri*  
Teknik Informatika  
Universitas Nahdlatul Ulama Indonesia Bogor