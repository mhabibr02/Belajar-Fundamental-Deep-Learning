
# Image Classification Project Belajar Fundamental Deep Learning

## Overview
Pada project ini mengembangkan model CNN berbasis transfer learning untuk mengklasifikasikan gambar Mamalia Hewan
antara lain; african_elephant, alpaca dan polar_bear. Bahasa Pemrograman yang digunakan ialah Python.

## Dataset
- **Nama** : Mammals Animals
- **Sumber**: Kaggle
- **Kelas**: african_elephant, alpaca, polar_bear.
- **Jumlah** (Train 934, Validation 102, Test 60)
- **Resolusi**: (256, 256)

## Metodologi
- **Arsitektur**: MobileNetV2, Conv2D, Pooling, dan Dense
- **Augmentasi**: Rotasi, Translasi, Flip Horizontal, Penyesuaian Kecerahan
- **Callbacks**: ModelCheckpoint, EarlyStopping
- **Inferensi**: Dilakukan menggunakan saved_model, bukti disimpan di `confusion_matrix.png`, `correct_inference.png`,
`inference_result.png` dan `train_image.png`

## Struktur
project/
├── saved_model/
│ ├── assets/
│ │ ├── `accuracy_loss_plot.png`
│ │ ├── `confusion_matrix.png`
│ │ ├── `correct_inference.png`
│ │ ├── `inference_result.png`
│ │ └── `train_image.png`
│ ├── variables/
│ │ ├── `variables.data-00000-of-00001`
│ │ └── `variables.index`
│ ├── `fingerprint.pb`
│ ├── `saved_model.pb`
│ └── `best_model_sequential.h5`
├── tfjs_model/
│ ├── `group1-shard1of3.bin`
│ ├── `group1-shard2of3.bin`
│ ├── `group1-shard3of3.bin`
│ └── `model.json`
├── tflite/
│ ├── `label.txt`
│ └── `model.tflite`
├── `notebook.ipynb`
├── `readme.md`
└── `requirements.txt`

## Hasil
- **Accuracy**: 96.98%
- **Visualisasi**: `accuracy_loss_plot.png`
- **Bukti Inferensi**: `inference_result.png` dan `correct_inference.png`
- **Analisis**: `confusion_matrix.png`
