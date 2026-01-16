# Daegu Apartment Price Prediction with Machine Learning Analysis
## 🔎 Latar Belakang
Menentukan harga jual apartemen merupakan tantangan bagi pemilik maupun pembeli.
Pemilik ingin menetapkan harga yang kompetitif agar unit cepat terjual tanpa kehilangan potensi keuntungan yang maksimal, sementara pembeli ingin memastikan harga yang dibayar sesuai dengan nilai pasar bahkan ingin mencari peluang untuk dapat menemukan harga unit dibawah harga pasar.
Untuk menjawab kebutuhan tersebut, project ini memanfaatkan Machine Learning, khususnya Linear Regression, guna menemukan pola faktor-faktor yang memengaruhi harga apartemen di Korea Selatan.
Dataset mencakup berbagai karakteristik unit seperti lokasi, jenis koridor, jarak ke stasiun subway, fasilitas sekitar, tahun pembangunan, serta ukuran unit.
________________________________________

## ⚙️ Data dari Dataset:
- **Hallway Type**: Tipe koridor apartemen, terdapat 3 tipe koridor dalam apartemen yaitu **Terraced, Mixed, Corridor**, dengan paling banyak jenis apartemennya adalah **Terraced**.
- **TimeToSubway**: Waktu yang dibutuhkan untuk mencapai stasiun subway terdekat, terdapat 3 kelompok waktu yaitu **0-5min, 10min~15min, 15min~20min, 5min~10min, no_bus_stop_nearby**, dengan paling banyak apartemen menawarkan fasilitas **0-5min** untuk ke stasiun subway terdekat.
- **SubwayStation**: Nama stasiun subway terdekat, terdapat 8 stasiun subway yaitu **Kyungbuk_uni_hospital, Chil-sung-market, Bangoge, Sin-nam, Banwoldang, no_subway_nearby, Myung-duk, Daegu**, Lokasi apartemen paling banyak ada di sekitar stasiun subway **Myung-duk**.
- **N_FacilitiesNearBy (ETC)**: Jumlah fasilitas umum di sekitar apartemen, yaitu dari **0 (tidak ada) sampai jumlah fasilitas yang paling banyak ada di 5**.
- **N_FacilitiesNearBy (PublicOffice)**: Jumlah fasilitas kantor pemerintahan di sekitar apartemen, yaitu dari **0 (tidak ada) sampai paling banyak fasilitas kantor pemerintahan di sekitar apartemen adalah 7**.
- **N_SchoolNearBy (University)**: Jumlah universitas di sekitar apartemen, yaitu dari **0 (tidak ada) sampai paling banyak jumlah universitas di sekitar apartemen adalah 5**.
- **N_Parkinglot (Basement)**: Jumlah tempat parkir di basement, yaitu dari **0 (tidak ada) sampai paling banyak ada terdapat 1321 slot parkir**.
- **YearBuilt**: Tahun pembangunan apartemen, yaitu paling lama adalah bangunan yang dibangun pada tahun **1978** dan bangunan paling baru dibangun pada tahun **2015**.
- **N_FacilitiesInApt**: Jumlah fasilitas yang tersedia di dalam apartemen, yaitu **paling sedikit ada 1** dan **paling banyak ada 10 jenis fasilitas**.
- **Size (sqft)**: Luas apartemen (dalam kaki persegi), dengan apartemen yang **luas paling kecil adalah 135 sqf** dan **paling luas adalah 2337 sqf**.
- **SalePrice**: Harga jual apartemen (Won), dimana apartemen **paling murah seharga 32,743 won** dan **paling mahal seharga 585,840 won**.
________________________________________

## 📊 Model yang Digunakan
1.	Model IA — Multiple Linear Regression (HallwayType & SubwayStation → Binary Encoding)
2.	Model IB — Multiple Linear Regression (HallwayType & SubwayStation → Ordinal Encoding, berdasarkan harga minimum)
3.	Model II — Simple Linear Regression (Hanya menggunakan fitur Size (sqf))
________________________________________

## 🎯 Evaluasi Model
Metode evaluasi yang digunakan:
•	R-squared (R²) → seberapa besar variasi harga dapat dijelaskan model
•	RMSE → besar error prediksi dalam satuan Won
•	RMSPE → error prediksi dalam persentase
Selain itu dilakukan eksperimen dengan:
•	Scaling
•	Ridge Regression
•	Lasso Regression
________________________________________
*📌 Daegu Apartment Price Prediction with Machine Learning Analysis - Vivi Novela*
