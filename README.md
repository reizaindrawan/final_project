# Summary Insight Exploratory Data Analysis

## Descriptive Analysis dan Univariate Analysis

1. Berdasarkan distribusi histoghram, Kolom `Complain dan Citier` merupakan kategorikal jadi untuk  tahap selanjutnya dimasukan ke kelompok kategori.
2. Tipe data target `Churn` bisa diubah ke bentuk Boolean.
3. Kolom `Statisfactionscore` yang merupakan kolom mengenai rating customer dapat sebagai data numerik dan kategorik sekaligus. Saat masuk ke pre-processing disesuaikan saja mau melihatnya di sudut pandang numerik atau kategorik.
4. Untuk `customer id` memiliki nilai unik  sejumlah dataset sehingga tidak perlu dimasukan ke dalam fitur nantinya.
5. Berdasarkan hasil distribusi boxplot dan histplot `banyak fitur yang bersifat positive skewed` dimana nilai mean > median yang berarti banyak outlier yang berada di nilai besar. Hal ini perlu di perhatikan lebih jauh ketika akan melakukan preprocessing bisa dengan melakukan  feature transformation (seperti : normalization, standardization, atau log transformation)
6. Berdasarkan analisa yang di lakukan pengelompokan numerik  sebanyak 10 data dan kategorik 10 data. Berikut pembagiannya:



## Multivariate Analysis

1. Ada beberapa fitur yang memiliki korelasi yang sangat signifikan & tidak terlalu signifkan terhadap label serta ada fitur yang tidak memiliki korelasi terhadap label. Fitur yang paling relevan terhadap label dan harus dipertahankan ialah : PreferredLoginDevice, PreferredPaymentMode, Gender, PreferedOrderCat, MaritalStatus, SatisficationScore, Complain
2. Ada beberapa fitur yang memiliki korelasi positif & korelasi negatif dengan fitur yang lainnya serta fitur OrderCount dengan  CouponUsed yang memiliki korelasi 0,75 yang membuat kedua fitur tersebut redundan oleh sebab itu salah satu dari kedua fitur tersebut harus dihapus untuk meningkatkan efisiensi penyimpanan data

## Business Insight
1. 53% yang churn melakukan complain
2. 52% customer yang churn memiliki satisfaction score dibawah 4
3. 66% yang churn menggunakan mobile device
4. 65% yang churn memiliki tenure yang rendah (1-2)
5. 72% yang churn hanya melakukan order 1-2x

## Rekomendasi

1. Menerima dan mendata complain customer untuk dijadikan bahan evaluasi
2. Memberikan pelayanan yang terbaik dan konsisten
3. Bisa memberikan promo khusus bagi pengguna mobile device agar tidak churn
4. Analisa apa saja competitor yang ada serta manfaat yang diberikan oleh competitor seperti harga, layanan, fitur, dll

