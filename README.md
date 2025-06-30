## Data yang digunakan
Dataset yang digunakan merupakan data dari DQLab Store yang merupakan e-commerce dimana pembeli dan penjual saling bertemu. Pengguna bisa membeli barang dari pengguna lain yang berjualan. Setiap pengguna bisa menjadi pembeli sekaligus penjual.

Ada 4 tabel yang tersedia,

users, berisi detail data pengguna. Berisi,
1. user_id : ID pengguna
2. nama_user : nama pengguna
3. kodepos : kodepos alamat utama dari pengguna
4. email : email dari pengguna

Total data/baris = 17.936

products, berisi detail data dari produk yang dijual. Berisi,
1. product_id : ID produk
2. desc_product : nama produk
3. category : kategori produk
4. base_price : harga asli dari produk

Total data/baris = 1.145 


orders, berisi transaksi pembelian dari pembeli ke penjual. Berisi,
1. order_id : ID transaksi
2. seller_id : ID dari pengguna yang menjual
3. buyer_id : ID dari pengguna yang membeli
4. kodepos : kodepos alamat pengirimian transaksi (bisa beda dengan alamat utama)
5. subtotal : total harga barang sebelum diskon
6. discount : diskon dari transaksi
7. total : total harga barang setelah dikurangi diskon, yang dibayarkan pembeli
8. created_at : tanggal transaksi
9. paid_at : tanggal dibayar
10. delivery_at : tanggal pengiriman

Total data/baris = 74.874


order_details, berisi detail barang yang dibeli saat transaksi. Berisi,
1. order_detail_id : ID table ini
2. order_id : ID dari transaksi
3. product_id : ID dari masing-masing produk transaksi
4. price : harga barang masing-masing produk
5. quantity : jumlah barang yang dibeli dari masing-masing produk

Total data/baris = 187.452

## Tools yang digunakan
Google bigquery : https://console.cloud.google.com/bigquery?sq=342996244348:ee64a05fdac340edb37038c657b4de9a
