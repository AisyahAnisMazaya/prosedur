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

2. Source code ini adalah program Golang yang bertujuan untuk menentukan pemenang dari suatu kompetisi berdasarkan skor yang diperoleh dari setiap peserta. Program ini memiliki beberapa fungsi yang dijelaskan sebagai berikut;

- Fungsi hitungSkor Fungsi ini menerima dua parameter, yaitu waktu (array integer yang berisi waktu tempuh setiap peserta) dan skor (pointer ke integer). Fungsi ini digunakan untuk menghitung total skor yang diperoleh setiap peserta. Algoritma yang digunakan adalah:
Untuk setiap waktu dalam array waktu, jika waktu kurang dari atau sama dengan 300 detik, maka skor ditambah 1.
Skor akhir disimpan ke pointer skor.

- Fungsi cariPemenang Fungsi ini menerima empat parameter, yaitu peserta (map yang berisi nama peserta dan array waktu tempuhnya), pemenang (pointer ke string), maxSoal (pointer ke integer), dan minskor (pointer ke integer). Fungsi ini digunakan untuk menentukan pemenang berdasarkan skor tertinggi dan jumlah soal yang diselesaikan. Algoritma yang digunakan adalah:
Fungsi ini beriterasi melalui setiap peserta di map peserta.
Untuk setiap peserta, fungsi ini memanggil fungsi hitungSkor untuk menghitung total skor.
Jika skor peserta lebih besar dari skor maxSoal atau (skor sama dengan maxSoal dan jumlah soal yang diselesaikan lebih banyak), maka pemenang diubah menjadi nama peserta, maxSoal diubah menjadi skor peserta, dan minskor diubah menjadi jumlah soal yang diselesaikan.

- Fungsi main Fungsi ini adalah fungsi utama yang menjalankan program. Algoritma yang digunakan adalah:
Fungsi ini membuat map peserta yang menyimpan data nama peserta dan array waktu tempuhnya.
Fungsi ini meminta input nama peserta dan array waktu tempuhnya dari pengguna.
Fungsi ini memanggil fungsi cariPemenang untuk menentukan pemenang.
Fungsi ini mencetak nama pemenang, jumlah soal yang diselesaikan, dan total waktu tempuh.
Secara keseluruhan, program ini dirancang untuk menentukan pemenang kompetisi berdasarkan skor yang diperoleh dari setiap peserta. Skor dihitung berdasarkan waktu tempuh setiap peserta dan pemenang ditentukan berdasarkan skor tertinggi dan jumlah soal yang diselesaikan.

3. Penjelasan Kode:
- Deklarasi Paket:
package main : Menyatakan bahwa kode program ini adalah program utama yang akan dieksekusi.

- Import Library:
import ("fmt") : Mengimpor library fmt yang digunakan untuk mencetak ke layar konsol.

- Fungsi cetakDeret(n int):
Fungsi ini menerima satu parameter integer n, yang mewakili nilai awal deret Collatz.
Fungsi ini menggunakan loop for untuk iterasi sampai nilai n menjadi 1.
Di dalam loop:
fmt.Printf("%d ", n) : Mencetak nilai n ke layar konsol, diikuti dengan spasi.
if n%2 == 0 : Mengecek apakah n adalah bilangan genap.
Jika ya, n = n/2 : Nilai n dibagi dengan 2.
else : Jika n ganjil.
n = 3*n + 1 : Nilai n dikalikan dengan 3 dan ditambah 1.
Setelah loop selesai, fmt.Printf("1\n") : Mencetak "1" di layar konsol, yang merupakan nilai akhir deret Collatz.

- Fungsi main():
Fungsi ini merupakan fungsi utama yang akan dieksekusi ketika program dijalankan.
var n int : Mendeklarasikan variabel n sebagai integer, yang akan menyimpan nilai awal deret Collatz yang diinputkan oleh pengguna.
fmt.Print("Masukkan nilai suku awal: ") : Mencetak pesan ke layar konsol, meminta pengguna untuk memasukkan nilai awal deret Collatz.
fmt.Scan(&n) : Membaca nilai input dari pengguna dan menyimpannya ke variabel n.
`if n > 0 && n < 10000
