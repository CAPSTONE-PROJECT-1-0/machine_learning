# 🍔 Food Image Classification with MobileNetV2

Klasifikasi gambar makanan menggunakan **Transfer Learning** dengan arsitektur **MobileNetV2**.

## 🚀 Fitur Utama
- Menggunakan pretrained **MobileNetV2** sebagai feature extractor
- Output: Label kategori makanan (multi-class classification), Keseimbangan gizi makanan
- Model disimpan dan bisa digunakan ulang untuk prediksi gambar baru

## 🧪 Dataset
- Folder `train/` dan `test/` berisi subfolder sesuai nama kelas makanan
- Gambar otomatis di-preprocess dan diaugmentasi dengan `ImageDataGenerator`

## 📈 Hasil Model
- Training & validation accuracy dan loss divisualisasikan
- Model diekspor sebagai file `.h5`
