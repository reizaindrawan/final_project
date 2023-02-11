# Summary Insight

## Descriptive Analysis dan Univariate Analysis

1. Berdasarkan distribusi histoghram, Kolom Complain dan Citier merupakan kategorikal jadi untuk  tahap selanjutnya dimasukan ke kelompok kategori.
2. Tipe data target Churn bisa diubah ke bentuk Boolean.
3. Kolom Statisfactionscore yang merupakan kolom mengenai rating customer dapat sebagai data numerik dan kategorik sekaligus. Saat masuk ke pre-processing disesuaikan saja mau melihatnya di sudut pandang numerik atau kategorik.
4. Untuk customer id memiliki nilai unik  sejumlah dataset sehingga tidak perlu dimasukan ke dalam fitur nantinya.
5. Berdasarkan hasil distribusi boxplot dan histplot banyak fitur yang bersifat positive skewed dimana nilai mean > median yang berarti banyak outlier yang berada di nilai besar. Hal ini perlu di perhatikan lebih jauh ketika akan melakukan preprocessing bisa dengan melakukan  feature transformation (seperti : normalization, standardization, atau log transformation)
6. Berdasarkan analisa yang di lakukan pengelompokan numerik  sebanyak 10 data dan kategorik 10 data. Berikut pembagiannya:

* Kolom Numerik =  [  'Tenure', 'WarehouseToHome','HourSpendOnApp', 'NumberOfDeviceRegistered', 'NumberOfAddress',  'OrderAmountHikeFromlastYear’ CouponUsed', 'OrderCount', 'DaySinceLastOrder', 'CashbackAmount’]
* Kolom Kategorik =  ['PreferredLoginDevice', 'CityTier',  'Churn', 'PreferredPaymentMode', 'Gender', 'SatisfactionScore’,  'PreferedOrderCat', 'MaritalStatus', 'Complain’]  

