# LAPBY.03

NAMA: NAUFAL YAZID ALBANI 

NIM:312410279

KELAS:TI.24.A.4

MATKUL:BAHASA PEMOGRAMAN 

## Latihan 1

1. Tampilkan n bilangan acak yang lebih kecil dari 0.5.
2. nilai n diisi pada saat runtime
3. anda bisa menggunakan kombinasi while dan for untuk menyelesaikannya
4. gunakan fungsi random() yang dapat diimport terlebih dahulu

```python
from random import random

N = int(input("Masukkan nilai N: "))

i = 1
while i <= N:
    r = random()
    print(f"data ke: {i} => {r}")
    i += 1
````
## Membangkitkan Nilai Random() memasukan Nilai N dan menggunakan while 

```python
from random import random
````
kode program ini untuk memanggil fungsi `random()` yang terletak pada library python itu sendiri 

```python
N = int(input("Masukkan nilai N: "))
````
memasukan inputan N 

```python
i = 1
while i <= N:
    r = random()
    print(f"data ke: {i} => {r}")
    i += 1
````
kode ini menggunakan perulangan dengan fungsi `while` yang dimana memprogramkan variable i lebih dari N(i=1),dan akan proses ke fungsi random() yang dibungkus oleh variable (r) ,cetak "data {i} yang dimana (i) itu (1),=> ke variable (r) yaitu `random()`

```python
i += 1
````
i+= 1 yaitu akan menambahkan menjadi 2,karena diprogram itu index 1=0,jika 0 < N maka output yang keluar tanpa batas.

hasil program tersebut

![Screenshot 2024-11-01 213958](https://github.com/user-attachments/assets/d687af3a-cf59-4dc3-b65a-899b354c549e)
<img width="271" alt="image" src="https://github.com/user-attachments/assets/9139211f-75ca-4afb-8088-5a9167e17b7b">


