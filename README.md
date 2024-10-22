1. Penjelasan Program
-  Paket dan Impor
Program dimulai dengan deklarasi 'package main' , yang menunjukkan bahwa ini adalah program yang dapat dieksekusi.
Paket 'fmt' diimpor untuk melakukan operasi input/output yang terformat.

-  Fungsi Faktorial ('faktorial')
Fungsi ini menghitung nilai faktorial dari suatu bilangan bulat 'n' dan menyimpan hasilnya di variabel yang ditunjuk oleh 'hasil' .
Prosesnya dimulai dengan menginisialisasi 'hasil' menjadi 1, kemudian mengalikan 'hasil' dengan setiap bilangan dari 1 hingga 'n' .

- Fungsi Permutasi ('permutasi')
Fungsi ini menghitung jumlah permutasi dari 'n' item yang diambil 'r' pada satu waktu dengan rumus: [ P(n, r) = \frac{n!}{(n-r)!} ]
Fungsi ini memanggil 'faktorial' untuk mendapatkan nilai faktorial dari 'n' dan 'n-r' .

-  Fungsi Kombinasi ('kombinasi')
Fungsi ini menghitung jumlah kombinasi dari 'n' item yang diambil 'r'  pada satu waktu dengan rumus: [ C(n, r) = \frac{n!}{r! \cdot (n-r)!} ]
Sama seperti fungsi permutasi, fungsi ini juga memanggil 'faktorial' untuk menghitung nilai faktorial yang diperlukan.

-  Fungsi Utama ('main')
Fungsi ini membaca empat bilangan bulat dari pengguna: 'a' , 'b' , 'c' , dan 'd'. 
Program memeriksa apakah 'a >= c' dan 'b >= d' untuk memastikan bahwa input valid untuk menghitung permutasi dan kombinasi.
Jika valid, program menghitung permutasi dan kombinasi untuk pasangan (a, c) dan (b, d).
Hasil dari perhitungan tersebut dicetak ke layar.

- Contoh Penggunaan
Misalnya, jika pengguna memasukkan 5 3 2 1, program akan:
Menghitung permutasi dan kombinasi untuk 5 diambil 2 dan 3 diambil 1.

- Peningkatan yang Dapat Dilakukan
Validasi Input: Tambahkan penanganan kesalahan untuk input yang tidak valid (misalnya, bilangan negatif).
Efisiensi: Untuk nilai n yang lebih besar, pertimbangkan menggunakan metode iteratif atau memoization untuk mengoptimalkan perhitungan faktorial.
Format Output: Mungkin perlu memformat output agar lebih jelas dan mudah dibaca.

2. 
