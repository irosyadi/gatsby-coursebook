---
layout: default
author: irosyadi
title:  5. Optimisasi
date: 2021-06-17 21:18:02
category: machine-learning-cv
tags: ["machine learning", "computer vision"]
draft: false
---

# 5. Optimisasi

## Topik
- Pekan 5: Optimisasi (*optimization*)
    - *Loss functions*
    - *Optimization*
    - *Stochastic gradient descent*

## Pembahasan
Pada bagian sebelumnya kita membahas dua komponen penting dalam klasifikasi citra:

- Fungsi skor yang memetakan piksel citra ke skor kelas (yaitu menggunakan fungsi linear)
- *Loss function* yang mengukur kualitas parameter berdasarkan seberapa dekat skor yang diperoleh terhadap label benar pada data pelatihan. Kita menggunakan algoritme Softmax/SVM untuk itu.

Selanjutnya kita akan belajar komponen ketiga yaitu **optimisasi**. Optimisasi adalah proses mencari parameter (bobot) yang meminimalkan *loss function*. Lebih lanjut, setelah kita memahami bagaimana ketiga komponen tersebut berinteraksi, selanjutnya kita akan mengembangkan komponen pertama (fungsi skor) dari fungsi linear menjadi fungsi yang lebih kompleks: jaringan saraf, dan *convolutional neural network* (CNN).


## Salindia (slide)
- [CS231n - Lecture 3](http://cs231n.stanford.edu/slides/2021/lecture_3.pdf) (4,3 MB)
- [CS294 - Lecture 4](https://bcourses.berkeley.edu/courses/1453965/files/69573147/download) (1,5 MB)
- [EECS498 - Lecture 4](https://web.eecs.umich.edu/~justincj/slides/eecs498/FA2020/598_FA2020_lecture04.pdf) (66,9 MB)

## Referensi
- [Chapter 8: Optimization](http://www.deeplearningbook.org/contents/optimization.html) dari buku [Deep Learning](http://www.deeplearningbook.org/)
- [Linear Classification](https://cs231n.github.io/linear-classify/)  
- [Optimization](https://cs231n.github.io/optimization-1/)