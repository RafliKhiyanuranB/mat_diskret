
# Aljabar Boolean & Gerbang Logika

## Tujuan
- Memahami hubungan antara logika Boolean dan sirkuit komputer digital.
- Belajar cara merancang sirkuit logika sederhana.
- Memahami bagaimana sirkuit digital bekerja bersama-sama untuk membentuk sistem komputer yang kompleks.

---

## Operator Boolean
### Operator Biner
1. **Penjumlahan (+)**: Digunakan untuk operasi disjungsi (OR).
2. **Perkalian (⋅)**: Digunakan untuk operasi konjungsi (AND).

### Operator Uner
- **Komplemen (’)**: Digunakan untuk menghasilkan nilai yang berlawanan dari suatu elemen. Misalnya, jika `a = 1` maka `a' = 0`, dan sebaliknya.

---

## Manfaat dalam Pemrograman
Aljabar Boolean sering digunakan dalam pemrograman untuk mengevaluasi ekspresi logika.

## Contoh dalam Pemrograman Python
```python
a = True
b = False
result = a and b  # hasilnya adalah False
```

---

## Aksioma Aljabar Boolean
Untuk setiap `a, b, c ∈ B` berlaku aksioma-aksioma berikut:
- **Closure**: `a + b ∈ B` dan `a ⋅ b ∈ B`.
- **Identitas**: `a + 0 = a` dan `a ⋅ 1 = a`.
- **Komutatif**: `a + b = b + a` dan `a ⋅ b = b ⋅ a`.
- **Distributif**: `a ⋅ (b + c) = (a ⋅ b) + (a ⋅ c)` dan `a + (b ⋅ c) = (a + b) ⋅ (a + c)`.
- **Komplemen**: Untuk setiap `a ∈ B` terdapat elemen unik `a' ∈ B` sehingga `a + a' = 1` dan `a ⋅ a' = 0`.

---

## Aljabar Boolean
Aljabar Boolean adalah sistem matematika untuk manipulasi variabel yang dapat memiliki salah satu dari dua nilai:
- Dalam logika formal, nilai-nilai ini adalah **benar** dan **salah**.
- Dalam sistem digital, nilai-nilai ini adalah **nyala** dan **mati** (1 dan 0) atau **tinggi** dan **rendah**.

Ekspresi Boolean dibuat dengan melakukan operasi pada variabel Boolean. Operator Boolean yang umum termasuk:
- **AND (⋅)**: Konjungsi (perkalian)
- **OR (+)**: Disjungsi (penjumlahan)
- **NOT (')**: Komplemen (kebalikan nilai)

### Tabel Kebenaran
Operator Boolean dapat dijelaskan sepenuhnya menggunakan tabel kebenaran. Contoh:

#### AND
| A | B | A ⋅ B |
|---|---|-------|
| 0 | 0 |   0   |
| 0 | 1 |   0   |
| 1 | 0 |   0   |
| 1 | 1 |   1   |

#### OR
| A | B | A + B |
|---|---|-------|
| 0 | 0 |   0   |
| 0 | 1 |   1   |
| 1 | 0 |   1   |
| 1 | 1 |   1   |

### Fungsi Boolean
Sebuah fungsi Boolean memiliki:
- Setidaknya satu variabel Boolean
- Setidaknya satu operator Boolean
- Setidaknya satu input dari himpunan `{0, 1}`

Fungsi ini menghasilkan output yang juga merupakan anggota dari himpunan `{0, 1}`.

---

## Hukum dan Identitas Boolean
Berikut adalah beberapa hukum penting dalam Aljabar Boolean:
1. **Hukum Identitas**: 
   - `a + 0 = a`
   - `a ⋅ 1 = a`
   
2. **Hukum Komplemen**: 
   - `a + a' = 1`
   - `a ⋅ a' = 0`

3. **Hukum Distributif**: 
   - `a ⋅ (b + c) = (a ⋅ b) + (a ⋅ c)`
   - `a + (b ⋅ c) = (a + b) ⋅ (a + c)`

4. **Hukum DeMorgan**:
   - `a' ⋅ b' = (a + b)'`
   - `a' + b' = (a ⋅ b)'`

---

## Gerbang Logika
Fungsi Boolean diimplementasikan dalam sirkuit komputer digital yang disebut **gerbang logika**. Gerbang logika adalah perangkat elektronik yang menghasilkan hasil berdasarkan dua atau lebih nilai input. 

### Jenis Gerbang Logika
1. **Gerbang AND**: Menghasilkan `1` jika semua inputnya adalah `1`.
   - Contoh: `1 AND 0 = 0`
2. **Gerbang OR**: Menghasilkan `1` jika setidaknya satu inputnya adalah `1`.
   - Contoh: `1 OR 0 = 1`
3. **Gerbang NOT**: Menghasilkan nilai kebalikan dari input.
   - Contoh: `NOT 1 = 0`
4. **Gerbang XOR (Exclusive OR)**: Menghasilkan `1` hanya ketika nilai input berbeda.
   - Contoh: `1 XOR 0 = 1`

### Gerbang Universal
1. **Gerbang NAND**: Kebalikan dari gerbang AND.
   - Contoh: `1 NAND 1 = 0`
2. **Gerbang NOR**: Kebalikan dari gerbang OR.
   - Contoh: `1 NOR 1 = 0`

NAND dan NOR dikenal sebagai **gerbang universal** karena semua fungsi Boolean dapat diimplementasikan menggunakan gerbang-gerbang ini.

### Gerbang dengan Banyak Input
Gerbang logika dapat memiliki beberapa input dan lebih dari satu output. Output kedua bisa berupa komplemen dari operasi.

---

## Sirkuit Kombinasional
Sirkuit yang mengimplementasikan fungsi Boolean seringkali merupakan **rangkaian logika kombinasional**. Output dari sirkuit ini hanya bergantung pada nilai input saat ini, tanpa menyimpan status sebelumnya.

### Contoh: Half Adder
Salah satu rangkaian kombinasional yang sederhana adalah **Half Adder**, yang menjumlahkan dua bit.

| A | B | Sum (XOR) | Carry (AND) |
|---|---|-----------|-------------|
| 0 | 0 |     0     |      0      |
| 0 | 1 |     1     |      0      |
| 1 | 0 |     1     |      0      |
| 1 | 1 |     0     |      1      |

Rangkaian ini menggunakan:
- **XOR** untuk menemukan jumlah (sum)
- **AND** untuk menemukan carry

---

## Kesimpulan
Dengan memahami Aljabar Boolean dan gerbang logika, kita dapat merancang sirkuit digital yang kompleks, termasuk sirkuit kombinasional seperti **Half Adder**. Prinsip-prinsip ini adalah dasar dari pengoperasian sistem komputer modern.
