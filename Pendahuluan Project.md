# Performa-Penjualan-Percabang
Perusahaan  Sedang butuh perbandingan performa dari setiap cabang di berbagai kota. ambil saja lima kota terbesar di Pulau Jawa untuk dianalisis dari segi order size, customer count, product count, brand count, dan GMV dalam basis bulanan. Tabel di pivot untuk setiap measure yang dibutuhkan, lalu mencari angkanya per bulan?”   “Benar. Sebelum saya beri deadline, dari kamu bisa selesai kapan?” tawar Andra.    “Hmmm, datanya sendiri sudah bersih atau perlu aku cleaning lagi, Ndra?” tanyaku sembari menimbang-nimbang.    “Datanya sudah bersih. Nanti akan coba saya kirimkan yang versi lengkapnya dalam tahun 2019 agar bisa kamu pertimbangkan estimasi waktu pengerjaan.”   “Oke, Ndra. Soalnya, kalau datanya sudah bersih, dua hari cukup sih. Tapi aku cek dulu deh data lengkap yang nanti dikirim.”   “Selamat bekerja, Aksara.”
Hal yang perlu dilakukan:

[1]. Load masing-masing data *.csv dengan Pandas

[2]. Pengecekan dan Transformasi Data 
      - Cek data sekilas (melihat bentuk data biasanya 5 data teratas)
      - Cek list kolom untuk semua dataframe apakah seluruh kolom dari keempat dataframe yang terpisah itu sama
        Jika sama digabungkan.
      - Cek informasi dataframe yang telah digabungkan
      - Statistik deskriptif dari dataframe yang telah digabungkan.
[3] Transformasi Data 
      - Jika ada data yang tidak seharusnya maka dapat dibuang
      - Jika ada kolom yang seharusnya bertipe datetime64 ubahlah
      - Cek kembali informasi dataframe 
      - Tampilkan kembali statistik deskriptif dari dataframe
[4]. Filter province yang hanya termasuk 5 provinsi besar di Jawa (DKI Jakarta, Jawa Barat, Jawa Tengah, Jawa Timur, dan Yogyakarta)

[5]. Mengelompokkan data berdasarkan order_date dan province yang sudah difilter dan menghitung order unique count, customer unique count, product unique count, brand unique count, dan GMV (Gross Merchandise Volume = total_price untuk semua penjualan)

[6]. Melakukan unstack untuk mendapatkan order_date di bagian baris dan province di bagian column
[7]. Slicing data untuk masing-masing measurement (kolom), misal: kolom order

[8]. Lakukan resampling pada data tersebut untuk dilakukan perhitungan secara bulanan
[9]. Plot untuk hasil pada langkah #[8]

Langah 7 s/d 9 yang telah dilakukan baru untuk satu measurement yaitu order. Berarti ada empat kali lagi kode seperti ini harus dibuat. Karena struktur code masih sama, dapat menggunakan perulangan sesuai dengan jumlah measurement yaitu 5, sehingga kelima measurement dapat ditampilkan grafiknya dalam satu canvas figure.

Mari memulai dengan membuat sebuah perulangan dengan dataframe unstack_city_province yang digunakan (hasil dari langkah ke 5 di part 2).

 
