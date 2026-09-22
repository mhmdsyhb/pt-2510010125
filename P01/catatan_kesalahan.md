# Catatan Kesalahan Praktikum 5

## Tabel Praktikum 5

No	Berkas	Jenis Kesalahan	Pesan/Error	Penyebab	Solusi
1	k1_sintaks.cpp	Kesalahan Sintaks	uexpected ‘,’ or ‘;’ before ‘std’, unused variable ‘nilai’	Variabel telah dideklarasikan tetapi belum digunakan, serta terdapat kekurangan tanda ; pada bagian nilai = 80	Gunakan variabel tersebut dalam perhitungan atau hapus jika tidak diperlukan, kemudian tambahkan ; setelah deklarasi int nilai = 80
2	k2_nama.cpp	Kesalahan Nama Variabel	Nilai’ was not declared in this scope; did you mean ‘nilai’, ‘bonus’ was not declared in this scope	Terdapat kesalahan dalam penulisan nama variabel. Seharusnya menggunakan nilai, bukan Nilai, dan variabel bonus belum dideklarasikan	Ubah penulisan Nilai menjadi nilai dan deklarasikan variabel bonus terlebih dahulu
3	k3_runtime.cpp	Kesalahan Logika	Program melakukan pembagian dengan angka 0 ketika jumlah mahasiswa yang dimasukkan adalah 0	Program belum melakukan pengecekan terhadap kondisi jumlah_mahasiswa == 0 sebelum proses pembagian dilakukan	Periksa terlebih dahulu apakah jumlah_mahasiswa == 0 sebelum melakukan pembagian
4	k4_logika.cpp	Kesalahan Logika	Program menghasilkan pembulatan menjadi 81, sedangkan hasil yang seharusnya adalah 81.67 karena nilai dibagi dengan 3	Pembagian menggunakan bilangan bulat sehingga hasil desimal tidak ditampilkan	Gunakan 3.0 sebagai pembagi agar hasil perhitungan dapat menghasilkan nilai desimal, yaitu 81.67

Kesimpulan
Menurut saya, kesalahan logika termasuk jenis kesalahan yang cukup berbahaya karena program tetap dapat berjalan seperti biasa tanpa menampilkan pesan error, tetapi hasil yang diperoleh bisa saja tidak sesuai dengan yang seharusnya. Oleh sebab itu, tidak cukup hanya memastikan program dapat dikompilasi dan dijalankan. Hasil perhitungan serta alur logika program juga perlu diperiksa dan diuji secara teliti. 