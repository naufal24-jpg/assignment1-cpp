# Laporan Programming Assignment 1: Basic C++
# REPORT - Programming Assignment 1

## 1. Deskripsi Program

Program ini dibuat untuk menghitung umur seseorang berdasarkan tanggal lahir yang diinputkan oleh pengguna. Program akan menghasilkan umur dalam tahun, umur dalam bulan, serta hari dalam seminggu dari tanggal lahir tersebut.

---

## 2. Input dan Output

### Input

Format input:

```
dd/mm/yyyy
```

Contoh:

```
12/05/2005
```

### Output

Format output:

```
tahun bulan hari
```

Contoh:

```
20 250 Kamis
```

---

## 3. Algoritma Program

### a. Menghitung Umur dalam Tahun

* Menghitung selisih tahun antara tanggal sekarang dan tanggal lahir
* Jika ulang tahun belum terjadi pada tahun ini, maka umur dikurangi 1

### b. Menghitung Umur dalam Bulan

* Menghitung selisih tahun dan dikonversi ke bulan
* Menambahkan selisih bulan
* Jika tanggal sekarang lebih kecil dari tanggal lahir, maka dikurangi 1 bulan

### c. Menentukan Hari

* Menggunakan fungsi `mktime()` dari library `<ctime>`
* Mengambil nilai `tm_wday` untuk menentukan hari

---

## 4. Struktur Program

Program terdiri dari beberapa fungsi utama:

* `yearsOld()` → menghitung umur dalam tahun
* `monthsOld()` → menghitung umur dalam bulan
* `dayOfDate()` → menentukan hari dari tanggal

---

## 5. Kesimpulan

Program ini berhasil menghitung umur dalam tahun dan bulan serta menentukan hari dari tanggal lahir menggunakan fungsi bawaan C++. Penggunaan struktur `tm` mempermudah pengolahan data tanggal.
