# **machine_learning**


# 🍱 Food Classification with CNN

Deteksi jenis makanan dari gambar menggunakan Convolutional Neural Network (CNN). Proyek ini dikembangkan untuk mengklasifikasikan gambar makanan ke dalam beberapa kategori menggunakan deep learning.

## 🔍 Ringkasan
- Input: Gambar makanan (ukuran 64x64 piksel, 3 channel RGB)
- Output: Label kategori makanan (contoh: nasi goreng, ayam goreng, rendang, dll)
- Model: CNN menggunakan Keras Sequential API
- Dataset: Terstruktur dalam folder `train/` dan `test/` dengan subfolder untuk tiap kelas

## 🧠 Arsitektur Model
- 2x Convolutional Layer (32 dan 64 filter) + ReLU + MaxPooling
- Flatten → Dense 128 unit → Dropout 0.5
- Output: Dense dengan softmax sesuai jumlah kelas makanan

## 📈 Evaluasi Model
- Akurasi training & validasi divisualisasikan tiap epoch
- Model diekspor ke file `.h5` untuk deployment

## 🛠️ Tools & Library
- Python
- TensorFlow / Keras
- Matplotlib
- NumPy
