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
![Screenshot 2024-11-01 214226](https://github.com/user-attachments/assets/ca431fd5-d0fc-47e6-882c-69ad4e8be924)
![Screenshot 2024-11-01 214413](https://github.com/user-attachments/assets/cee16f20-ee3e-44a1-b159-d932940fec0c)

## latihan 2

Latihan 2: latihan2.py
Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan modal
awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada bulan ketiga
baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5, pendapatan meningkat 5%,
selanjutnya pada bulan ke 8 mengalami penurunan keuntungan sebesar 2%, sehingga laba
menjadi 3%. Hitung total keuntungan selama 8 bulan berjalan usahanya.

```python
laba = 0
total_laba = 0

for bulan in range(1, 9):
    if bulan in [1, 2]:
        laba = 0
    elif bulan in [3, 4]:
        laba = 10000000.0
    elif bulan in [5, 6, 7]:
        laba = 5000000.0
    elif bulan in [8]:
        laba = 20000000.0
    print(f"laba bulan ke- {bulan} sebesar: {laba}")
    
    total_laba += laba
print(f"Total laba adalah: {total_laba}")

````
hasil program tersebut

![Screenshot 2024-11-01 214812](https://github.com/user-attachments/assets/74593595-8bd7-4b7b-aa54-cb07e0029068)

## hitung total selama 8 bulann berjalan usahanya

```python
laba = 0
total_laba = 0

````
variable yang dimasukan dengan angka 0

```python
for bulan in range(1, 9):
````
fungsi `for` sama saja dengan `while` yaitu for perulangan yang bisa diketahui tanpa menggunakan struktur kondisi 

untuk`(, 9)` akan melakukan perulangan dari 1-9 kalau di bahasa pemograman index yaitu 0-8

```python
if bulan in [1, 2]:
        laba = 0
````
jika bulan didalam 1 dan 2 maka laba 0

```python
elif bulan in [3, 4]:
        laba = 10000000.0
````
jika bulan didalam 3 dan 4 maka laba 10000000.0

```python
elif bulan in [5, 6, 7]:
        laba = 5000000.0
````
jika bulan didalam 5,6 dan 7 maka laba 5000000.0

```python
elif bulan in [8]:
        laba = 20000000.0
    print(f"laba bulan ke- {bulan} sebesar: {laba}")

````
jika bulan didalam 8 maka laba akan mencetak perulangan 1-8 sesuai program range yang diinginkan 

```python
total_laba += laba
print(f"Total laba adalah: {total_laba}")

````
dan memproses akan menghitung semua hasil data yang di kumpulkan

## latihan 3

Latihan 2: latihan2.py
Seorang pengusaha menginvestasikan uangnya untuk memulai usahanya dengan modal
awal 100 juta, pada bulan pertama dan kedua belum mendapatkan laba. pada bulan ketiga
baru mulai mendapatkan laba sebesar 1% dan pada bulan ke 5, pendapatan meningkat 5%,
selanjutnya pada bulan ke 8 mengalami penurunan keuntungan sebesar 2%, sehingga laba
menjadi 3%. Hitung total keuntungan selama 8 bulan berjalan usahanya.

```python
saldo = 1000000

while True:
    print(f"Saldo saat ini: Rp {saldo}")
    print("1. Tarik Uang")
    print("2. Keluar")
    pilihan = input("Pilih menu : ")

    if pilihan == '1':
        jumlah_penarikan = int(input("Masukkan jumlah penarikan: "))
        if jumlah_penarikan <= saldo:
            saldo -= jumlah_penarikan
            print("Penarikan berhasil!")
        else:
            print("Saldo tidak mencukupi!")
    elif pilihan == '2':
        print("Terima kasih telah menggunakan ATM!")
        break
    else:
        print("Pilihan tidak valid!")

    print()  # Menambahkan baris kosong untuk pemisah antar transaksi

````
## membuat program ATM sederhana 

```python
saldo = 1000000

````
dengan memasukan variable saldo untuk menentukan jumlah saldo tersebut 

```python
while True:
    print(f"Saldo saat ini: Rp {saldo}")
    print("1. Tarik Uang")
    print("2. Keluar")
    pilihan = input("Pilih menu : ")

````
kode ini menggunakan while yaitu perulangan jika salah menginputkan atau sudah selesai menginputkan,program akan terus berlanjut

```python
if pilihan == '1':
        jumlah_penarikan = int(input("Masukkan jumlah penarikan: "))
        if jumlah_penarikan <= saldo:
            saldo -= jumlah_penarikan
            print("Penarikan berhasil!")
        else:
            print("Saldo tidak mencukupi!")

````
Menggunakan sruktur Kondisi if else, yang dimana jika memilih angka 1, akan memasukan menu Tarik uang, yang dimana program tersebut akan menjalani

jika memilih angka 1, jumlah yang ingin di tarik lebih kecil dari saldo maka (salso -= jumlah penarikan) yang artinya jumlah saldo akan di kurangi dengan inpitan yang dimasukan, dan akan mencetak "Penarikan berhasil"

Jika inputan penarikan melebihi saldo akan mencetak "Saldo tidak mencukupi"

```python
elif pilihan == '2':
        print("Terima kasih telah menggunakan ATM!")
        break
    else:
        print("Pilihan tidak valid!")

    print()  # Menambahkan baris kosong untuk pemisah antar transaksi

Dan Jika memilih angka 2, maka yang di pilih Output Keluar, yang mencetak "Terima kasih telah menggunakan ATM!", dan akan memproses ke fungsi `break()` yang berfungsi untuk menghentikan Perulangan atau `while` tersebut

jika tidak memilih selain 1 atau 2, akan mencetak "Pilihan tidak valid!", dan fungsi `print()` Untuk Menambahkan baris kosong untuk pemisah antar transaksi


hasil program tersebut

![Screenshot 2024-11-01 221105](https://github.com/user-attachments/assets/51c61b4c-487a-4297-b566-21c13b6e31b0)


