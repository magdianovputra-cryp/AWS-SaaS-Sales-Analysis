# AWS-SaaS-Sales-Analysis

## **Latar Belakang**
AWS SaaS Sales adalah perusahaan yang bergerak di bidang penjualan perangkat lunak sebagai layanan (SaaS) melalui platform Amazon Web Services (AWS). Perusahaan ini menyediakan berbagai solusi perangkat lunak yang dapat diakses secara online, memungkinkan pelanggan untuk mengelola bisnis mereka dengan lebih efisien dan efektif. Dengan memanfaatkan infrastruktur cloud AWS, AWS SaaS Sales menawarkan skalabilitas, keamanan, dan fleksibilitas yang tinggi bagi para pelanggannya.

## **Pernyataan Masalah**
Bagaimana tren penjualan dan profitabilitas AWS SaaS berubah dari waktu ke waktu (per bulan tiap tahun)?
- Apakah terdapat pola musiman atau periode tertentu yang menunjukkan peningkatan atau penurunan signifikan dalam kinerja penjualan?

Sejauh mana pemberian diskon memengaruhi profitabilitas penjualan?
- Apakah peningkatan diskon mendorong volume penjualan yang cukup untuk menutupi penurunan margin keuntungan, atau justru menyebabkan kerugian?

Bagaimana perilaku pelanggan dapat dikelompokkan menggunakan model LRFM (Length, Recency, Frequency, Monetary)?
- Segmen pelanggan mana yang memberikan kontribusi tertinggi terhadap penjualan, dan segmen mana yang berisiko menurun atau perlu strategi retensi khusus?

## **Tujuan Analisis**
Tujuan dari analisis ini mencakup:
- Mengidentifikasi trend penjualan dan profitabilitas berdasarkan waktu (per bulan pada setiap tahun).
- Mengidentifikasi pengaruh diskon terhadap profitabilitas penjualan.
- Menganalisis perilaku pelanggan berdasarkan segmen LRFM (Length, Recency, Frequency, Monetary).

## **Data**
Dalam dataset ini, terdapat 19 kolom dengan berbagai tipe data, yaitu numerik dan kategorikal. Berikut adalah deskripsi singkat dari setiap kolom dalam dataset:

1. Row ID: Identitas unik untuk setiap transaksi.

2. Order ID: Identitas unik untuk setiap pesanan.

3. Order Date: Tanggal ketika pesanan dilakukan.

4. Date Key: Representasi numerik dari tanggal pesanan (format YYYYMMDD).

5. Contact Name: Nama orang yang melakukan pesanan.

6. Country: Negara tempat pesanan dilakukan.

7. City: Kota tempat pesanan dilakukan.

8. Region: Wilayah tempat pesanan dilakukan.

9. Subregion: Sub-wilayah tempat pesanan dilakukan.

10. Customer: Nama perusahaan yang melakukan pesanan.

11. Customer ID: Identitas unik untuk setiap pelanggan.

12. Industry: Industri tempat pelanggan berada.

13. Segment: Segmen pelanggan (SMB, Strategic, Enterprise).

14. Product: Produk yang dipesan.

15. License: License key produk.

16. Sales: Total nilai penjualan dari transaksi.

17. Quantity: Jumlah item dalam transaksi.

18. Discount: Diskon yang diterapkan pada transaksi.

19. Profit: Laba dari transaksi.

## Kesimpulan
1. Analisis Kinerja Penjualan
- Analisis tren penjualan dan profit menunjukkan pertumbuhan bisnis yang positif dari 2020 ke 2023
- Penjualan dan profit sama-sama meningkat signifikan di akhir tahun, menandakan adanya pola musiman (Peak Season).
- Sebaliknya pada awal tahun, selalu menunjukkan adanya penurunan pada sales dan profit yang menandakan bahwa pada awal tahun merupakan Low Season.

