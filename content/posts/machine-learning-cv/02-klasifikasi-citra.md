---
layout: default
author: irosyadi
title:  2. Klasifikasi Citra
date: 2021-06-17 21:18:02
category: machine-learning-cv
tags: ["machine learning", "computer vision"]
draft: false
---

# 2. Klasifikasi Citra

## Topik
- Pekan 2: Klasifikasi Citra
    - Klasifikasi berbasis data (*data-driven*)
    - *k-nearest neighbor*
    - Klasifikasi linear

## Pembahasan
Pada bagian ini kita akan mengenal problem klasifikasi citra. Dalam problem klasifikasi citra, tugas yang harus dilakukan komputer adalah memberikan sebuah label kepada sebuah citra input sesuai dengan kategori yang ditetapkan. Problem klasifikasi citra adalah salah satu problem penting dalam *computer vision* dan memiliki aplikasi praktis yang banyak. Terlebih lagi, berbagai tugas *computer vision* seperti deteksi dan segmentasi obyek bisa direduksi sebagai suatu problem klasifikasi citra.

Pengenalan konsep (obyek) visual bagai manusia relatif mudah, tetapi tidak bagi komputer. Tantangan yang dihadapi komputer di antaranya adalah: variasi sudut pandang, variasi skala, deformasi obyek, tampilan obyek, kondisi pencahayaan, latar belakang, dan variasi bentuk obyek pada kelas sama. Lalu, bagaimanakah cara komputer melakukan klasifikasi citra?

## Salindia (slide)
- [CS231n - Lecture 2](http://cs231n.stanford.edu/slides/2021/lecture_2.pdf) (5,1 MB)
- [CS294 - Lecture 2](https://bcourses.berkeley.edu/courses/1453965/files/69518023/download) (2,6 MB)
- [EECS498 - Lecture 2](https://web.eecs.umich.edu/~justincj/slides/eecs498/FA2020/598_FA2020_lecture02.pdf) (150 MB)

## Referensi
- Bab 1-4 dari buku [Deep Learning](http://www.deeplearningbook.org/)
- [Image Classification Problem](https://cs231n.github.io/classification/)  
- [Linear Classification](https://cs231n.github.io/linear-classify/)

## Rangkuman

- Problem **Klasifikasi Citra** adalah problem yang mana dengan berbekal berbagai himpunan citra yang setiap himpunannya telah diberi label yang sebuah kategori, komputer ditugaskan untuk memprediksi citra uji yang dimasukkan dan diukur tingkat akurasi prediksinya.
- **Nearest Neighbor classifier** adalah sebuah pengklasifikasi sederhana dengan beberapa *hyper-parameter* (seperti nilai *k*, atau jarak yang digunakan untuk membandingkan contoh). Penentuan nilai hyper-parameter ditentukan oleh perancang algoritme klasifikasi.
- Penentuan hyper-parameter dapat dilakukan dengan membagi data latih menjadi dua: data pelatihan (training set) dan data validasi (validation set) yang diikuti dengan pengubahan nilai hyper-parameter untuk mendapatkan unjuk kerja klasifikasi terbaik.
- Data pelatihan yang terbatas dapat diatasi dengan prosedur **cross-validation** yang akan membantu mengurangi derau/kesalahan dalam mengestimasi hyper-parameter terbaik.
- Ketika hyper-parameter yang terbaik ditemukan, dilakukan **evaluation** pada data set uji yang sesungguhnya.
- Algoritme *Nearest Neighbor* hanya dapat mencapai akurasi 40% pada datset CIFAR-10. *Nearest neighbor* secara algoritme sederhana tetapi secara komputasi lambat dan membutuhkan penyimpanan data besar.
- Penghitungan jarak L1 dan L2 pada nilai piksel mentah tidak mencukupi, karena jarak lebih berkorelasi dengan latar belakang (background) dan distribusi warna daripada muatan semantik dari gambar itu sendiri.

## Ringkasan

- Problem klasifikasi citra Image memiliki banyak tantangan seperti di antaranya adalah pencahayaan (*illumination*) dan sudut pandang (*viewpoint*).
  - ![](https://raw.githubusercontent.com/mbadry1/CS231n-2017-Summary/master/Images/39.jpeg)
- **K nearest neighborhood** (KNN) adalah salah satu algoritme klasifikasi citra, tapi unjuk kerjanya tidak bagus. Sifat-sifat KNN adalah:
  - Jenis hyperparameter dari KNN adalah: *k* dan ukuran jarak.
  - *k* adalah jumlah tetangga (*neighbor*) yang dibandingkan.
  - Ukuran jarak yang digunakan di antaranya adalah:
    - L2 distance (Euclidean distance) : lebih baik untuk titik non koordinat
    - L1 distance (Manhattan distance) : lebih baik untuk titik koordinat
- Hyperparameter dapat dioptimalkan dengan teknik validasi silang (*cross-validation*) (dalam hal ini untuk memprediksi *k*) sebagai berikut :
  1. Bagi dataset menjadi `f` lipatan (*fold*).
  2. Pada setiap hyperparameter yang terprediksi:
     - Latih algoritme dengan lipatan f-1 dan tes dengan lipatan tersisa. Ulang langkah ini untuk setiap lipatan.
  3. Pilih hyperparameter yang memberikan nilai pelatihan terbaik (atas rata-rata semua lipatan)
- Algoritme **Linear SVM** adalah salah satu teknik klasifikasi citra, tapi ia memiliki problem kutukan dimensi (*curse of dimension*) yang membuatnya berhenti melakukan perbaikan unjuk kerja.
- Algoritme **Logistic regression** juga merupakan salah satu teknik klasifikasi citra, tetapi karena klasifikasi citra bersifat non linear, unjuk kerjanya tidak cukup bagus.
