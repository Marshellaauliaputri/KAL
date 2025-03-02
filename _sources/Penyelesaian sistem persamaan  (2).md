---
title: 'Penyelesaian sistem persamaan '

---

## Penyelesaian sistem persamaan linear 
### operasi baris elementer
Operasi Baris Elementer(0BE) adalah serangkaian manipulasi aljabar yang dilakukan pada baris matriks dengan tujuan menyelesaikan sistem persamaan linear, mencari invers matriks, atau menentukan determinan. 
## jenis jenis operasi baris elementer
1. Pertukaran Baris (Swapping Rows)
Menukar posisi dua baris dalam matriks. Operasi ini dinotasikan sebagai *Ri↔Rj* yang berarti baris ke-i ditukar dengan baris ke-j
2. Perkalian Baris dengan Konstanta Tak Nol
Mengalikan semua elemen dalam satu baris dengan suatu bilangan bukan nol.Operasi ini dinotasikan sebagai Ri→kRi dimana k≠0 berarti semua elemen di baris kedua dikalikan dengan 2.
3. Penjumlahan satu baris dengan konstanta non-Nol dengan baris yang lain.Menambahkan atau mengurangi kelipatan suatu baris ke baris lain. Operasi ini dinotasikan sebagai 
Ri→Ri+kRj,berarti baris kedua dikurangi 3 kali baris pertama.

### eleminasi gaus 
Eliminasi Gauss adalah metode sistematis untuk menyelesaikan sistem persamaan linear dengan menggunakan operasi baris elementer. Eliminasi Gauss digunakan untuk menyelesaikan sistem persamaan linear dengan mengubah matriks koefisien menjadi bentuk yang lebih sederhana. Berikut langkah-langkahnya:

1. Matriks Augmented: Pertama, sistem persamaan linear dituliskan dalam bentuk matriks teraugmentasi, yang menggabungkan koefisien variabel dengan hasil persamaan.

2. Operasi Baris Elementer: Tiga jenis operasi baris elementer diterapkan:

* Pertukaran Baris: Menukar posisi dua baris.

* Penskalaan Baris: Mengalikan semua elemen dalam suatu baris dengan bilangan konstan tak nol.

* Penggantian Baris: Menjumlahkan kelipatan satu baris ke baris lainnya.

3. Bentuk Eselon Baris: Tujuan dari eliminasi adalah untuk mengubah matriks menjadi bentuk eselon baris, di mana setiap baris memiliki lebih banyak nol di sebelah kiri dibandingkan dengan baris di atasnya.

4. Substitusi Balik: Setelah mencapai bentuk eselon baris, nilai dari variabel dapat ditemukan melalui substitusi balik, dimulai dari variabel terakhir hingga variabel pertama.



Contoh Soal 1
Selesaikan dengan menggunakan eliminasi gaus
$$
\begin{array}{cc}
x_1 + 2x_2 + 3x_3 =6\\
2x_1+ 4x_2 + 6x_3 =12\\
x_3+x_2 = 2\\
\end{array}
$$
Penyelesaiannya:

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
2 & 4 & 6 & | &12\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 0 & 0 & | &0\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 1 & 1 & | &2\\
0 & 0 & 0 & | &0\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 0 & 1 & | &2\\
0 & 1 & 1 & | &2\\
0 & 0 & 0 & | &0\\
\end{bmatrix}
\quad
$$

$$
\begin{array}{cc}
x_1+x_3&=2\\
x_2+x_3&=2\\
\end{array}
$$

$$
\begin{array}{cc}
x_1&=2-1&=1\\
x_2&=2-1&=1\\
x_3&=1\\
\end{array}
$$
* Jadi hasil akhirnya adalah:
$$
\begin{array}{cc}
x_1&=1\\
x_2&=1\\
x_3&=1\\
\end{array}
$$
Contoh soal 2
Selesaikan dengan menggunakan eliminasi gaus 
\begin{array}{cc}
x_1 + x_2 + x_3 =3\\
        2x_1+x_3 = 5\\
        x_1+2x_2   = 3\\
\end{array}
Penyelesaiannya:
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
2 & 0 & 2 & | &5\\
1 & 2 & 0 & | &3\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 1 & -1 & | &0\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 0 & -1 & | &-1/2\\
\end{bmatrix}
\quad
$$
Substitusi balik dari baris ketiga:
$$
\begin{array}{cc}
-x_3&=-1/2\\
x_3&=1/2\
\end{array}
$$
Substitusi balik dari baris kedua:
$$
\begin{array}{cc}
-2x_2&=-1\\
x_2&=1/2\
\end{array}
$$
Substitusi balik dari baris pertama:
$$
\begin{array}{cc}
x_1 + x_2 + x-3& =-1\\
x_1 + 1/2 + 1/2& =3\\
x_1 + 1& = 3\\
x_1& = 2
\end{array}
$$
* Jadi hasil akhirnya adalah:
$$
\begin{array}{cc}
x_1& = 2\\
x_2& = 1/2\\
x_3& = 1/2
\end{array}
$$



Contoh Soal 3
Selesaikan dengan menggunakan eliminasi gaus 
$$
\begin{array}{cc}
        2x_1+2x_2 = 4\\
        x_1+x_2   = 2\\
\end{array}
$$
Penyelesaiannya:
$$
\begin{bmatrix}
2 & 2 &  | &4\\
1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 1 &  | &2\\
1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 1 &  | &2\\
0 & 0 & | &0\\
\end{bmatrix}
\quad
$$
Substitusi balik dari baris pertama:
$$
\begin{array}{cc}
x_1 + x_2&=2\\
x_1&= 2-x_2\\
x_2&= x_2
\end{array}
$$
* Jadi hasil akhirnya adalah:
$$
\begin{array}{cc}
(x_1, x_2)=(2-x_2,x_2)\\
\end{array}
$$
$$
\begin{array}{cc}
jika (x_2 =0) maka ((x_1,x_2)= (2,0)) \\
jika (x_2 =1) maka ((x_1,x_2)= (1,1))\\
jika (x_2 =2) maka ((x_1,x_2)= (0,2))\\
\end{array}
$$
sehingga sistem ini memiliki tak hingga banyak solusi 


Contoh Soal 4
Selesaikan dengan menggunakan eliminasi gaus 
$$
\begin{array}{cc}
        x_1+x_2 = 5\\
        x_1+2x_3  = 6\\
\end{array}
$$
Penyelesaian:
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 2 &| &6\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 1 &| &1\\
\end{bmatrix}
\quad
$$
Substritusi balik dari baris kedua:
$$
\begin{array}{cc}
x_2=1\\
x_1+1=5\\
x_1=4
\end{array}
$$
* Jadi hasil akhirnya adalah:
sistem ini memiliki solusi tunggal yaitu:
$$
\begin{array}{cc}
(x_1=4)\\
(x_2=1)
\end{array}
$$
