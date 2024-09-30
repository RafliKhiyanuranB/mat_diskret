## 1. Hukum De Morgan dalam Teori Himpunan

Hukum De Morgan terdiri dari dua aturan utama:

1. **Komplemen dari Irisan (Intersection)**:
   \[
   (A \cap B)^c = A^c \cup B^c
   \]
   
   **Penjelasan**: Komplemen dari irisan dua himpunan adalah himpunan elemen yang bukan anggota dari kedua himpunan tersebut, yaitu anggota yang berada di luar A atau B. Hasilnya sama dengan gabungan dari komplemen masing-masing himpunan.

2. **Komplemen dari Gabungan (Union)**:
   \[
   (A \cup B)^c = A^c \cap B^c
   \]

   **Penjelasan**: Komplemen dari gabungan dua himpunan adalah himpunan elemen yang tidak ada di salah satu himpunan tersebut. Ini sama dengan irisan dari komplemen himpunan A dan B.



### Contoh Soal: Pembuktian Hukum De Morgan

Misalkan kita memiliki dua himpunan:
- A = {1, 2, 3, 4}
- B = {3, 4, 5, 6}

Serta semesta (U) adalah:
- U = {1, 2, 3, 4, 5, 6, 7, 8}

#### Membuktikan Hukum 1: \((A \cap B)^c = A^c \cup B^c\)

**Langkah-langkah:**

1. **Irisan A dan B (A ∩ B)**:
   \[
   A \cap B = \{3, 4\}
   \]

2. **Komplemen dari A ∩ B ((A ∩ B)^c)**:
   \[
   (A \cap B)^c = U - \{3, 4\} = \{1, 2, 5, 6, 7, 8\}
   \]

3. **Komplemen A (A^c) dan Komplemen B (B^c)**:
   - A^c: Elemen di semesta U yang tidak ada di A:
     \[
     A^c = U - A = \{5, 6, 7, 8\}
     \]
   - B^c: Elemen di semesta U yang tidak ada di B:
     \[
     B^c = U - B = \{1, 2, 7, 8\}
     \]

4. **Gabungan dari Komplemen A dan B (A^c ∪ B^c)**:
   \[
   A^c \cup B^c = \{5, 6, 7, 8\} \cup \{1, 2, 7, 8\} = \{1, 2, 5, 6, 7, 8\}
   \]

5. **Hasil**:
   \[
   (A \cap B)^c = A^c \cup B^c = \{1, 2, 5, 6, 7, 8\}
   \]

   Ini membuktikan bahwa Hukum 1 benar.



#### Membuktikan Hukum 2: \((A \cup B)^c = A^c \cap B^c\)

**Langkah-langkah:**

1. **Gabungan A dan B (A ∪ B)**:
   \[
   A \cup B = \{1, 2, 3, 4, 5, 6\}
   \]

2. **Komplemen dari A ∪ B ((A ∪ B)^c)**:
   \[
   (A \cup B)^c = U - \{1, 2, 3, 4, 5, 6\} = \{7, 8\}
   \]

3. **Komplemen A (A^c) dan Komplemen B (B^c)**:
   - A^c: \(\{5, 6, 7, 8\}\)
   - B^c: \(\{1, 2, 7, 8\}\)

4. **Irisan dari Komplemen A dan B (A^c ∩ B^c)**:
   \[
   A^c \cap B^c = \{5, 6, 7, 8\} \cap \{1, 2, 7, 8\} = \{7, 8\}
   \]

5. **Hasil**:
   \[
   (A \cup B)^c = A^c \cap B^c = \{7, 8\}
   \]

   Ini membuktikan bahwa Hukum 2 benar.



### Kesimpulan:
Hukum De Morgan mempermudah perhitungan operasi himpunan yang melibatkan komplemen, irisan, dan gabungan. Hukum ini berguna dalam berbagai bidang matematika dan ilmu komputer, terutama dalam logika dan pemrograman.

---

## 2. Absorption Laws dalam Teori Himpunan

**Absorption Law** dalam teori himpunan menyederhanakan operasi gabungan (union) dan irisan (intersection). Terdapat dua bentuk dari hukum ini:

### 1. **Hukum Absorpsi untuk Gabungan (Union)**
\[
A \cup (A \cap B) = A
\]
Artinya, jika kita melakukan operasi gabungan antara himpunan \(A\) dan hasil dari irisan \(A\) dengan \(B\), hasil akhirnya adalah himpunan \(A\).

### 2. **Hukum Absorpsi untuk Irisan (Intersection)**
\[
A \cap (A \cup B) = A
\]
Artinya, jika kita melakukan operasi irisan antara himpunan \(A\) dan hasil dari gabungan \(A\) dengan \(B\), hasil akhirnya adalah himpunan \(A\).


## Contoh Soal dan Pembuktian

