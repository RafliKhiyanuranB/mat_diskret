---
title: Algoritma

---

# Algoritma 

## Definisi Algoritma
Algoritma adalah urutan dari sejumlah langkah logis dan sistematis untuk memecahkan suatu masalah tertentu.

Pada pemrograman, algoritma didefinisikan sebagai metode yang terdiri dari langkah-langkah terstuktur untuk mencari solusi suatu masalah dengan bantuan komputer.

## Algorithm Sequential Search
Sequential search adalah teknik pencarian data yang dilakukan dengan cara membandingkan setiap elemen data satu per satu, mulai dari elemen pertama hingga elemen yang dicari ditemukan. Proses ini terus berlanjut hingga data ditemukan atau seluruh elemen telah diperiksa.

Algoritma ini termasuk salah satu algoritma pencarian yang paling sederhana dan sering digunakan dalam situasi di mana data tidak memiliki struktur tertentu.

contoh:
1. Masukkan kata kunci
2. Mulai dari awal atau akhir, cek seluruh record dalam array atau list
3. Baca satu persatu berdasarkan key yang dicari
4. Jika sampai akhir pengulangan data tidak ada yang sama, maka data tidak ditemukan 

## Algoritma Binary Search
Sebuah algoritme pencarian biner (atau pemilahan biner) adalah sebuah teknik untuk menemukan nilai tertentu dalam sebuah larik (array) linear, dengan menghilangkan setengah data pada setiap langkah, dipakai secara luas tetapi tidak secara ekslusif dalam ilmu komputer. Sebuah pencarian biner mencari nilai tengah (median), melakukan sebuah pembandingan untuk menentukan apakah nilai yang dicari ada sebelum atau sesudahnya, kemudian mencari setengah sisanya dengan cara yang sama.

contoh:
1. Tetapkan penunjuk awal dengan 0, dan penunjuk akhir dengan indeks terakhir dari array
2. Tetapkan variabel mid, yang merujuk ke tengah array
3. Variabel ini dihitung sebagai (rendah+tinggi)/2
4. Jika elemen pada indeks tengah sama dengan elemen yang dicari, kembalikan indeks tengah 


## Pseudocode
Pseudocode adalah cara penulisan kode dan algoritma menggunakan bahasa umum yang digunakan sehari-hari sehingga lebih mudah dipahami. Karena itu pseudocode juga disebut sebagai false code atau representation code.


## Big O algoritma
 Big-O adalah cara untuk mengekspresikan kompleksitas waktu (atau ruang) suatu algoritma.
 
## Hitung Big O dari Algorithm Sequential Search 
 * Waktu kompleksitas ( time complexity)
    Time complexity adalah ukuran seberapa lama waktu yang dibutuhkan suatu algoritma untuk berjalan, berdasarkan ukuran input. Hal ini dinyatakan menggunakan notasi Big-O, yang memberikan perkiraan kasar waktu berjalan. Suatu algoritma dengan kompleksitas waktu yang lebih rendah umumnya akan lebih cepat daripada suatu algoritma dengan kompleksitas waktu yang lebih tinggi.

 * Ruang kompleksitas ( space komplexity)
    Space komplexity adalah ukuran seberapa banyak memori yang dibutuhkan suatu algoritma, berdasarkan ukuran input. Seperti kompleksitas waktu, kompleksitas ruang dinyatakan menggunakan notasi Big-O. Algoritma dengan kompleksitas ruang yang lebih rendah umumnya akan membutuhkan lebih sedikit memori daripada algoritma dengan kompleksitas ruang yang lebih tinggi.
    
## reference
1. https://binus.ac.id/malang/2017/09/pengenalan-algoritma/
2. https://fikti.umsu.ac.id/algoritma-sequential-search-pengertian-fungsi-dan-cara-kerjanya/
3. https://id.wikipedia.org/wiki/Algoritma_pencarian_biner
4. https://revou.co/kosakata/pseudocode
5. https://www.designgurus.io/blog/big-o-algorithm-complexity