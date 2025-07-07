
# Proyek Deep Learning - Klasifikasi Gambar Cuaca  
**Nurul Asyrifah**

### Latar Belakang

Cuaca memengaruhi berbagai aktivitas manusia, namun tidak semua wilayah memiliki sensor cuaca otomatis. Dengan memanfaatkan gambar dan teknologi deep learning, kita bisa mengembangkan sistem klasifikasi kondisi cuaca yang murah dan cepat.  

Model CNN dalam proyek ini dilatih untuk mengenali **4 kelas cuaca**:
- `cloudy`
- `rain`
- `shine`
- `sunrise`

---


### Goals

- Membangun CNN untuk klasifikasi cuaca.
- Mengevaluasi akurasi model.
- Mengekspor model ke `.tflite`, `.tfjs`, dan `saved_model`.

---

### Dataset
- **Sumber Dataset**: [Weather Dataset – Kaggle](https://www.kaggle.com/datasets/pratik2901/multiclass-weather-dataset)
- **Jumlah Kelas**: 4 (cloudy, rain, shine, sunrise)


### Struktur folder dataset:

```
dataset/
├── train/
│   ├── cloudy/
│   ├── rain/
│   ├── shine/
│   └── sunrise/
├── val/
│   ├── cloudy/
│   ├── rain/
│   ├── shine/
│   └── sunrise/
└── test/
    ├── cloudy/
    ├── rain/
    ├── shine/
    └── sunrise/
```
---

### Cara menjalankan Proyek
### 1. Struktur folder proyek

```
project_folder/
├── exported_model/
│   ├── saved_model_format/
│   ├── tflite/
│   ├── tfjs_model/
│   └── label.txt
├── dataset/
│   ├── train/
│   ├── val/
│   └── test/
├── train_model.ipynb
└── requirements.txt
```

### 2. Instalasi dependensi

```bash
pip install -r requirements.txt
```

### 3. Jalankan pelatihan

Buka `train_model.ipynb`, jalankan semua sel. Model akan diekspor otomatis ke:

- `saved_model_format/`
- `model.tflite`
- `tfjs_model/`
- `label.txt`

termasuk melakukan prediksi dengan interfence.

---

### Kesimpulan

Model CNN ini berhasil mengklasifikasikan gambar cuaca dengan performa baik. Dengan konversi ke berbagai format, model siap untuk digunakan di berbagai platform seperti website dan aplikasi Android.

---

> Proyek ini merupakan bagian dari eksplorasi deep learning terapan untuk klasifikasi visual berbasis citra cuaca.
