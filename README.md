# Project-Analysis-NYC-TLC
---
- Nama: Muhammad Umar Abdul Aziz
- Program: Job Connector Data Science and Machine Learning
- Batch: JCDS-0608 BDG
- Tableau Story link: https://public.tableau.com/app/profile/muhammad.umar1667/viz/NYCTLCAnalysis_17442109659040/Sumarry?publish=yes
---
## Abstrak

Penelitian ini bertujuan untuk menganalisis data perjalanan taksi di bawah pengelolaan New York City Taxi and Limousine Commission (NYC TLC) guna mengidentifikasi pola operasional, perilaku penumpang, dan faktor-faktor yang memengaruhi kualitas layanan. Analisis dilakukan terhadap distribusi perjalanan berdasarkan waktu dan lokasi, hubungan antara metode pembayaran dengan tip, pengaruh jenis perjalanan terhadap performa layanan, serta deteksi anomali data. Hasil analisis menunjukkan bahwa aktivitas taksi meningkat signifikan pada jam sibuk dan hari kerja, dengan lokasi populer seperti bandara dan pusat kota sebagai titik konsentrasi tertinggi. Pembayaran non-tunai cenderung menghasilkan tip yang lebih tinggi, sedangkan variasi tip rate antarwilayah dapat mencerminkan tingkat kepuasan pelanggan. Ditemukannya data anomali juga mengindikasikan perlunya validasi berkala terhadap sistem pencatatan. Temuan ini memberikan dasar bagi NYC TLC untuk meningkatkan efisiensi operasional, strategi alokasi armada, serta pengembangan kebijakan layanan yang berbasis data.
---
## Deskipsi Data

VendorID - ID penyedia layanan taksi. Biasanya:

- 1 = Creative Mobile Technologies (CMT)
- 2 = VeriFone Inc.

lpep_pickup_datetime - Waktu penjemputan penumpang.

lpep_dropoff_datetime - Waktu penurunan penumpang.

store_and_fwd_flag - Indikator apakah data perjalanan sementara disimpan sebelum dikirim ke server:

- Y = Data disimpan sementara.
- N = Data dikirim langsung ke server.

RatecodeID - Kode tarif yang digunakan dalam perjalanan:

- 1 = Tarif standar.
- 2 = Tarif perjalanan ke bandara JFK.
- 3 = Tarif perjalanan ke bandara Newark.
- 4 = Perjalanan dengan tarif yang dinegosiasikan sebelumnya.
- 5 = Tarif perjalanan gratis.
- 6 = Perjalanan ke luar kota yang telah ditentukan tarifnya.

PULocationID - ID lokasi penjemputan (berdasarkan zona taksi NYC).

DOLocationID - ID lokasi tujuan penumpang (berdasarkan zona taksi NYC).

passenger_count - Jumlah penumpang dalam perjalanan.

trip_distance - Jarak perjalanan dalam mil.

fare_amount - Tarif dasar perjalanan dalam dolar.

extra - Biaya tambahan, seperti:

- 1.00 = Tambahan biaya perjalanan malam hari (20:00 - 06:00).
- 0.50 = Biaya tambahan jam sibuk.

mta_tax - Pajak Metro Transit Authority (MTA) sebesar $0.50 per perjalanan.

tip_amount - Jumlah tip yang diberikan penumpang (jika pembayaran non-tunai).

tolls_amount - Jumlah biaya tol selama perjalanan.

ehail_fee - Biaya pemesanan elektronik (biasanya NaN untuk taksi reguler).

improvement_surcharge - Biaya tambahan per perjalanan ($0.30).

total_amount - Total biaya perjalanan termasuk tarif, pajak, tol, dan tip.

payment_type - Jenis pembayaran:

- 1 = Kartu kredit.
- 2 = Tunai.
- 3 = Tanpa biaya (misalnya perjalanan promosi).
- 4 = Dispute (pembayaran dipermasalahkan).
- 5 = Pembayaran lain.
- 6 = Voided trip (perjalanan yang dibatalkan).

trip_type - Jenis perjalanan:

- 1 = Perjalanan reguler.
- 2 = Perjalanan yang dipesan sebelumnya (dispatch).

congestion_surcharge - Biaya kemacetan ($2.75 per perjalanan, berlaku untuk perjalanan di Manhattan).
