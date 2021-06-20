---
layout: default
author: irosyadi
title:  13. Arsitektur-arsitektur CNN
date: 2021-06-17 21:18:02
category: machine-learning-cv
tags: ["machine learning", "computer vision"]
draft: false
---

# 13. Arsitektur-arsitektur CNN

## Topik
- Pekan 13: Arsitektur-arsitektur CNN
    - Arsitektur untuk klasifikasi: AlexNet, VGG, GoogLeNet, ResNet
    - Arsitektur untuk deteksi: YOLO
    - Dataset *deep learning* untuk *computer vision*
    - Progress proyek

## Pembahasan
Pada awalnya, kita membutuhkan banyak sekali dataset (hingga jutaan) untuk dapat melatih dan menggunakan CNN sehingga dapat melakukan klasifikasi citra dengan handal. Saat ini, kita tidak perlu seberat itu. Ada teknik yang disebut dengan *transfer learning* yang mana kita menambahkan penalaan, pengaturan, lapis, atau pelatihan yang baru terhadap suatu arsitektur yang sudah ada dan dilatih terhadap dataset yang sangat besar. Arsitektur tersebut sudah dikembangkan oleh peneliti dan perusahaan yang memilik sumber daya memadai untuk membangun arsitektur klasifikasi yang handal. Akan tetapi kita tetap perlu melihat karakteristik masing-masing.

## Salindia (slide)
- [CS231n - Lecture 9](http://cs231n.stanford.edu/slides/2021/lecture_9.pdf) (3,2 MB)
- [EECS498 - Lecture 8](https://web.eecs.umich.edu/~justincj/slides/eecs498/FA2020/598_FA2020_lecture08.pdf) (22,2 MB)