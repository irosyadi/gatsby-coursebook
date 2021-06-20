---
layout: default
author: irosyadi
title:  4. Klasifikasi Linear
date: 2021-06-17 21:18:02
category: machine-learning-cv
tags: ["machine learning", "computer vision"]
draft: false
---
# 4. Klasifikasi Linear

## Topik
- Pekan 4: Klasifikasi Linear
    - Klasifikasi linear
    - Fitur citra

## Pembahasan
Pada topik yang lalu, kita belajar tentang problem klasifikasi citra yang mana komputer ditugaskan untuk memberikan label pada sebuah citra dengan menggunakan teknik k-Nearest Neighbor (kNN). Akan tetapi, kNN memiliki beberapa kelemahan.

Selanjutnya kita akan belajar tentang bagaimana menggunakan teknik yang lebih baik daripada kNN. Teknik yang akan dipakai akan menggunakan dua komponen utama: fungsi skor (yang memetakan data menjadi skor kelas) dan *loss function* yang mengukur kedekatan skor yang diprediksi dengan label sesungguhnya. Kita meletakkan ini sebagai problem optimsasi yang mana kita akan meminimalkan *loss function* terhadap parameter fungsi skor.

## Salindia (slide)
- [CS231n - Lecture 3](http://cs231n.stanford.edu/slides/2021/lecture_3.pdf) (4,3 MB)
- [CS294 - Lecture 3](https://bcourses.berkeley.edu/courses/1453965/files/69531253/download) (1,2 MB)
- [EECS498 - Lecture 3](https://web.eecs.umich.edu/~justincj/slides/eecs498/FA2020/598_FA2020_lecture03.pdf) (79,6 MB)

## Referensi
- [Linear Classification](https://cs231n.github.io/linear-classify/)