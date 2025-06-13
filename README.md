# 🍔 Food Image Classification with MobileNetV2

Klasifikasi gambar makanan menggunakan **Transfer Learning** dengan arsitektur **MobileNetV2**.

## 🚀 Fitur Utama
- Menggunakan pretrained **MobileNetV2** sebagai feature extractor
- Fine-tuning pada dataset lokal makanan
- Input gambar 64x64 (RGB)
- Output: Label kategori makanan (multi-class classification), Keseimbangan gizi makanan
- Model disimpan dan bisa digunakan ulang untuk prediksi gambar baru

## 🧪 Dataset
- Folder `train/` dan `test/` berisi subfolder sesuai nama kelas makanan
- Gambar otomatis di-preprocess dan diaugmentasi dengan `ImageDataGenerator`
- Ukuran gambar: **64x64 px**

## 📈 Hasil Model
- Model mencapai akurasi tinggi
- Training & validation accuracy dan loss divisualisasikan
- Model diekspor sebagai file `.h5`
