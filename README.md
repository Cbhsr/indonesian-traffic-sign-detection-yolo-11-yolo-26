# indonesian-traffic-sign-detection-yolo-11-yolo-26
Source code eksperimen skripsi: Evaluasi arsitektur YOLO11s dan YOLO26s dengan Augmentasi Mosaic untuk deteksi rambu lalu lintas Indonesia

##  Abstrak Eksperimen
Penelitian ini membandingkan dua arsitektur *state-of-the-art* (YOLO11s dan YOLO26s) dalam melokalisasi dan mengklasifikasi 30 kelas rambu lalu lintas di Indonesia. Eksperimen ini berfokus pada manipulasi probabilitas **Mosaic Augmentation (1.0 dan 0.5)** untuk mengatasi masalah deteksi objek kecil (*small object detection*) dan oklusi dengan variabel kontrol regularisasi *optimizer* AdamW.

## 🛠️ Lingkungan Komputasi
- **Platform:** Google Colab / Kaggle
- **GPU:** NVIDIA Tesla T4 (14.6 GB VRAM)
- **Framework:** Ultralytics YOLO (v8.4.80) & PyTorch (2.11.0+cu128)
- **Reproducibility:** Seed 42 (Global & Deterministic)

## 📁 Struktur Repositori
- `lengkap-1.ipynb` : *Jupyter Notebook* utama yang memuat instalasi, ekstraksi dataset, pemanggilan *training*, hingga visualisasi metrik evaluasi.
- `/results` : Kumpulan grafik evaluasi (Confusion Matrix, Kurva Loss, Heatmap AP).
- `data.yaml` : Konfigurasi dataset untuk *framework* Ultralytics.

## 📊 Dataset
Dataset yang digunakan bersumber dari [Roboflow Universe: Traffic Sign in Indonesia Detection](https://universe.roboflow.com/putri-mawaring-wening-lwwcx/traffic-sign-in-indonesia-detection)  yang terdiri atas 11.157 citra dengan distribusi 30 kelas unik.

---
Dikembangkan oleh Bena Mahogra  - Universitas Amikom Yogyakarta (2026).
