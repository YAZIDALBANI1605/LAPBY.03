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
