---
layout: default
author: irosyadi
title:  7. Convolutional Neural Network (CNN)
date: 2021-06-17 21:18:02
category: machine-learning-cv
tags: ["machine learning", "computer vision"]
draft: false
---

# 7. Convolutional Neural Network (CNN)

## Topik
- Pekan 7: Convolutional Neural Networks (CNN)
    - Sejarah
    - Lapis *Convolution* dan *pooling*
    - Teori dan rancangan jaringan
    - Aplikasi CNN untuk *computer vision* dan aplikasi lain

## Pembahasan
*Convolutional Neural Networks* (CNN) sebagaimana lazimnya suatu jaringan saraf terdiri dari neuron-neuron yang bobot (parameter) serta biasnya dapat diperbarui (dipelajarkan). Setiap neuron menerima masukan, lalu melakukan perkalian dot dan mendapatkan pemicu nonlinear. 

Lalu apa yang berbeda? Arsitektur CNN adalah suatu jaringan saraf yang mengasumsikan masukannya adalah citra sehingga kita dapat merancang sifat arsitektur yang spesifik untuk melakukan klasifikasi citra. Dengan asumsi tersebut, maka kalkulasi parameter (dari suatu citra yang biasanya sangat besar) akan dapat dikurangi. Dalam CNN ada dua jenis lapis yang berfungsi untuk mempercepat klasifikasi citra: lapisan konvolusi dan lapisan *pooling*.

Sebagai suatu jaringan saraf, CNN masih memiliki sifat jaringan saraf: memiliki fungsi skor yang dapat diturunkan, memiliki *loss function* (seperti SVM/Softmax, dan semua trik yang kita pelajari saat melatih jaringan saraf biasa. Akan tetapi, mengingat lapisannya yang banyak dan rumit, kita perlu juga belajar melihat bagaimana visualisasi CNN belajar mengklasifikasi. Kita juga belajar bagaimana mempercepat rancangan arsitektur CNN yaitu dengan menggunakan teknik yang disebut *transfer learning*.

## Salindia (slide)
- [CS231n - Lecture 5](http://cs231n.stanford.edu/slides/2021/lecture_5.pdf) (11 MB)
- [CS294 - Lecture 7](https://bcourses.berkeley.edu/courses/1453965/files/69671012/download) (7 MB)
- [EECS498 - Lecture 7](https://web.eecs.umich.edu/~justincj/slides/eecs498/FA2020/598_FA2020_lecture07.pdf) (9,9 MB)

## Referensi
- [Convolutional Networks](http://cs231n.github.io/convolutional-networks)
- [Understanding CNN](https://cs231n.github.io/understanding-cnn/)
- [Transfer Learning](https://cs231n.github.io/transfer-learning/)