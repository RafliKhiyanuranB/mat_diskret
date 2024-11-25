---
title: Deretan dan Rekursi

---

### Deretan dan Rekursi
#### Pengertian Deretan (*sequence*)
**Deretan** adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu
**Definisinya** yaitu Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

N = {1, 2, 3, 4,}
S misalnya {2,4,6,8}, {1/3,1/5,1/7}

**Notasi Deretan** : {an}
**Deretan** umumnya dinyatakan dalam suatu formula, misalnya:
	an = 2n
	an = 1/n
	an = 7 – 3n
    
Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.

#### Contoh-contoh Deretan
***Deret Aritmetika***
Deret dengan pola kenaikan atau penurunan tetap.
- Contoh: 2,5,8,11,14,...
- Rumus suku ke-n:
![Screenshot 2024-11-23 214020](https://hackmd.io/_uploads/BJ2DFw1Qkx.png)
Di mana:
- 𝑎: suku pertama 
- 𝑏: beda (selisih antar suku
- 𝑛: nomor suku yang dicari

***Deret Geometri***
Deret dengan pola kelipatan tetap.
- Contoh: 3,6,12,24,48,…
- Rumus suku ke-n:
![Screenshot 2024-11-23 214239](https://hackmd.io/_uploads/H1zeqv1X1l.png)
Di mana:
- 𝑎: suku pertama 
- 𝑟: rasio (perbandingan antar suku,
- 𝑛: nomor suku yang dicari

***Deret Bilangan Kuadrat***
Deret dengan pola nilai berupa kuadrat bilangan bulat.
- Contoh: 1,4,9,16,25,…
- - Rumus suku ke-n:
![Screenshot 2024-11-23 214619](https://hackmd.io/_uploads/H1H0cDkQkl.png)

***Deret Bilangan Kubik***
Deret dengan pola nilai berupa kubik bilangan bulat.
- Contoh: 1,8,27,64,125,…
- Rumus suku ke-n:
![Screenshot 2024-11-23 214742](https://hackmd.io/_uploads/Hk-Qovy7ke.png)

***Deret Fibonacci***
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
- Contoh: 0,1,1,2,3,5,8,…
- Rumus suku ke-n (rekursif):
![Screenshot 2024-11-23 214844](https://hackmd.io/_uploads/ryA8jvk71x.png)


#### Penjumlahan Deretan
Jumlah Deretan 
![Screenshot 2024-11-23 215027](https://hackmd.io/_uploads/rkL0sPym1g.png)
adalah
![Screenshot 2024-11-23 215043](https://hackmd.io/_uploads/ByNk3Pk7yl.png)
atau dalam notasi sumasi:
![Screenshot 2024-11-23 215124](https://hackmd.io/_uploads/S1pghvk71e.png)
    k adalah indeks summasi, 
    m adalah batas bawah indeks,
    n adalah batas atas indeks
    
#### Pengertian Rekursi 
Rekursi adalah Sebuah objek dikatakan rekursif  (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri.Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).

***Fungsi Rekursi***
Fungsi rekursif didefinisikan oleh dua bagian : 
* **Basis**
Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit.Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
* **Rekurens**
Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri.Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil.
**Contoh**
Misalkan f didefinsikan secara rekusif sbb
![Screenshot 2024-11-23 215825](https://hackmd.io/_uploads/HJBoav1Xyg.png)
Tentukan nilai f(4)!
Solusi:      f(4) = 2f(3) + 4 
			=  2(2f(2) + 4) + 4
			=  2(2(2f(1) + 4) + 4) + 4
			=  2(2(2(2f(0) + 4) + 4) + 4) + 4
			=  2(2(2(23 + 4) + 4) + 4) + 4	
			=  2(2(2(10) + 4) + 4) + 4
			=  2(2(24) + 4) + 4
			=  2(52) + 4
			= 108	

***Struktur Rekursif***
Struktur data yang penting dalam komputer adalah pohon biner (binary tree). 
![Screenshot 2024-11-23 220101](https://hackmd.io/_uploads/HylrCvJQ1e.png)
* Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.
* Jumlah anak pada setiap simpul bisa 1, 2, atau 0.
* Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node)
* Simpul yang tidak mempunyai anak disebut simpul daun (leave).









