# 🛒 Analisis Data E-commerce DQLab Store dengan Google BigQuery

## 📂 Data yang Digunakan

Dataset yang digunakan merupakan data dari **DQLab Store**

### Struktur Tabel

| Tabel | Deskripsi | Jumlah Baris |
|---|---|---|
| **users** | Data detail pengguna | 17.936 |
| **products** | Data detail produk yang dijual | 1.145 |
| **orders** | Data transaksi pembelian | 74.874 |
| **order_details** | Detail barang pada tiap transaksi | 187.452 |

---

## 🛠️ Tools yang Digunakan

- **Google BigQuery**  
[https://console.cloud.google.com/bigquery?sq=342996244348:ee64a05fdac340edb37038c657b4de9a](https://console.cloud.google.com/bigquery?sq=342996244348:ee64a05fdac340edb37038c657b4de9a)

---

## 📌 Daftar Latihan Query SQL

Berikut adalah beberapa contoh latihan query yang saya kerjakan:

### 📊 1. Exploratory Data (Jumlah Data dan Missing Value)

- **Jumlah baris dan kolom pada tabel `products` dan `orders`**
- **Jumlah kategori produk unik**
- **Cek missing value pada setiap kolom**

### 📈 2. Analisis Transaksi

- **Jumlah transaksi per bulan (September 2019, November 2019, Januari 2020, Maret 2020, Mei 2020)**
- **Jumlah transaksi yang belum dibayar (`paid_at = NA`)**
- **Jumlah transaksi yang sudah dibayar tapi belum dikirim**
- **Transaksi yang dikirim pada hari yang sama dengan pembayaran**

### 👥 3. Analisis Pengguna (Users)

- **Jumlah total pengguna**
- **Jumlah pengguna yang pernah menjadi pembeli**
- **Jumlah pengguna yang pernah menjadi penjual**
- **Jumlah pengguna yang pernah menjadi pembeli sekaligus penjual**

### 🏅 4. Customer Ranking & Behavior

- **Top 5 pembeli dengan total pembelian terbesar**
- **Top 5 pembeli non-diskon dengan transaksi terbanyak**
- **Pembeli aktif sepanjang tahun 2020 dengan rata-rata transaksi > 1 juta**

### 📬 5. Analisis Domain Email Penjual

- **Domain email teratas dari para penjual**

### 📦 6. Analisis Produk

- **Top 5 produk terlaris di Desember 2019 (berdasarkan quantity)**
- **5 kategori dengan total quantity terbanyak di tahun 2020 (khusus transaksi yang sudah terkirim)**

### 💰 7. Analisis Transaksi Individual dan Bulanan

- **10 transaksi terbesar oleh user 12476**
- **Transaksi per bulan sepanjang tahun 2020**
- **10 pembeli dengan rata-rata transaksi terbesar di Januari 2020 (minimal 2 transaksi)**
- **Transaksi di atas 20 juta selama Desember 2019**

### 📦 8. Segmentasi Khusus Pelanggan

- **Dropshipper:** Pembeli dengan ≥10 transaksi dan pengiriman selalu ke alamat berbeda.
- **Reseller Offline:** Pembeli dengan ≥8 transaksi, alamat pengiriman sama dengan alamat utama, dan rata-rata quantity per transaksi > 10.
- **Penjual yang juga pembeli aktif:** Penjual yang pernah melakukan ≥7 transaksi sebagai pembeli.

### ⏳ 9. Analisis Durasi Pembayaran

- **Rata-rata, minimum, dan maksimum lama waktu pembayaran (dari tanggal order ke tanggal bayar)**  
(Per bulan selama tahun 2020)

---

## ✅ Skills dan Pembelajaran yang Didapat

- **Penguasaan dasar-dasar BigQuery**
- **Penggunaan fungsi agregat (COUNT, SUM, AVG, MIN, MAX)**
- **Query kondisi dan filtering (`WHERE`, `HAVING`, `GROUP BY`)**
- **Pengolahan tanggal dengan fungsi `EXTRACT`, `FORMAT_DATE`, `SAFE.PARSE_DATE`**
- **Analisis segmentasi pengguna berbasis perilaku**
- **Join antar tabel (`INNER JOIN`)**
- **Analisis missing value**
- **Menggunakan subquery untuk analisis lebih kompleks**

---

## 📌 Catatan Tambahan
Seluruh latihan ini merupakan bagian dari **latihan self-learning SQl BigQuery** dengan studi kasus data e-commerce.  
Project DQLab **Data Analyst E-Commerce Challenge**

---

