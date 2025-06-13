# 🍔 Food Image Classification with MobileNetV2

Klasifikasi gambar makanan menggunakan **Transfer Learning** dengan arsitektur **MobileNetV2**.

## 🚀 Fitur Utama
- Menggunakan pretrained **MobileNetV2** sebagai feature extractor
- Fine-tuning pada dataset lokal makanan
- Input gambar 64x64 (RGB)
- Output: Label kategori makanan (multi-class classification)
- Model disimpan dan bisa digunakan ulang untuk prediksi gambar baru

## 🧠 Arsitektur Model
- Base model: `MobileNetV2` dari TensorFlow (tanpa top layers)
- Layer tambahan (custom head):
  - `GlobalAveragePooling2D`
  - `Dense(128, activation='relu')`
  - `Dropout(0.5)`
  - `Dense(num_classes, activation='softmax')`
- Loss function: `categorical_crossentropy`
- Optimizer: `adam`
- Metrics: `accuracy`

## 🧪 Dataset
- Folder `train/` dan `test/` berisi subfolder sesuai nama kelas makanan
- Gambar otomatis di-preprocess dan diaugmentasi dengan `ImageDataGenerator`
- Ukuran gambar: **64x64 px**

## 📈 Hasil Model
- Model mencapai akurasi tinggi
- Training & validation accuracy dan loss divisualisasikan
- Model diekspor sebagai file `.h5`