2. Pengaruh Diskon terhadap Profit
- Berdasarkan analisis, diskon 30% ke atas cenderung memberikan rata-rata profit yang negatif. Hal ini menunjukkan bahwa diskon yang terlalu tinggi dapat merugikan perusahaan, sehingga perlu strategi diskon yang lebih bijak untuk menjaga profitabilitas.
- Korelasi antara diskon dan profit adalah -0.22, yang menunjukkan korelasi negatif lemah. Artinya, semakin tinggi diskon yang diberikan, cenderung semakin rendah profit yang diperoleh.
- Produk "Marketing Suite" menjadi satu-satunya produk yang memiliki rata-rata profit negatif. Hal ini menunjukkan bahwa perlu adanya peninjauan ulang, seperti strategi pemasaran atau penetapan harga untuk produk tersebut agar dapat meningkatkan profitabilitasnya.

3. Analisis LRFM
- Pelanggan baru mendominasi jumlah pelanggan (New Cust Low Value), tapi kontribusi nilai tertinggi justru datang dari New Cust High Value dan Loyal Customer. 
- Loyal Customer punya rata-rata pembelian tertinggi, menunjukkan potensi profit jangka panjang yang kuat. 
- Segmen “At Risk” masih punya total transaksi yang cukup tinggi.
- Segmen “Old Cust Inactive” dan “Potential Loyal Cust” jumlah dan nilai transaksinya kecil.
- **Anthem** dan **Ford Motor** dapat dijadikan target utama untuk program loyalitas dan penawaran eksklusif guna mempertahankan hubungan bisnis yang kuat.

## Rekomendasi
1. Optimalkan Strategi Pemasaran baik pada Akhir Tahun (Peak Season) ataupun Awal Tahun (Low Season)
- Luncurkan kampanye bertema musiman seperti Year-End Sale, Holiday Promo, atau Cashback Akhir Tahun untuk memaksimalkan momentum.
- Buat campaign khusus awal tahun seperti New Year Deals atau Product Refresh Discounts untuk menjaga arus penjualan agar tetap stabil di periode low season ini

2. Pengelolaan Diskon secara Strategis
- Berdasarkan analisis, diskon di atas 30% cenderung memberikan rata-rata profit negatif. Oleh karena itu, diskon di atas 30% sebaiknya dihindari atau jika memang diperlukan, harus diimbangi dengan strategi lain seperti bundling produk atau upselling untuk menjaga profitabilitas.
- Perusahaan harus fokus pada efektivitas diskon, memastikan bahwa diskon yang diberikan benar-benar mendorong penjualan tambahan tanpa mengorbankan margin keuntungan. Dari visualisasi diskon moderat (10-20%) memberikan rata-rata profit yang positif, sehingga diskon moderat ini dapat dipertimbangkan sebagai strategi diskon yang efektif.

3.  Segmentasi dan Aktivasi Pelanggan
- Fokus pada Pelanggan bernilai tinggi dan loyal, seperti "Anthem" dan "Ford Motor", dengan program loyalitas khusus, penawaran eksklusif, dan layanan pelanggan premium untuk mempertahankan hubungan bisnis yang kuat.
- Retensi Pelanggan Baru Bernilai Tinggi: Fokus pada retensi pelanggan baru yang memiliki nilai pembelian tinggi (New Cust High Value) dengan strategi onboarding yang efektif, penawaran khusus, dan komunikasi yang personal untuk mengubah mereka menjadi pelanggan loyal jangka panjang.
- Dorong repeat purchase cepat untuk New Cust Low Value dengan voucher pembelian kedua, edukasi produk, dan promosi personalisasi untuk membangun engagement awal.
- Lakukan reaktivasi campaign personal untuk Cust At Risk, supaya menghindari mereka benar-benar churn. Karena segment ini masih mempunyai kontribusi yang cukup besar dalam penjualan.

## Link Dashboard Tableau
https://public.tableau.com/app/profile/magdianov.putra/viz/AWSSaaSSalesDashboard_17603588379630/AWSSaaSSalesDashboard?publish=yes

## Link Slide Presentasi
https://www.canva.com/design/DAG1wy-Tnfk/joXMymvX-kQ_0QwNEznMVg/view?utm_content=DAG1wy-Tnfk&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h97cf8cda47
