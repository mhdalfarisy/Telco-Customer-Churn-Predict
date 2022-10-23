

## PROJECT : # PREDICT CUSTOMER CHURN (TELCO COMPANY)

![a1](https://github.com/mhdalfarisy/mhdalfarisy/blob/main/7-Strategies-To-Reduce-Customer-Churn-Rate.png)

## Table of Contents

- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Metric](#metric)
- [Analytical Approach](#analytical-approach)
- [Definisi Kolom](#definisi-kolom)
- [Data Analyst dan Machine Learning](#data-analyst-dan-machine-learning)
  - [Kesimpulan Data Analyst dan Machine Learning](#kesimpulan-data-analyst-dan-machine-learning)
  - [Saran Data Analyst dan Machine Learning](#saran-data-analyst-dan-machine-learning)
- [Others Data Visualization Report](#others-data-visualization-report)

### **Problem Statement**

Berhentinya pelanggan menggunakan layanan jasa dari perusahaan merupakan metrik penting untuk melakukan evaluasi bisnis. Karena mempertahankan pelanggan yang pergi jauh lebih hemat biaya dari pada mencari pelanggan baru. Hal ini di pengaruhi dari banyak faktor salah satunya pelanggan memilih penyedia layanan lain dan persaingan antara perusahaan setiap tahunnya mencapai 15-25% yang kompetitive untuk mendapatkan pelanggan.

Untuk mengurangi perginya pelanggan dari perusahaan, maka perusahaan perlu melakukan pendekatan pada pelanggan untuk mencengahnya pergi dari perusahaan. Hal ini dapat dilakukan dengan menerapkan machine learning pada bisnis perusahaan dengan menemukan klasifikasi total pelanggan yang seharunya mendapatkan pendekatan dari perusahaan (Dapat berupa promo atau campaign), hal ini diperlukan karena jika perusahaan memberikan pada semua pelanggan untuk campaign dan promonya maka akan memerlukan biaya yang besar sehingga ini akan semakin beresiko pada perusahaan untuk segi beban di laporan laba rugi.

### **Objectives**

Berdasarkan pendahuluan dan rumusan masalah, proyek ini bertujuan untuk mengembangkan model pembelajaran mesin learning yang nanti dapat digunakan perusahaan untuk mengklasifikasi pelanggan mana yang akan pergi dan pelanggan mana yang tidak pergi.

Hal ini akan berguna untuk perusahaan ketika mempertahankan pelanggan yang akan pergi dengan memberikan manfaat promosi dengan target yang lebih jelas dan hal ini akan mengurangi pengeluaran perusahaan dibandingkan ketika perusahaan memberikan promosi kepada semua pelanggan agar mereka tidak pergi dan dampak lainnya ketika promosi difokuskan pada pelanggan yang akan pergi perusahaan akan menghemat biaya promosi dan dapat menambah pendapatan dari pelanggan yang tidak pergi ini.

### **Metric**

- 0 = Non-Churn (Negative)
- 1 = Churn (Positive)

Error tipe 1: False Positive

Kesalahan ini akan menambah beban perusahaan dengan memberikan keuntungan dan promosi kepada pelanggan non-churn dan mengabaikan pelanggan yang berpindah.

Error Tipe 2: False Negative

Kesalahan ini akan membuat perusahaan mengabaikan pelanggan mereka yang berpindah tanpa memberi mereka manfaat/promosi untuk mempertahankan retensi mereka.

### **Analytical Approach**

- Pendekatan analisa ini dengan cara melakukan pembagian variabel pada saat dilakukan Exploratory Data Analyst dan Visualisasi Data:
  - Melakukan Exploratory Data Analyst terhadap seluruh variabel yang ada untuk mengetahui karakteristik pelanggan yang berhenti berlangganan (Jupyter NoteBook).
  - Melakukan Visualisasi data dari setiap analisa untuk mendapatkan gambaran secara visual dari hasil Exploratory Data Analyst (Tableau).
  - Untuk model pembelajaran mesin, kami ingin memprediksi pelanggan yang memiliki risiko churn yang tinggi. Dalam hal ini, kita akan menggunakan Model Klasifikasi untuk memprediksi Churn Customer dan disini difokuskan rekomendasi campaign pada False Positif.

### **Definisi Kolom**
| **Nama Kolom** |**Keterangan Kolom** |
| --- | --- |
|CustomerID| ID unik yang mengidentifikasi setiap pelanggan|
|gender | Jenis kelamin pelanggan|
|Senior Citizen | Menunjukkan jika pelanggan berusia 65 tahun ke atas|
|Partner | Menunjukkan jika pelanggan memiliki akun berbagi|
|Dependents | Menunjukkan jika pelanggan tinggal dengan tanggungan. Tanggungan bisa anak-anak, orang tua, kakek-nenek, dll.|
|Tenure | Berapa lama pelanggan telah menjadi pelanggan|
|Phone Service | Menunjukkan jika pelanggan berlangganan layanan telepon rumah dengan perusahaan|
|MultipleLines | Menunjukkan jika pelanggan berlangganan beberapa saluran telepon dengan perusahaan|
|Internet Service | Menunjukkan apakah pelanggan berlangganan layanan internet|
|Online Security | Menunjukkan jika pelanggan berlangganan layanan keamanan online tambahan|
|Online Backup | Menunjukkan apakah pelanggan berlangganan layanan pencadangan online tambahan|
|DeviceProtection | Menunjukkan jika pelanggan berlangganan perlindungan perangkat tambahan untuk peralatan Internet mereka|
|Tech Support | Menunjukkan apakah pelanggan berlangganan layanan dukungan teknis|
|Streaming TV | Menunjukkan jika pelanggan menggunakan layanan Internet mereka untuk melakukan streaming program televisi dari penyedia pihak ketiga|
|Streaming Film | Menunjukkan jika pelanggan menggunakan layanan Internet mereka untuk melakukan streaming film dari penyedia pihak ketiga|
|Kontrak | Menunjukkan jenis kontrak pelanggan saat ini|
|Paperless Billing | Menunjukkan jika pelanggan telah memilih paperless billing|
|Payment Method | Menunjukkan bagaimana pelanggan membayar tagihan mereka|
|Monthly Charges | Menunjukkan total biaya bulanan pelanggan saat ini untuk semua layanan mereka dari perusahaan|
|Total Charges | Menunjukkan total biaya pelanggan|
|Churn | Menunjukkan apakah pelanggan memiliki TV streaming atau tidak (Ya, Tidak, Tidak ada layanan internet)|

## Data Analyst dan Machine Learning

### **Kesimpulan Data Analyst dan Machine Learning**

1. Pelanggan gender male memiliki persentase berhenti paling banyak 37,3%
2. Pelanggan kurang dari 60 tahun memiliki persentase tertinggi berhenti menggunakan layanan jasa perusahaan
3. Pelanggan yang tidak menggunakan akun pengguna bersama paling banyak berhenti menggunakan layanan perusahaan
4. Pelanggan yang tidak memiliki tanggungan memiliki persentase tertinggi untuk berhenti berlangganan sebanyak 21,9%
5. Pelanggan yang berhenti kurang dari 10 bulan menggunakan jasa layanan perusahaan
6. Jasa layanan telepon rumah memiliki tingkat pelanggan berhenti tertinggi 24,1%
7. Layanan telepon lebih dari 1 dengan hanya 1 pengguna sama sama memiliki tingkat pelanggan berhenti 12,1%
8. Jaringan fiber optik memiliki persentase tertinggi pelanggan berhenti 18,4%
9. Pelanggan berhenti paling banyak yang tidak menggunakan keamanan jaringan tambahan
10. Pelanggan yang tidak menggunakan layanan backup data jasa online paling banyak berhenti 17,5%
11. Dari 43,9% pelanggan tidak menggunakan keamanaan perangkat, ada 17,2% pelanggan berhenti menggunakan layanan perusahaan
12.	Banyak pelangan yang berhenti menggunakan layanan perusahaan dari pelanggan yang tidak menggunakan layanan bantuan teknis
13.	Pelanggan yang berhenti menggunakan layanan jasa perusahaan berasal dari pelanggan yang tidak menggunakan layanan internet untuk straming tv sebanyak 13.4%
14.	Pelanggan yang menggunakan jaringan internet banyak berhenti berlanggan dari kategori yang tidak menggunakan jaringan tersebut untuk straming film dari pihak ketiga sebanyak 13.3%
15.	Kontrak pelanggan dengan perusahaan paling banyak month to month dan ini paling banyak pelanggan yang berhenti 23.5%
16.	Pelanggan yang mendapatkan kertas bukti pembayaran tagihan lebih banyak berhenti berlangganan sebanyak 19.9% 
17.	Pelaggan paling banyak berhenti berlangganan dari metode pembayaran elektronik check 15.2%
18.	Pelanggan yang paling banyak berhenti dari total pembayaran kurang dari 2.000 USD sedangkan pelanggan yang memiliki tagihan di atas 2.000 USD banyak tetap menggunakan layanan perusahaan.
19. Model XGBoost Regressor memiliki skor tertinggi yaitu 56% dan dilakukan tuning skor meningkat menjadi 63%.
20. Pelanggan yang berhenti berlangganan diprediksi 373 orang, setelah dilakukan tuning pada model Model XGBoost Regressor dengan data over sampling diperoleh prediksi pelanggan yang berhenti berlangganan 425 orang.  

## **Saran Data Analyst dan Machine Learning**

1. Fokuskan promosi pada pelangan yang bergender male untuk usia kurang dari 60 tahun dan pelanggan yang menggunakan layanan telekomunikasi untuk keperluan sendiri serta belum memiliki tanggungan dan promosi ini akan berdampak pada pelanggan hingga 12 bulan pertama setelah promosi dengan tujuan mereka akan bisa mereview hasil keuntungan dari promosi ini dan mempercepat perputaran keuangan perusahaan.
2. :
   - a. Produk yang difokuskan ada pada pelanggan yang masih menggunakan telephone rumah, pelanggan yang menggunakan jaringan internet fiber optic, pelanggan yang tidak menggunakan layanan keamanan jaringan, backup data online, bantuan teknis tambahan, keamanan perangkat yang digunakan, pelanggan yang tidak menggunakan layanan straming TV dan Movie dengan pihak ke tiga.
   
   - b. perusahaan dapat membuat paket layanan seperti :
     - 1. Paket layanan telepon seluler + telephone rumah diskon 10% (Untuk pelanggan pengguna Handphone dan Telephone rumah)
     - 2. Paket keamanan jaringan internet pada fiber optic diskon 10% (Untuk pelanggan yang menggunakan jaringan fiber optic dan pelanggan yang tidak menggunakan keamanan jaringan)
     - 3. Paket keamanan jaringan Handphone + Keamanan perangkat diskon 10% (Untuk pelanggan yang menggunakan jaringan internet + Keamanan perangkat)
     - 4. Paket backup data online + Bantuan teknis (Untuk pelanggan yang menginginkan keamanan datanya dapat terjaga dengan realtime)
     - 5. Paket internet straming TV + Movie diskon 12% (Untuk pelanggan yang tidak menggunakan layanan straming TV dan Movie)
     - 6. Diskon tambahan 5% jika mengambil lebih dari 1 paket layanan
#
3. Untuk pelanggan yang masih menggunakan kontrak perbulan, coba di tawarkan untuk menggunakan kontrak 1 tahun dan tawarkan keunggulan / keuntungan yang akan mereka dapatkan terutama dari biaya yang lebih hemat dan berikan diskon tambahan jika mereka menggunakan pembayaran dengan credit card karena credit card memiliki persentase pelanggan berhenti paling kecil atau tawarkan dengan pembayaran tranfer bank karena ini adalah persentase terkecil kedua pelanggan berhenti.

4.  :
   - Target pelangan yang mendapatkan promo sebelum menggunakan machine learning :
   1. Total pelanggan 7.043
   2. Pelanggan yang berhenti berlangganan 1.869
   3. Pendapatan setiap pelanggan (Ex Paket Basic) 1.000 USD
   4. Pendapatan setiap bulan = 7.043 x 1.000 USD = 7.043.000 USD
   5. Biaya marketing per pelanggan yang sudah ada : 10 USD X 1.869 pelanggan = 18.690 USD
   6. Total biaya marketing untuk pelanggan yang sudah ada : 10 USD X 7.043 pelanggan = 70.430 USD per pelanggan yang sudah ada untuk promosinya
   7.  Jika total biaya promosi yang dikeluarkan sebanyak ini, dan bisa menghasilkan pelanggan dengan membeli paket basic ada 7.043.000 USD pendapatan yang perusahaan akan terima (1.000 USD paket basic X 7.043 pelanggan) dengan laba bersih 6.972.570 USD dengan total beban promosi yang dikeluarkan sekitar 1% dibulan berikutnya.
#   
   - Target pelangan yang mendapatkan promo menggunakan machine learning dengan memanfaatkan pelanggan yang sudah ada :
   1. Total pelanggan 7.043
   2. Pelanggan 425 yang diprediksi berhenti berlangganan (FP)
   3. Pendapatan setiap pelanggan (Ex Paket Basic) 1.000 USD
   4. Pendapatan setiap bulan = 7.043 x 1.000 USD = 7.043.000 USD
   5. Biaya marketing per pelanggan yang sudah ada : 10 USD
   6. Total biaya marketing untuk pelanggan yang sudah ada : 10 USD X 425 pelanggan = 4.250 USD
   7. Jika total biaya promosi yang dikeluarkan 4.250 USD, dan bisa menghasilkan pelanggan dengan membeli paket basic ada 7.043.000 USD pendapatan yang perusahaan akan terima (1.000 USD paket basic X 7.043 pelanggan) dengan laba bersih 7.038.750 USD dengan total beban promosi yang dikeluarkan sekitar 0,06% dibulan berikutnya.

### **Others Data Visualization Report**
<br>
<code><a href="https://public.tableau.com/app/profile/muhammad.al.farisy6147" target="_blank"><img height="300" src="https://github.com/mhdalfarisy/mhdalfarisy/blob/main/tol_devices_optimized.png"></a></code>
<br>

---

**💬 Ask me about anything, I'll be happy to help!** <br>
**💬 My inbox is always open, Contact me**
<br>
<br> 
  </a>
  <a href="mailto:m.alfarisy797@gmail.com">
    <img align="left" alt="Muhammad Al-farisy | Gmail" width="26px" src="https://cdn.worldvectorlogo.com/logos/official-gmail-icon-2020-.svg" />
  </a>
  <a href="https://www.linkedin.com/in/m-alfarisy97/">
    <img align="left" alt="Muhamamd Al-farisy | Instagram" width="26px" src="https://cdn.worldvectorlogo.com/logos/linkedin-icon-2.svg" />
  </a>
  <a href="https://www.instagram.com/inifaris_____/">
    <img align="left" alt="Muhammad Al-farisy | Instagram" width="24px" src="https://cdn.worldvectorlogo.com/logos/instagram-5.svg" />
  </a>
  <a href="https://public.tableau.com/app/profile/muhammad.al.farisy6147">
    <img align="left" alt="Muhammad Al-farisy | Tableau" width="24px" src="https://cdn.worldvectorlogo.com/logos/tableau-logo.svg" />
  </a>
  
<br>
<br>

⭐️ From [Muhammad Al-farisy](https://github.com/mhdalfarisy)