### Contoh 1: Hukum Absorpsi untuk Gabungan (Union)

Misalkan kita punya dua himpunan:
\[
A = \{1, 2, 3\}, \quad B = \{2, 3, 4\}
\]

Mari kita buktikan bahwa:
\[
A \cup (A \cap B) = A
\]

#### Langkah-langkah:
1. **Cari Irisan \(A \cap B\)**:
   \[
   A \cap B = \{2, 3\}
   \]
   Karena \(2\) dan \(3\) ada di kedua himpunan \(A\) dan \(B\).

2. **Gabungkan \(A\) dengan \(A \cap B\)**:
   \[
   A \cup (A \cap B) = \{1, 2, 3\} \cup \{2, 3\} = \{1, 2, 3\}
   \]

3. **Kesimpulan**:
   Hasil akhirnya adalah \(A\), sehingga hukum absorsi untuk gabungan terbukti benar.


### Contoh 2: Hukum Absorpsi untuk Irisan (Intersection)

Sekarang, mari kita buktikan bahwa:
\[
A \cap (A \cup B) = A
\]

#### Langkah-langkah:
1. **Cari Gabungan \(A \cup B\)**:
   \[
   A \cup B = \{1, 2, 3, 4\}
   \]

2. **Cari Irisan antara \(A\) dan \(A \cup B\)**:
   \[
   A \cap (A \cup B) = \{1, 2, 3\} \cap \{1, 2, 3, 4\} = \{1, 2, 3\}
   \]

3. **Kesimpulan**:
   Hasil akhirnya adalah \(A\), sehingga hukum absorsi untuk irisan terbukti benar.


## Penjelasan Intuitif
- **Hukum Absorpsi untuk Gabungan** menyatakan bahwa jika kita sudah memiliki seluruh elemen dari \(A\), maka menambahkan bagian \(A \cap B\) tidak akan mengubah hasil, karena \(A\) sudah mencakup semua elemen tersebut.
- **Hukum Absorpsi untuk Irisan** menyatakan bahwa ketika kita mencari irisan dari \(A\) dengan gabungan \(A\) dan \(B\), himpunan \(A\) sudah sepenuhnya terdapat di dalam gabungan tersebut, sehingga hasilnya tetap \(A\).

Hukum ini sangat berguna dalam menyederhanakan ekspresi himpunan dalam banyak kasus.

---

## Complement Laws dalam Teori Himpunan

**Complement Laws** menggambarkan hubungan antara suatu himpunan dengan komplemennya. Ada dua hukum utama:

### 1. **Komplemen dari Himpunan Semesta (Universal Set) adalah Himpunan Kosong**
   \[
   A \cup A^c = U
   \]
   Himpunan **A** gabung komplemen **A** sama dengan himpunan semesta **U**.

### 2. **Komplemen dari Himpunan itu Sendiri adalah Himpunan Kosong**
   \[
   A \cap A^c = \emptyset
   \]
   Himpunan **A** irisan dengan komplemen **A** adalah himpunan kosong.

### Bukti dengan Contoh Soal

#### Misalkan:
- Himpunan Semesta (U) = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
- Himpunan A = {1, 2, 3, 4, 5}
- Komplemen dari A (A^c) = {6, 7, 8, 9, 10}

#### Contoh 1: **Komplemen dari Gabungan (Union)**
Buktikan bahwa:  
\[
A \cup A^c = U
\]

**Langkah 1:**  
Gabungkan himpunan **A** dan komplemennya **A^c**:
- A = {1, 2, 3, 4, 5}
- A^c = {6, 7, 8, 9, 10}

**Langkah 2:**  
Lakukan operasi gabungan (union):
\[
A \cup A^c = \{1, 2, 3, 4, 5\} \cup \{6, 7, 8, 9, 10\} = \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\}
\]

Hasilnya adalah himpunan semesta **U**, yang membuktikan hukum:
\[
A \cup A^c = U
\]

#### Contoh 2: **Komplemen dari Irisan (Intersection)**
Buktikan bahwa:  
\[
A \cap A^c = \emptyset
\]

**Langkah 1:**  
Iriskan himpunan **A** dan komplemennya **A^c**:
- A = {1, 2, 3, 4, 5}
- A^c = {6, 7, 8, 9, 10}

**Langkah 2:**  
Lakukan operasi irisan (intersection):
\[
A \cap A^c = \{1, 2, 3, 4, 5\} \cap \{6, 7, 8, 9, 10\} = \emptyset
\]

Hasilnya adalah himpunan kosong **∅**, yang membuktikan hukum:
\[
A \cap A^c = \emptyset
\]

### Kesimpulan:
- **Komplemen dari gabungan himpunan dan komplemennya** akan selalu menghasilkan himpunan semesta.
- **Komplemen dari irisan himpunan dan komplemennya** akan selalu menghasilkan himpunan kosong.


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











































