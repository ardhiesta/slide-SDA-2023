---
marp: true
---

# Asymptotic Analysis

## Struktur Data dan Algoritma

#### Ardhi Wijayanto

Informatika
Universitas Sebelas Maret
2023

---

> Diberikan 2 algoritma untuk menyelesaikan suatu problem. Bagaimana menentukan algoritma mana yang paling bagus?

### Cara-1

Implementasikan kedua algoritma ke dalam program
Jalankan program
Hitung waktu yang dibutuhkan kedua algoritma

---

## Kelemahan Cara-1

* Perbedaan **input untuk test** : 
Algoritma pertama bisa jadi lebih bagus dari algoritma kedua untuk input tertentu. Dan untuk sejumlah input yang lain algoritma kedua lebih bagus daripada algoritma pertama.
* Perbedaan **spesifikasi komputer** : 
Pada komputer X, algoritma pertama lebih bagus dari pada algoritma kedua. 
Pada komputer Y, didapatkan hasil algoritma kedua lebih bagus daripada algoritma pertama.

---

## Contoh : Linear Search vs Binary Search

Mencari sebuah nilai di dalam array. Temukan karakter **G** pada sorted array yang memuat karakter A - R. 

{'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O, 'P', 'Q', 'R'}

---

## Linear Search vs Binary Search

Skenario :
* Linear Search dijalankan pada komp-A
* Binary Search dijalankan pada komp-B
* Komputer A dan B sudah diukur dan bandingkan kemampuan komputasinya. Misal komp-A memiliki nilai 0,2 dan komp-B nilainya 1.000 (artinya komp-A 5.000 kali lebih powerful dibanding komp-B).

---

## Linear Search vs Binary Search

Berdasarkan skenario 
> Linear Search pada komp-A 
Binary Search pada komp-B
kemampuan komp-A 5.000x komp-B

* Pada array yang ukurannya kecil, komp-A bisa menyelesaikan search lebih cepat dari komp-B.
* Pada array tertentu yang ukurannya jauh lebih besar, Binary Search yang dijalankan pada komp-B dapat menyelesaikan search lebih cepat daripada Linear Search pada komp-A. 

---

## Linear Search vs Binary Search

![search](https://raw.githubusercontent.com/ardhiesta/slide-SDA-2023/main/images/linear_binary_runtime.jpg)

---

## Linear Search vs Binary Search

Waktu yang dibutuhkan untuk menyelesaikan searching pada **Binary Search** meningkat secara **logaritmik** seiring pertumbuhan ukuran array. Sedangkan pada **Linear Search**, pertambahan waktunya meningkat secara **linear**.

---

## Linear Search 

![Image](https://www.baeldung.com/wp-content/ql-cache/quicklatex.com-d3dd66a9a897f6adac0921c872da5173_l3.svg)

---

## Binary Search 

![Image](https://www.baeldung.com/wp-content/ql-cache/quicklatex.com-73f4953cdc21e359c0336f4fb943052f_l3.svg)

---

## Linear Search vs Binary Search

Mencari sebuah nilai di dalam array

![search](https://i0.wp.com/algorithms.tutorialhorizon.com/files/2019/08/Linear-Search-VS-Binary-Search.png?resize=548%2C462&ssl=1)

---

## Notasi Big O

*Time complexity*
Mendefinisikan seberapa lama (*runtime*) suatu algoritma dijalankan seiring dengan bertambahnya data.

---

> Mengapa repot-repot menghitung *time complexity*?

Skalabilitas, pertumbuhan data
Umur pakai program

---

## Time Complexity

![chart](https://raw.githubusercontent.com/ardhiesta/slide-SDA-2023/main/images/chartBigO.jpg)

---

## Terima kasih

Source code slide ini dapat dilihat di https://github.com/ardhiesta/slide-SDA-2023

---

# Referensi

https://www.geeksforgeeks.org/analysis-of-algorithms-set-1-asymptotic-analysis/
https://www.baeldung.com/cs/linear-search-vs-binary-search
https://betterprogramming.pub/big-o-notation-for-dummies-like-me-98ac2d141f9f