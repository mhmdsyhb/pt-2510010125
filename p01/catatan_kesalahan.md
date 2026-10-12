# Catatan Kesalahan Praktikum 5

## Ringkasan Belajar dari Error

1. `k1_sintaks.cpp`
   - Kategori: Error Sintaks
   - Masalah: `expected ',' or ';' before 'std'` dan `unused variable 'nilai'`
   - Penyebab: deklarasi `int nilai = 80` tidak diakhiri tanda titik koma, lalu variabel itu tidak dipakai lagi dalam proses program
   - Solusi: tambahkan `;` setelah deklarasi, lalu gunakan variabel tersebut dalam perhitungan atau hapus jika memang tidak diperlukan

2. `k2_nama.cpp`
   - Kategori: Error Penamaan Variabel
   - Masalah: `'Nilai' was not declared in this scope; did you mean 'nilai'` dan `'bonus' was not declared in this scope'`
   - Penyebab: nama variabel tidak konsisten, dan `bonus` dipakai sebelum dideklarasikan
   - Solusi: pakai nama variabel yang seragam di seluruh kode dan deklarasikan `bonus` sebelum penggunaannya

3. `k3_runtime.cpp`
   - Kategori: Error Logika (Runtime)
   - Masalah: pembagian dengan nol terjadi saat jumlah mahasiswa bernilai 0
   - Penyebab: program tidak validasi input sebelum melakukan operasi pembagian
   - Solusi: cek `jumlah_mahasiswa == 0` sebelum menghitung rata-rata, lalu beri peringatan atau hentikan eksekusi

4. `k4_logika.cpp`
   - Kategori: Error Logika
   - Masalah: hasil output menjadi `81`, padahal seharusnya `81.67`
   - Penyebab: pembagian memakai angka `3` bertipe integer, sehingga hasilnya ikut dibulatkan
   - Solusi: ubah pembagi menjadi `3.0` agar hasil perhitungan tetap presisi

## Kesimpulan Singkat

Error logika adalah jenis kesalahan yang paling berbahaya karena program tetap bisa berjalan tanpa menampilkan pesan error, tetapi hasil akhirnya tetap salah. Sementara error sintaks dan penamaan biasanya langsung terlihat saat kompilasi, error logika baru ditemukan saat kita mengecek hasil akhir dan membandingkannya dengan logika yang benar. Oleh karena itu, debugging tidak cukup hanya sampai program bisa dicompile; kita juga harus mengecek alur dan outputnya secara cermat.
